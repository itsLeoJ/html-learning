## HTML Lists 📝

-----

Lists are used to group related items. HTML offers three types: **unordered**, **ordered**, and **description** lists.

### 📋 Unordered Lists

-----

Used when the **order of items does not matter**, like a shopping list.

  * **Wrapper Element:** `<ul>` (Unordered List)
  * **Item Element:** `<li>` (List Item)

**Example:** A grocery list.

```html
<ul>
  <li>milk</li>
  <li>eggs</li>
  <li>bread</li>
  <li>hummus</li>
</ul>
```

### 🔢 Ordered Lists

-----

Used when the **order of items is important**, like a set of instructions or steps.

  * **Wrapper Element:** `<ol>` (Ordered List)
  * **Item Element:** `<li>` (List Item)

**Example:** Driving directions.

```html
<ol>
  <li>Drive to the end of the road</li>
  <li>Turn right</li>
  <li>Go straight across the first two roundabouts</li>
  <li>Turn left at the third roundabout</li>
</ol>
```

### nesting lists

-----

You can place a list inside another list item (`<li>`) to create sub-lists or nested structures. This is great for showing hierarchical relationships.

**Example:** Adding choices to a step in a recipe.

```html
<ol>
  <li>Add all the ingredients into a food processor.</li>
  <li>
    Process all the ingredients into a paste.
    <ul>
      <li>For a coarse "chunky" hummus, process for a short time.</li>
      <li>For a smooth hummus, process for a longer time.</li>
    </ul>
  </li>
</ol>
```

### 📖 Description Lists

-----

Used for a series of **terms and their corresponding descriptions**, like a glossary or dictionary entries.

  * **Wrapper Element:** `<dl>` (Description List)
  * **Term Element:** `<dt>` (Description Term)
  * **Description Element:** `<dd>` (Description Definition)

**Key Point:** A single term (`<dt>`) can have multiple descriptions (`<dd>`).

**Example:** Defining terms.

```html
<dl>
  <dt>soliloquy</dt>
  <dd>
    In drama, where a character speaks to themselves, representing their inner thoughts.
  </dd>
  <dt>Coffee</dt>
  <dd>The drink that gets the world running in the morning.</dd>
  <dd>A light brown color.</dd>
</dl>
```