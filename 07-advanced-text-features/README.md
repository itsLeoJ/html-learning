### Advanced Text Features 📝

This article explores HTML elements for defining text semantics, focusing on less common but useful elements beyond basic headings, paragraphs, and lists.

-----

### Prerequisites 🛠️

To understand these concepts, you should have a basic familiarity with:

  * **HTML Syntax**
  * **Text-level semantics** (headings, paragraphs, lists)

-----

### Key Learning Outcomes 🎯

You will learn about marking up:

  * Quotations
  * Abbreviations and acronyms
  * Addresses
  * Times and dates
  * Superscript and subscript

-----

### Quotations 💬

HTML provides two main elements for quotations:

#### Blockquotes

Use the `<blockquote>` element for **block-level content** (paragraphs, lists, etc.) quoted from another source. Include the source URL in a `cite` attribute.

  * **Example:**

<!-- end list -->

```html
<blockquote cite="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/blockquote">
  <p>The HTML <blockquote> Element indicates that the enclosed text is an extended quotation.</p>
</blockquote>
```

#### Inline quotations

Use the `<q>` element for **short, inline quotations** that don't require new paragraphs.

  * **Example:**

<!-- end list -->

```html
<p>The quote element is <q cite="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/q">intended for short quotations that don't require paragraph breaks.</q></p>
```

#### Citations 📚

The `<cite>` element is used to contain the **title of a work** being quoted, not the URL.

  * **Example:**

<!-- end list -->

```html
<p>According to the <cite>MDN blockquote page</cite>...</p>
```

-----

### Abbreviations and Acronyms 🗣️

The `<abbr>` element is used to wrap an abbreviation or acronym.

  * **Best Practice:** On first use, provide the full expansion of the term in plain text. For shortened terms, provide the full expansion in the `title` attribute.
  * **Example:**

<!-- end list -->

```html
<p>We use <abbr>HTML</abbr>, Hypertext Markup Language, to structure our web documents.</p>
<p>The new user interface design <abbr title="Looks good to me">LGTM</abbr>!</p>
```

  * **Note:** The `<acronym>` element is no longer used and should be replaced by `<abbr>`.

-----

### Contact Details ✉️

The `<address>` element is for marking up **contact information** for the nearest `<article>` or `<body>` element.

  * **Example:**

<!-- end list -->

```html
<address>
  <p>Chris Mills<br>Manchester<br>UK</p>
</address>
```

-----

### Superscript and Subscript ⬆️⬇️

  * `<sup>` for **superscript** (e.g., dates, mathematical equations).

  * `<sub>` for **subscript** (e.g., chemical formulas).

  * **Example:**

<!-- end list -->

```html
<p>My birthday is on the 25<sup>th</sup> of May.</p>
<p>Caffeine's chemical formula is C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>.</p>
```

-----

### Representing Computer Code 💻

  * `<code>`: Marks up a generic piece of **computer code**.

  * `<pre>`: Retains **whitespace and formatting** for blocks of code.

  * `<var>`: Marks up **variable names**.

  * `<kbd>`: Marks up **keyboard input**.

  * `<samp>`: Marks up the **output of a program**.

  * **Example:**

<!-- end list -->

```html
<pre><code>const para = document.querySelector('p');</code></pre>
<p>In the example, <var>para</var> represents an element.</p>
<p>Select text with <kbd>Ctrl</kbd> + <kbd>A</kbd>.</p>
```

-----

### Times and Dates ⏳

The `<time>` element marks up times and dates in a **machine-readable format** using the `datetime` attribute.

  * **Example:**

<!-- end list -->

```html
<time datetime="2016-01-20">20 January 2016</time>
<time datetime="19:30">7.30pm</time>
```

-----

### Summary ✅

This article covered several HTML elements for text semantics, including quotations, abbreviations, contact details, superscripts/subscripts, and computer code. These elements are essential for adding more precise meaning to web content.