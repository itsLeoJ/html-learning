# 📝 Test Your Skills: Advanced HTML Text

-----

This skill test helps you assess your understanding of using lesser-known HTML elements for advanced semantic features.

## 📋 Task 1

-----

Add semantics to the provided HTML by:

  * Turning the second paragraph into a block-level quote and indicating the source is from Accessibility.
  * Marking up "HTML" and "CSS" as acronyms with expansions as tooltips.
  * Using subscript and superscript for chemical formulas and dates.
  * Associating machine-readable dates with the text.

## 🧑‍💻 Finished Example

-----

**HTML:**

```html
<h1>Advanced text semantics</h1>
<p>Let's start with a quote:</p>
<p> HTML, Hypertext Markup Language is by default accessible, if used correctly. </p>
<p>CSS can also be used to make web pages more, or less, accessible.</p>
<p>Chemical Formulae: H2O (Water), C2H6O (Ethanol).</p>
<p> Dates: December 25th 2019 (Christmas Day), November 2nd 2019 (Día de los Muertos). </p>
```

**CSS:**

```css
body { background-color: white; color: #333; font: 1em / 1.4 Helvetica Neue, Helvetica, Arial, sans-serif; padding: 1em; margin: 0; }
h1 { font-size: 2rem; margin: 0; color: purple; }
p { margin: 0.5em 0; }
abbr, time { color: green; }
```

## ✅ Solution

-----

```html
<h1>Advanced text semantics</h1>
<p>Let's start with a quote:</p>
<blockquote cite="https://developer.mozilla.org/en-US/docs/Learn/Accessibility">
  <p>
    <abbr title="HyperText Markup Language">HTML</abbr>, Hypertext Markup Language is by default accessible, if used correctly.
  </p>
</blockquote>
<p>
  <abbr title="Cascading Style Sheets">CSS</abbr>, Cascading Style Sheets, can also be used to make web pages more, or less, accessible.
</p>
<p> Chemical Formulae: H<sub>2</sub>O (Water), C<sub>2</sub>H<sub>6</sub>O (Ethanol). </p>
<p> Dates: <time datetime="2019-12-25">December 25<sup>th</sup> 2019</time> (Christmas Day), <time datetime="2019-11-02">November 2<sup>nd</sup> 2019</time> (Día de los Muertos). </p>
```