# Challenge: Letter markup 📝

---

We all learn to write a letter sooner or later; it is also a useful example to test our text formatting skills. In this challenge, you'll have a letter to mark up as a test for your HTML text formatting skills, as well as hyperlinks and proper use of the HTML `<head>` element.

## Starting Point 🚀

---

- Get the raw text you need to mark up, and the CSS to style the HTML.
- Create a new `.html` file using your text editor or use an online editor such as CodePen or JSFiddle.
- **Note:** If you get stuck, you can reach out to us in one of our communication channels.

## Project Brief 📋

---

- Your task is to mark up a letter that needs to be hosted on a university intranet.
- The letter is a response from a research fellow to a prospective PhD student concerning their application to the university.

### Block/Structural Semantics 🧱

- Use appropriate document structure: `<!DOCTYPE html>`, `<html>`, `<head>`, and `<body>`.
- Mark up the letter as an organization of headings and paragraphs.
- There is one top-level heading ("Re:" line) and three second-level headings.
- Use an appropriate list type to mark up the semester start dates, study subjects, and exotic dances.
- Put the two addresses inside `<address>` elements.
- Each line of the address should be on a new line, but not in a new paragraph.

### Inline Semantics ✒️

- Mark up the names of the sender and receiver (and Tel and Email) with strong importance using `<strong>`.
- The four dates should have appropriate elements containing machine-readable dates.
- The first address and first date should have a `class="sender-column"` attribute.
- Mark up the five acronyms/abbreviations in the main text — "PhD," "HTML," "CSS," "BC," and "Esq." — with `<abbr>`.
- Mark up the six sub/superscripts appropriately (chemical formulae, and 10³ and 10⁴).
- Mark up at least two appropriate words with strong importance/emphasis (`<strong>` or `<em>`).
- Add two hyperlinks (`<a>`) with titles. The URL can be `http://example.com`.
- Mark up the university motto quote and citation with appropriate elements.

### The Head of the Document 📝

- The character set of the document should be set as `utf-8` using the appropriate `<meta>` tag.
- The author should be specified in an appropriate `<meta>` tag.
- The provided CSS should be included inside an appropriate `<link>` tag.

## Hints and Tips 💡

---

- Use the W3C HTML validator to validate your HTML.
- You don't need to know any CSS for this assignment; just put the provided CSS inside an HTML element.

## Example 🖼️

---

- The following screenshot shows an example of what the letter might look like after being marked up.