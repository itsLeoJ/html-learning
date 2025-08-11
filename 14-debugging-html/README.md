# Debugging HTML 🐛

This article introduces tools and techniques for finding and fixing errors in HTML.

***

## Prerequisites & Learning Outcomes 🎯

**Prerequisites:**

* Basic HTML syntax.
* Familiarity with text-level and structural HTML.

**Learning Outcomes:**

* Understand key concepts of HTML debugging.
* Use the **DOM inspector** in browser DevTools.
* Identify common HTML error types.
* Use the **HTML validator** to find errors.

***

## What are the two types of errors? 🤔

1.  **Syntax errors:** Typos that prevent code from running.
2.  **Logic errors:** Code runs, but not as intended.

HTML is parsed **permissively** by browsers, which means it attempts to display the page even with errors. This is both good and bad: the page will always load, but the browser's corrections might not be what you intended.

***

## The DOM Inspector 🔍

Modern browsers include **developer tools (devtools)** with a **DOM inspector** that shows the rendered HTML of a webpage.

**How to Use:**

* Open devtools (usually the first tab).
* Examine the DOM tree structure.
* Expand and collapse nodes to view descendants.
* Hover over nodes to highlight elements on the page.
* The inspector allows you to see how the browser has corrected invalid markup.

***

## Example: Common Errors in Action 🧐

A sample HTML file with deliberate errors demonstrates how browsers handle badly-formed code.

**Source Code Problems:**

* Unclosed `<p>` and `<li>` elements.
* An unclosed `<strong>` tag that makes the rest of the text bold.
* Badly nested elements: `<strong>...<em>...</strong>...</em>`.
* An unclosed attribute value (`href="..."`) that causes the link to disappear.

**Browser Corrections:**

* The browser adds closing tags for paragraphs and list items.
* It closes the unclosed `<strong>` element around each text block.
* It fixes the badly nested elements to be correctly structured.
* The link with the unclosed `href` attribute is deleted entirely.

***

## HTML Validation ✅

The **Markup Validation Service** (or HTML validator) by the W3C is the best tool for checking HTML.

**How to Use:**

1.  Open the Markup Validation Service.
2.  Provide a web address, upload a file, or paste code directly.
3.  Click **Check** to get a report of errors.

**Interpreting Error Messages:**

* Messages include line and column numbers to help locate the error.
* `End tag ... implied...`: An element is open and needs to be closed.
* `Unclosed element ...`: A tag is missing its closing counterpart.
* `... violates nesting rules`: Elements are incorrectly nested.
* `End of file reached...`: A cryptic error often related to an unclosed attribute near the end of the file.

**Pro-Tip:** Fix a few errors at a time and revalidate. Fixing one error can often resolve several other related issues.