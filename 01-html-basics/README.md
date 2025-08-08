## 📝 What is HTML?

-----

**HTML (HyperText Markup Language)** is the standard language for creating web pages. It uses a series of **elements** to structure content.

  - **Elements** are used to enclose, or "wrap," different parts of the content to make it appear or act a certain way.
  - **Tags**, like `<p>` for a paragraph, are what create the elements.

For example, to make text a paragraph, you wrap it in paragraph tags:

```html
<p>My cat is very grumpy</p>
```

HTML files are just text documents with a `.html` extension, like `index.html`, which is commonly a website's home page.

> **Note:** HTML tags are **not case-sensitive**, but it's best practice to write them in **lowercase** for consistency and readability.

## 🔬 Anatomy of an HTML element

-----

An element consists of an opening tag, content, and a closing tag.

  - **The opening tag**: `p` - Marks where the element begins.
  - **The content**: `My cat is very grumpy` - The actual text or media inside the element.
  - **The closing tag**: `/p` - Marks where the element ends. It's the same as the opening tag but with a forward slash `/`.

### Nesting elements

You can place elements inside other elements. This is called **nesting**. For correct nesting, inner elements must be closed before outer elements.

  - **Correct ✅:**
    ```html
    <p>My cat is <strong>very</strong> grumpy.</p>
    ```
  - **Incorrect ❌:**
    ```html
    <p>My cat is <strong>very grumpy.</p></strong>
    ```

### Void elements

Some elements, called **void elements**, consist of only a single tag. They are used to insert content like images.

```html
<img src="https://raw.githubusercontent.com/mdn/beginner-html-site/gh-pages/images/firefox-icon.png" alt="Firefox icon" />
```

## 🏷️ Attributes

-----

**Attributes** provide extra information about an element and are always specified in the opening tag.

An attribute should have:

1.  A space between it and the element name.
2.  The attribute name, followed by an `=` sign.
3.  The attribute value, wrapped in quotes (`""` or `''`).

### Boolean Attributes

**Boolean attributes** don't need a value. Their presence in the tag means their value is `true`. For example, the `disabled` attribute on an input field.

```html
<input type="text" disabled />

<input type="text" />
```

### Quotes in Attributes

While sometimes optional, it's best to **always use quotes** around attribute values to avoid browser errors. You can use single or double quotes, but don't mix them for the same attribute.

  - **Good ✅:** `<a href="https://www.example.com">A link.</a>`
  - **Good ✅:** `<a href='https://www.example.com'>A link.</a>`
  - **Bad ❌:** `<a href="https://www.example.com'>A link.</a>`

To use quotes within an attribute value, use the opposite type of quote or a character reference.

  - **Using opposite quotes:**
    ```html
    <a href="https://www.example.com" title="Isn't this fun?">A link.</a>
    ```
  - **Using character references:**
    ```html
    <a href="https://www.example.com" title="An &quot;interesting&quot; reference">A link.</a>
    ```

## 📄 Anatomy of an HTML document

-----

Individual elements combine to form a full HTML page. Here is a basic template:

```html
<!doctype html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <title>My test page</title>
  </head>
  <body>
    <p>This is my page</p>
  </body>
</html>
```

  - **`<!doctype html>`**: The doctype declaration. It's a historical artifact that ensures the browser renders the page correctly.
  - **`<html>`**: The root element that wraps all the content on the page.
  - **`<head>`**: A container for metadata that isn't displayed on the page itself, like the page title, character set, and CSS styles.
  - **`<meta charset="utf-8">`**: Specifies the document's character encoding as UTF-8, which can handle most characters from any human language.
  - **`<title>`**: Sets the title of the page, which appears in the browser tab.
  - **`<body>`**: Contains all the content that you want to display on the page, like text, images, and videos.

## 💨 Whitespace in HTML

-----

No matter how much whitespace (spaces, tabs, new lines) you use in your HTML source code, the browser will reduce it to a single space when displaying the page.

```html
<p>Dogs are silly.</p>

<p>
  Dogs
    are
  silly.
</p>
```

Both paragraphs above will look identical in the browser. However, using whitespace properly in your code improves **readability**.

## ✨ Character references: including special characters in HTML

-----

To display characters that have special meaning in HTML (like `<` or `>`), you need to use **character references**. These start with an ampersand (`&`) and end with a semicolon (`;`).

| Character | Reference |
| :---: | :---: |
| `<` | `&lt;` |
| `>` | `&gt;` |
| `"` | `&quot;` |
| `'` | `&apos;` |
| `&` | `&amp;` |

For example, to display `<p>` as text:

```html
<p>In HTML, you define a paragraph using the &lt;p&gt; element.</p>
```

> **Note:** For most other symbols, you don't need references as long as your character encoding is set to UTF-8.

## 🤫 HTML comments

-----

You can add comments to your HTML code that are ignored by the browser. Comments are useful for leaving notes for yourself or other developers. They start with \`\`.

```html
<p>I'm not inside a comment.</p>

```

In the example above, only the first paragraph will be visible on the web page.

## ✅ Summary

-----

  - HTML provides the **structure** for web content using elements and tags.
  - Elements can be **nested** inside one another and can have **attributes** for extra information.
  - A typical HTML document has a `<!doctype>`, `<html>`, `<head>`, and `<body>`.
  - Use **character references** for special characters and **comments** to explain your code.
  - While HTML structures the page, **CSS (Cascading Style Sheets)** is used to style it (colors, fonts, layout).