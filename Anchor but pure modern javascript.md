# <\a> but pure modern javascript 
1.  Anchor functionality using a button element (odins-crow.com inspiration)
	- Only updates main content (prevents refreshing unlike an anchor element).
	- Uses `fetch()` then `new DOMParser()` to get the element id in this case.
	- Finally loads new main element content.
	- NOTE: after enough bloody research I finally achieve this by just only using pure javascript (can't be bothered using some other frameworks like react, SSI, or CMS etc. so I can explore the javascript ecosystem more) and finally I'll honor a thankful appreciation to chatgpt.
 2. Save & restore state when refreshing using `localStorage.setItem()`
3. Updates url using `history.pushState()`

```javascript
// fetch-parser.js
import appFunctions from "../animation";

async function fetchHtmlContent(url, elementId, newUrl, currentApp) {
  const response = await fetch(url);
  const htmlText = await response.text();

  const parser = new DOMParser();
  const docFull = parser.parseFromString(htmlText, "text/html");

  const parsedContent = docFull.getElementById(elementId);

  history.pushState(null, null, newUrl);

  document.getElementById("fetch-parser-content").innerHTML =
    parsedContent.innerHTML;

  if (appFunctions[currentApp]) {
    appFunctions[currentApp].forEach((key) => {
      key();
    });
  } else {
    console.log("App not found!");
  }

  localStorage.setItem(
    "pageState",
    JSON.stringify({ url, elementId, newUrl, currentApp })
  );
}

export default fetchHtmlContent;
```

```javascript
// restore-state.js

import fetchHtmlContent from "./fetch-parser";

const restoreState = () => {
  const savedState = localStorage.getItem("pageState");
  if (savedState) {
    const { url, elementId, newUrl, currentApp } = JSON.parse(savedState);
    fetchHtmlContent(url, elementId, newUrl, currentApp);
  }
};

export default restoreState;
```

