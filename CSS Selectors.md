# 🎨 CSS Selectors
###### **SEARCH THE OTHER KIND OF SELECTOR. EXPLAIN THE FUNCTION. GIVE AT LEAST 10.**

**Rosacay, Ike Andrie N.**
**ICT 11 - 5 Programming**
*2024-04-25*
## 🔧Basic Selectors

##### 1. Type Selector
Selects elements of the specified type.
```css
body {
	background-color: #000;
}
```
##### 2.  Class Selector
Opt for specific class attribute.
```css
.container {
	max-width: 69vw;
}
```
##### 3. ID Selector
Choose for specific class attribute.
```css
#navbar {
	max-width: 69vw;
}
```
##### 4. Universal Selector
Selects a single element with the specified id attribute.
```css
* {
	box-sixing: border-box;
}
```
##### 5. Attribute Selector
Pick elements based on an attribute or attribute value.
```css
[type="button"] {
    background-color: green;
    color: white;
}
```

## ⚙️ Combinators
##### 6. Descendant combinator
Selects elements that are descendants of another element.
```css
div p {
    margin-left: 20px;
}
```
##### 7. Child combinator
Choose direct children of an element.
```css
ul > li {
    list-style-type: none;
}
```
##### 8. Adjacent Sibling combinator
Filter an element that is directly after another spicific element.
```css
h1 + p {
    margin-top: 0;
}
```
##### 9. General Sibling combinator
Elect all elements that are sibling of a specified element.
```css
h1 ~ p {
    color: grey;
}
```
## 🧲 Psuedo-Class Selector
##### 10. A pseudo-class is used to define a special state of an element. It can be used to style an element when it is in a certain state or condition. For example, pseudo-classes can target elements when they are hovered over, focused, or checked, among other states. Pseudo-classes begin with a colon (`:`).

**Some common pseudo-elements include:**
- `:hover` — Applies styles when the user hovers over an element with the mouse.
- `:focus` — Applies styles when the element has focus (e.g., input fields when clicked).
- `:active` — Applies styles when the element is being activated (e.g., clicked on).
- `:nth-child()` — Applies styles to elements based on their position in a group of siblings.
- `:first-child` and `:last-child` — Target the first or last element among a group of sibling elements.

*Use case example:*
```css
/* Psuedo-class example: change to certain color when hover */
.specified-class:hover {
	color: rgb(34, 18, 109);
}

/* another example */
div:nth-child(4) {
	font-size: var(size-3xl);
}
```
## 🔗 Psuedo-Elements Selector
##### 11. A pseudo-element is used to style specific parts of an element. Pseudo-elements can be thought of as targeting virtual elements that exist within other elements, allowing you to style certain parts without the need to add extra markup (HTML) to the page. Pseudo-elements begin with two colons (`::`).

**A few common pseudo-elements are:**
- `::before` — Inserts and styles content before the content of the selected element.
- `::after` — Inserts and styles content after the content of the selected element.
- `::first-letter` — Applies styles to the first letter of the first line of a block-level element.
- `::first-line` — Applies styles to the first formatted line of a text inside a block-level element.
- `::selection` — Applies styles to the portion of a document that has been highlighted (selected) by the user.

*Use case example:*
```css
/* Pseudo-element example: add content before a header */
h1::before {
    content: "★ ";
    color: red;
}
```
