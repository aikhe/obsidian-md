---
cssClass: wide-page
---

Activity for today study The HTML \<form> Elements and list them on the microsoft word together the functionality.

**Rosacay, Ike Andrie N.**
**ICT 11-5**
*2024-04-30*
   
<h1 style="text-align: center">
  The HTML
  <strong style="font-family: monospace; font-family: monospace; color: #404754"
    >&lt;<strong style="color: #e06c75">form</strong>&gt;</strong
  >
  Element
</h1>

<form style="display: flex; justify-content: center;">
	<fieldset>
	    <legend>Personal Information</legend>
	    <label for="name">Pangalan:</label>
	    <input type="text" id="name" name="name" required><br><br>
	    <label for="email">Email:</label>
	    <input type="email" id="email" name="email" required><br><br>
	    <label for="birthdate">Petsa ng Kapanganakan:</label>
	    <input type="date" id="birthdate" name="birthdate" required><br><br>
	</fieldset>
	<fieldset>
	    <legend>Course Details</legend>
	    <label for="course">Pumili ng Kurso:</label>
	    <select id="course" name="course">
	            <option value="watercolor">Portrait Art</option>
	    </select><br><br>
	    <label for="experience">Karanasan sa Art:</label>
	    <textarea id="experience" name="experience" rows="4" cols="15" placeholder="I-share ang iyong art journey..."></textarea>
	</fieldset>
	<fieldset>
	    <legend>Additional Preferences</legend>
	    <label for="favoriteTool">Paboritong Art Tool:</label>
	    <input list="tools" id="favoriteTool" name="favoriteTool">
	    <datalist id="tools">
	        <option value="Brush">
	        <option value="Pencil">
	        <option value="Chisel">
	        <option value="Palette">
	    </datalist><br><br>
	    <label>Need accommodation?</label>
	    <input type="checkbox" id="accommodation" name="accommodation"><br><br>
	    <label for="output">Expected Fee (PHP):</label>
	    <output id="output" name="output" for="course">3000</output><br><br>
	</fieldset>
</form>

<br>

<div
  style="
    display: flex;
    gap: 1rem;
    max-width: 60rem;
    margin: auto;
    border: solid rgba(164, 167, 177, 0.582) 2px;
    border-radius: 6px;
    padding-left: 2rem;
    padding-right: 2rem;
    padding-bottom: 1rem;
  "
>
  <h3 style="white-space: nowrap; margin-right: 1rem">
    What is the<br />
    <strong
      style="font-family: monospace; font-family: monospace; color: #404754"
      >&lt;<strong style="color: #e06c75">form</strong>&gt;<br
    /></strong>
    Element?
  </h3>
  <div>
    <p>
      Think of the <strong>&lt;form&gt;</strong> tag as the
      <strong>main container</strong> or ‘bahay’ where
      <strong>all your user input elements live</strong> —like text boxes,
      dropdowns, checkboxes, and buttons. When you're building a web page and
      need to gather some input from users,
      <strong><strong>&lt;form&gt;</strong> is your go-to element</strong>.
    </p>
    <li>
      It's the stage where <strong>all your form elements perform</strong>.
      Basically, <code>&lt;form&gt;</code> is the container that
      <strong>holds all your input fields</strong>, buttons, and other elements
      na <i>kailangan mo para sa user input and interaction on a webpage</i>.
    </li>
  </div>
</div>

<br>

<div
  style="
    display: grid;
    grid-template-columns: auto auto;
    gap: 1rem 2rem;
    margin-bottom: 1rem;
  "
>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      1.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">input</strong>&gt;</strong
      >
    </h4>
    <li>
      Ito ung <strong>jack-of-all-trades</strong> sa mundo ng forms. Think of it
      as your <strong>all-around</strong> utility player sa basketball; kaya
      niyang maging text box, radio button, checkbox, at iba pa. Depende sa
      <code>&nbsp;type&nbsp;</code> attribute niya,
      <strong>he can be whoever you want him to be!</strong>
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      2.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">label</strong>&gt;</strong
      >
    </h4>
    <li>
      Ang best friend ng mga <code>&lt;input&gt;</code> fields.
      <strong>Labels provide descriptions or labels</strong> (obviously, di ba?)
      for your inputs,
      <i
        >making it easier for users to understand kung ano ba talaga ang
        kailangan nilang ilagay</i
      >. Plus, kapag nag-click ka sa label,
      <strong>active rin ang linked input field</strong>. Teamwork makes the
      dream work!
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      3.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">select</strong>&gt;</strong
      >
    </h4>
    <li>
      Parang dropdown menu sa mga fast food.
      <strong>This element lets users pick from a list of options</strong>.
      Kapag pinindot mo,
      <i>magbubukas ito at ipapakita ang mga "items" na pwede mong i-choose</i>.
      <strong>Handy for saving space</strong> on forms habang pinapakita ang mga
      choices na parang menu.
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      4.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">textarea</strong>&gt;</strong
      >
    </h4>
    <li>
      Kung novelist ka, love mo 'to.
      <strong>It's a bigger text box designed for longer inputs</strong>, like
      comments or messages. Pwede kang magsulat ng mini-essay dito
      <strong>without worrying about running out of space</strong>.
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      5.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">button</strong>&gt;</strong
      >
    </h4>
    <li>
      Ito ang buzzer beater shot ng form!
      <strong
        >Buttons are there to submit data, reset forms, or trigger specific
        actions</strong
      >. They come in all shapes and sizes,
      <i>ready to be clicked para magpatuloy sa susunod na action!</i>
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      6.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">fieldset</strong>&gt;</strong
      >
    </h4>
    <li>
      Imagine mo, ito ung parang <strong>organizer</strong> ng iyong forms.
      <strong>It groups related elements together</strong>,
      <i>making your form easier to understand</i>. Parang putting all your arts
      tools sa isang box <strong>para organized ka</strong>.
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      7.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">legend</strong>&gt;</strong
      >
    </h4>
    <li>
      <strong>Partner in crime</strong> ng <code>&lt;fieldset&gt;</code>.
      <strong
        >It provides a caption or a title sa mga groups na ginawa mo</strong
      >
      sa <code>&lt;fieldset&gt;</code>.
      <i>Para tong signboard na nagsasabi kung anong section ka na ng form</i>.
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      8.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">datalist</strong>&gt;</strong
      >
    </h4>
    <li>
      Secret menu sa café.
      <strong
        >It gives an autocomplete feature to your
        <code>&lt;input&gt;</code> elements</strong
      >. Users can start typing, and ito na, mag-suggest na siya ng options
      <strong>based on what they've typed</strong>.
      <i>Magic, di ba?</i>
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      9.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">output</strong>&gt;</strong
      >
    </h4>
    <li>
      Ang scorekeeper ng iyong form.
      <strong
        >This element is used to display the result of a calculation or user
        action</strong
      >.
      <i>Ito ung nagpapakita ng output based sa ginawa ng users sa form mo</i
      >. Parang instant feedback, <strong>fresh from the oven!</strong>
    </li>
  </div>
  <div style="display: flex">
    <h4 style="white-space: nowrap; margin-right: 2rem">
      10.
      <strong
        style="font-family: monospace; font-family: monospace; color: #404754"
        >&lt;<strong style="color: #e06c75">option</strong>&gt;</strong
      >
    </h4>
    <li>
      Siyempre, kung may <code>&lt;select&gt;</code>, may
      <code>&lt;option&gt;</code>.
      <strong
        >These are the individual choices inside your
        <code>&lt;select&gt;</code> menu or your
        <code>&lt;datalist&gt;</code></strong
      >.
      <i
        >Each <code>&lt;option&gt;</code> is one possible choice na puwedeng
        piliin ng users.</i
      >
    </li>
  </div>
</div>

<div style="display: flex; max-width: 50rem; margin: auto; align-items: center">
  <h4 style="white-space: nowrap; margin-right: 2rem">
    11.
    <strong
      style="font-family: monospace; font-family: monospace; color: #404754"
      >&lt;<strong style="color: #e06c75">optgroup</strong>&gt;</strong
    >
  </h4>
  <li>
    Ito <strong>ung divider ng iyong options</strong>. Used to group
    related options within a <code>&lt;select&gt;</code> dropdown,
    <strong>making it easier to navigate</strong>. Parang chapters sa libro,
    <i>helping you find what you need faster</i>.
  </li>
</div>

<br><br><br>
<br><br><br>

<h2 style="
		display: flex;
		align-items: center;
	    gap: 1rem;
	    max-width: fit-content;
	    margin: auto;
	    border: solid rgba(164, 167, 177, 0.582) 2px;
	    border-radius: 6px;
		padding: 1rem 3rem;
	"
>
  Example
  <strong style="font-family: monospace; font-family: monospace; color: #404754"
    >&lt;<strong style="color: #e06c75">form</strong>&gt;</strong
  >
</h2>

<br>

<form style="max-width: 60rem; margin: auto;">
	<div style="display: flex; justify-content: center; margin-bottom: 1rem;">
		<fieldset>
		    <legend>Personal Information</legend>
		    <label for="name">Pangalan:</label>
		    <input type="text" id="name" name="name" required><br><br>
		    <label for="email">Email:</label>
		    <input type="email" id="email" name="email" required><br><br>
		    <label for="birthdate">Petsa ng Kapanganakan:</label>
		    <input type="date" id="birthdate" name="birthdate" required><br><br>
		</fieldset>
		<fieldset>
		    <legend>Course Details</legend>
		    <label for="course">Pumili ng Kurso:</label>
		    <select id="course" name="course">
		            <option value="watercolor">Portrait Art</option>
		    </select><br><br>
		    <label for="experience">Karanasan sa Art:</label>
		    <textarea id="experience" name="experience" rows="4" cols="20" placeholder="I-share ang iyong art journey..."></textarea>
		</fieldset>
		<fieldset>
		    <legend>Additional Preferences</legend>
		    <label for="favoriteTool">Paboritong Art Tool:</label>
		    <input list="tools" id="favoriteTool" name="favoriteTool">
		    <datalist id="tools">
		        <option value="Brush">
		        <option value="Pencil">
		        <option value="Chisel">
		        <option value="Palette">
		    </datalist><br><br>
		    <label>Need accommodation?</label>
		    <input type="checkbox" id="accommodation" name="accommodation"><br><br>
		    <label for="output">Expected Fee (PHP):</label>
		    <output id="output" name="output" for="course">3000</output><br><br>
		</fieldset>
	</div>
	<button style="width: 100%" type="submit">Submit</button>
</form>

<br><br><br>

<h2 style="
		display: flex;
		align-items: center;
	    gap: 1rem;
	    max-width: fit-content;
	    margin: auto;
	    border: solid rgba(164, 167, 177, 0.582) 2px;
	    border-radius: 6px;
		padding: 1rem 3rem;
	"
>
  HTML &amp; CSS
</h2>

<br>

```html
<form style="max-width: 60rem; margin: auto;">
	<div style="display: flex; justify-content: center; margin-bottom: 1rem;">
		<fieldset>
		    <legend>Personal Information</legend>
		    <label for="name">Pangalan:</label>
		    <input type="text" id="name" name="name" required><br><br>
		    <label for="email">Email:</label>
		    <input type="email" id="email" name="email" required><br><br>
		    <label for="birthdate">Petsa ng Kapanganakan:</label>
		    <input type="date" id="birthdate" name="birthdate" required><br><br>
		</fieldset>

		<fieldset>
		    <legend>Course Details</legend>
		    <label for="course">Pumili ng Kurso:</label>
		    <select id="course" name="course">
		            <option value="watercolor">Portrait Art</option>
		    </select><br><br>
		    <label for="experience">Karanasan sa Art:</label>
		    <textarea id="experience" name="experience" rows="4" cols="20" placeholder="I-share ang iyong art journey..."></textarea>
		</fieldset>

		<fieldset>
		    <legend>Additional Preferences</legend>
		    <label for="favoriteTool">Paboritong Art Tool:</label>
		    <input list="tools" id="favoriteTool" name="favoriteTool">
		    <datalist id="tools">
		        <option value="Brush">
		        <option value="Pencil">
		        <option value="Chisel">
		        <option value="Palette">
		    </datalist><br><br>
		    <label>Need accommodation?</label>
		    <input type="checkbox" id="accommodation" name="accommodation"><br><br>
		    <label for="output">Expected Fee (PHP):</label>
		    <output id="output" name="output" for="course">3000</output><br><br>
		</fieldset>
	</div>

	<button style="width: 100%" type="submit">Submit</button>
</form>
```