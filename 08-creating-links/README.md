# In this article 📖

  - What is a hyperlink?
  - Anatomy of a link
  - A quick primer on URLs and paths
  - Link best practices
  - Creating a navigation menu
  - Email links
  - Test your skills\!
  - Summary

-----

# Prerequisites 📝

  - **Basic HTML familiarity**, as covered in Basic HTML Syntax.
  - **Text-level semantics** such as headings and paragraphs and lists.

-----

# Learning outcomes ✅

  - Understand why links are the fundamental feature of the web. There is no web without links.
  - The **`href` attribute**.
  - **Absolute and relative paths**, and when to use them.
  - Path syntax in detail — slashes, single dot, and double dot.
  - Link states and why they are important — `:hover`, `:focus`, `:visited`, and `:active`.
  - **Inline and block-level links**.
  - Understanding the benefits of writing good link text, such as better accessibility for screen reader users, and potential positive SEO effects.

-----

# What is a hyperlink? 🌐

  - Hyperlinks are one of the most exciting innovations the Web has to offer. They've been a feature of the Web since the beginning, and are what makes the Web a web.
  - Hyperlinks allow us to link documents to other documents or resources, link to specific parts of documents, or make apps available at a web address.
  - Almost any web content can be converted to a link so that when clicked or otherwise activated the web browser goes to another web address (URL).

-----

# Anatomy of a link 🔗

  - A basic link is created by wrapping the text or other content inside an **`<a>`** element and using the **`href`** attribute, also known as a Hypertext Reference, or target, that contains the web address.

**Example:**

```html
<p> I'm creating a link to <a href="https://www.mozilla.org/en-US/">the Mozilla homepage</a>. </p>
```

## Block level links

  - Almost any content can be made into a link, even block-level elements.
  - Wrap a heading element in an anchor (`<a>`) element to make it a link.

**Example:**

```html
<a href="https://developer.mozilla.org/en-US/"> <h1>MDN Web Docs</h1> </a>
```

## Image links 🖼️

  - To turn an image into a link, wrap the **`<img>`** element with an **`<a>`** element.

**Example:**

```html
<a href="https://developer.mozilla.org/en-US/"> <img src="mdn_logo.svg" alt="MDN Web Docs" /> </a>
```

## Adding supporting information with the `title` attribute

  - The **`title`** attribute contains additional information about the link, such as the kind of information the page contains or things to be aware of on the website.
  - **Note:** A link title is only revealed on mouse hover, which means it may not be accessible to all users.

**Example:**

```html
<p> I'm creating a link to <a href="https://www.mozilla.org/en-US/" title="The best place to find more information about Mozilla's mission and how to contribute"> the Mozilla homepage</a>. </p>
```

-----

# A quick primer on URLs and paths 🗺️

  - A **URL**, or Uniform Resource Locator, is a string of text that defines where something is located on the Web.
  - **Paths** specify where the file you're interested in is located in the filesystem.

## Linking in the same directory

  - If the file is in the same directory, you can just specify the filename.

**Example:**

```html
<p> Want to contact a specific staff member? Find details on our <a href="contacts.html">contacts page</a>. </p>
```

## Linking to subdirectories

  - To go down into a subdirectory, specify the directory name, a forward slash, then the filename.

**Example:**

```html
<p>Visit my <a href="projects/index.html">project homepage</a>.</p>
```

## Linking to parent directories

  - To go up a directory level, use two dots (`..`).

**Example:**

```html
<p>A link to my <a href="../pdfs/project-brief.pdf">project brief</a>.</p>
```

## Document fragments

  - You can link to a specific part of an HTML document by using an **`id`** attribute on the target element and referencing it with a hash symbol (`#`) in the link's `href`.

**Example:**

```html
<h2 id="Mailing_address">Mailing address</h2>
<p> Want to write us a letter? Use our <a href="contacts.html#Mailing_address">mailing address</a>. </p>
```

## Absolute versus relative URLs

  - **Absolute URL:** Points to a location defined by its absolute location on the web, including protocol and domain name (e.g., `https://www.example.com/projects/index.html`).
  - **Relative URL:** Points to a location that is relative to the file you are linking from (e.g., `project-brief.pdf`).

-----

# Link best practices ✨

## Use clear link wording

  - Descriptive link text is crucial for screen reader users, search engines, and visual readers.
  - **Good link text:** `Download Firefox`
  - **Bad link text:** `Click here to download Firefox`
  - **Tips:**
      - Don't repeat the URL as link text.
      - Don't say "link" or "links to".
      - Keep link text as short as possible.
      - Avoid linking the same text to different places.

## Linking to non-HTML resources — leave clear signposts

  - Add clear wording to the link text when linking to resources that won't open in the current page (e.g., downloads, streaming videos, popups).

**Example:**

```html
<p> <a href="/large-report.pdf" download> Download the sales report (PDF, 10MB) </a> </p>
```

## Use the `download` attribute when linking to a download

  - Use the **`download`** attribute to provide a default filename for a downloaded resource.

**Example:**

```html
<a href="https://download.mozilla.org/?product=firefox-latest-ssl&os=win64&lang=en-US" download="firefox-latest-64bit-installer.exe"> Download Latest Firefox for Windows (64-bit) (English, US) </a>
```

## When to open links in a new tab 🚪

  - By default, links open in the same tab. To open a link in a new tab, use `target="_blank"`.
  - This can be useful for external links but can also be disorienting for some users.
  - Provide a visual cue, such as an icon, for links that open in new tabs.

-----

# Creating a navigation menu 📄

  - A navigation menu is typically an unordered list (`<ul>`) of links that is consistent across all pages of a website.
  - Remove the link to the current page to provide a visual reminder of the user's location.

-----

# Email links 📧

  - Create links that open a new email message using the `mailto:` URL scheme in the `href` attribute.
  - The email address is optional.

**Basic Example:**

```html
<a href="mailto:nowhere@mozilla.org">Send email to nowhere</a>
```

## Specifying details

  - You can add other email header fields like `subject`, `cc`, and `body` as query terms in the `mailto:` URL.
  - Use a question mark (`?`) to separate the URL from the fields and ampersands (`&`) to separate each field.

**Detailed Example:**

```html
<a href="mailto:nowhere@mozilla.org?cc=name2@rapidtables.com&bcc=name3@rapidtables.com&subject=The%20subject%20of%20the%20email&body=The%20body%20of%20the%20email"> Send mail with cc, bcc, subject and body </a>
```