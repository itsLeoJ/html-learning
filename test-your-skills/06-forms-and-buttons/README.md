# Test Your Skills: Forms and Buttons 📝

-----

This is a skill test to assess your understanding of how HTML forms and buttons work.

## Forms and Buttons 1 🧑‍💻

-----

**Task:** Create two `<input>` elements for user ID and password, and a submit button.

**Instructions:**

  * Create appropriate inputs for user ID and password, and associate them with their text labels.
  * Create a submit button inside the remaining list item with the text "Log in".

**Solution:**

```html
<form>
  <ul>
    <li>
      <label for="uid">User ID</label>
      <input type="text" id="uid" name="uid" />
    </li>
    <li>
      <label for="pwd">Password</label>
      <input type="password" id="pwd" name="pwd" />
    </li>
    <li>
      <button>Log in</button>
    </li>
  </ul>
</form>
```

## Forms and Buttons 2 🦄

-----

**Task:** Create working sets of checkboxes and radio buttons.

**Instructions:**

  * Turn the first `<fieldset>` contents into a set of radio buttons for pony characters.
  * Make sure only one pony can be selected at a time, and the first one is selected on page load.
  * Turn the second `<fieldset>` content into a set of checkboxes for hotdog preferences.
  * Add two more hotdog choices.

**Solution:**

```html
<form>
  <fieldset>
    <legend>Who is your favorite pony?</legend>
    <ul>
      <li>
        <label for="pinkie">Pinkie Pie</label>
        <input type="radio" id="pinkie" name="pony" value="pinkie" checked />
      </li>
      <li>
        <label for="rainbow">Rainbow Dash</label>
        <input type="radio" id="rainbow" name="pony" value="rainbow" />
      </li>
      <li>
        <label for="twilight">Twilight Sparkle</label>
        <input type="radio" id="twilight" name="pony" value="twilight" />
      </li>
    </ul>
  </fieldset>
  <fieldset>
    <legend>Hotdog preferences</legend>
    <ul>
      <li>
        <label for="vegan">Vegan</label>
        <input type="checkbox" id="vegan" name="hotdog" value="vegan" />
      </li>
      <li>
        <label for="onions">Onions</label>
        <input type="checkbox" id="onions" name="hotdog" value="onions" />
      </li>
      <li>
        <label for="mustard">Mustard</label>
        <input type="checkbox" id="mustard" name="hotdog" value="mustard" />
      </li>
      <li>
        <label for="ketchup">Ketchup</label>
        <input type="checkbox" id="ketchup" name="hotdog" value="ketchup" />
      </li>
    </ul>
  </fieldset>
  <button>Submit</button>
</form>
```

## Forms and Buttons 3 📝

-----

**Task:** Create inputs for a user to update their email, website, phone number, and favorite color.

**Instructions:**

  * Create appropriate input types for each field.
  * Use `<label>` elements to associate the text labels with their respective form fields.

**Solution:**

```html
<form>
  <h2>Edit your preferences</h2>
  <ul>
    <li>
      <label for="email">Email</label>
      <input type="email" id="email" name="email" />
    </li>
    <li>
      <label for="website">Website</label>
      <input type="url" id="website" name="website" />
    </li>
    <li>
      <label for="phone">Phone number</label>
      <input type="tel" id="phone" name="phone" />
    </li>
    <li>
      <label for="fave-color">Favorite color</label>
      <input type="color" id="fave-color" name="fave-color" />
    </li>
    <li>
      <button>Update preferences</button>
    </li>
  </ul>
</form>
```

## Forms and Buttons 4 🍔

-----

**Task:** Implement a drop-down select menu for a user to pick their favorite food.

**Instructions:**

  * Create a basic `<select>` box structure.
  * Associate it with the "food" label.
  * Split the choices into two subgroups: "mains" and "snacks", using `<optgroup>`.

**Solution:**

```html
<form>
  <ul>
    <li>
      <label for="food">Pick your favorite food:</label>
      <select name="food" id="food">
        <optgroup label="mains">
          <option>Salad</option>
          <option>Curry</option>
          <option>Pizza</option>
          <option>Fajitas</option>
        </optgroup>
        <optgroup label="snacks">
          <option>Biscuits</option>
          <option>Crisps</option>
          <option>Fruit</option>
          <option>Breadsticks</option>
        </optgroup>
      </select>
    </li>
    <li>
      <button>Submit choice</button>
    </li>
  </ul>
</form>
```

## Forms and Buttons 5 ✍️

-----

**Task:** Structure the provided form fields into distinct containers.

**Instructions:**

  * Separate the first two fields and the second two fields into two distinct `<fieldset>` containers.
  * Give each `<fieldset>` a descriptive `<legend>`: "Personal details" and "Comment information".
  * Mark up each text label with `<label>` to semantically associate it with its field.
  * Add `<ul>` and `<li>` elements to structure the label/field pairs.

**Solution:**

```html
<form>
  <fieldset>
    <legend>Personal details</legend>
    <ul>
      <li>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" />
      </li>
      <li>
        <label for="age">Age:</label>
        <input type="number" id="age" name="age" />
      </li>
    </ul>
  </fieldset>
  <fieldset>
    <legend>Comment information</legend>
    <ul>
      <li>
        <label for="comment">Comment:</label>
        <input type="text" id="comment" name="comment" />
      </li>
      <li>
        <label for="email">Email (include if you want a reply):</label>
        <input type="email" id="email" name="email" />
      </li>
    </ul>
  </fieldset>
</form>
```

## Forms and Buttons 6 ✅

-----

**Task:** Add validation features to a simple support query form.

**Instructions:**

  * Make all input fields **mandatory** using the `required` attribute.
  * Change the "Email address" and "Phone number" fields to appropriate input types (`email` and `tel`) for specific validation.
  * Set a required length of 5-20 characters for "User name", a max length of 15 for "Phone number", and a max length of 200 for "Comment".

**Solution:**

```html
<form>
  <h2>Enter your support query</h2>
  <ul>
    <li>
      <label for="uname">User name:</label>
      <input type="text" name="uname" id="uname" required minlength="5" maxlength="20" />
    </li>
    <li>
      <label for="email">Email address:</label>
      <input type="email" name="email" id="email" required />
    </li>
    <li>
      <label for="phone">Phone number:</label>
      <input type="tel" name="phone" id="phone" required maxlength="15" />
    </li>
    <li>
      <label for="comment">Comment:</label>
      <textarea name="comment" id="comment" required maxlength="200"></textarea>
    </li>
    <li>
      <button>Submit comment</button>
    </li>
  </ul>
</form>
```