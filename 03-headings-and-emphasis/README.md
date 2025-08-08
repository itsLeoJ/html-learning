# 📝 HTML: Headings & Paragraphs
---
## 🧱 The Basics
* HTML's primary role is to give text **structure** so browsers can display it correctly.
* **Paragraphs**: Wrap blocks of text in `<p>` tags.
    * `html <p>I am a paragraph, oh yes I am.</p>`
* **Headings**: Use `<h1>` to `<h6>` for titles and subtitles.
    * `html <h1>I am the title of the story.</h1>`

## ιε Building a Hierarchy
---
Headings create a logical structure, with `<h1>` as the main heading, `<h2>` as subheadings, `<h3>` as sub-subheadings, and so on.

### ✅ Best Practices
1.  **One `<h1>` Per Page**: Use a single `<h1>` for the top-level heading.
2.  **Correct Order**: Don't skip levels (e.g., an `<h2>` should not be followed by an `<h4>`).
3.  **Keep it Simple**: Aim for no more than three heading levels per page to keep the document easy to navigate.

## 🤔 Why Structure Matters
---
Without structure, a browser sees text as one large, unreadable chunk. Proper structure provides critical benefits:

* 👀 **Scannability**: Users quickly scan headings to find relevant information.
* 🔍 **SEO**: Search engines use headings to identify important keywords, boosting page rankings.
* ♿ **Accessibility**: Screen readers use headings as signposts, allowing visually impaired users to navigate content efficiently.
* 🎨 **Styling**: Elements are needed to target content with CSS and JavaScript.

## 💪 The Power of Semantics
---
Semantics is about using the correct element for its **meaning and function**, not just for its appearance.

* 👍 **Good (Semantic): `<h1>This is a top level heading</h1>`**
    * This has semantic value. Browsers, search engines, and screen readers understand its role as the main heading.

* 👎 **Bad (Presentational): `<span style="font-size: 32px;">Is this a heading?</span>`**
    * This only *looks* like a heading. A `<span>` has no semantic meaning, so you lose all the SEO and accessibility benefits.


# ✍️ Emphasis and Importance in HTML

-----

### 🎯 Core Concepts & Goals

  * **Prerequisites**: Basic knowledge of HTML syntax.
  * **Learning Outcomes**:
      * Understand semantic elements like `<em>` and `<strong>`.
      * Identify deprecated presentational tags (`<big>`, `<font>`).
      * Learn the new semantic meanings of `<i>` and `<b>`.

-----

### 🗣️ Emphasis: `<em>`

The `<em>` element is used to apply stress emphasis to words, subtly altering the meaning of a sentence.

  * **Effect**: Screen readers may use a different tone of voice.
  * **Default Style**: Renders as *italic* text.
  * **Usage**: Do not use it purely for italic styling.

<!-- end list -->

```html
<p>I am <em>glad</em> you weren't <em>late</em>.</p>
```

-----

### 💪 Strong Importance: `<strong>`

The `<strong>` element marks text that has strong importance, seriousness, or urgency.

  * **Effect**: Screen readers may use a different tone of voice.
  * **Default Style**: Renders as **bold** text.
  * **Usage**: Do not use it purely for bold styling.

<!-- end list -->

```html
<p>This liquid is <strong>highly toxic</strong>.</p>
<p>I am counting on you. <strong>Do not</strong> be late!</p>
```

✨ **Pro-Tip**: You can nest `<em>` and `<strong>` elements.

```html
<p>...if you drink it, <strong>you may <em>die</em></strong>.</p>
```

-----

### ⚠️ Italic, Bold, and Underline: `<i>`, `<b>`, `<u>`

These elements were originally for presentation only. In HTML5, they were given new semantic roles.

> **Best Practice**: Only use `<b>`, `<i>`, or `<u>` when a more suitable semantic element (`<strong>`, `<em>`, `<mark>`) is not available. Always consider accessibility.

  * **`<i>`**: Used for text traditionally conveyed in italics.

      * 📚 Foreign words: `<i lang="fr">soupe à l'oignon</i>`
      * 🔬 Taxonomic designations: `<i>Archilochus colubris</i>`
      * 💡 Technical terms or thoughts.

  * **`<b>`**: Used for text traditionally conveyed in bold, without implying extra importance.

      * 🔑 Keywords: Use the elements based on their \<b\>semantic\</b\> meaning...
      * 🏷️ Product names.

  * **`<u>`**: Used for text traditionally conveyed with an underline.

      * ✍️ Misspellings: `<u class="spelling-error">spel</u>`
      * 📛 Proper names (in some contexts).

> **Warning ❗️**: Users strongly associate underlining with hyperlinks. If you use `<u>`, consider changing its default styling with CSS to avoid confusion.

```html
<p>The Ruby-throated Hummingbird (<i>Archilochus colubris</i>) is the most common hummingbird...</p>

<p>Someday I'll learn how to <u class="spelling-error">spel</u> better.</p>

<dl>
  <dt>Semantic HTML</dt>
  <dd>Use the elements based on their <b>semantic</b> meaning, not their appearance.</dd>
</dl>
```