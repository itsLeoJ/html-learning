# 🖼️ HTML images

In the beginning, the web was just text, but soon the ability to embed images and other content was added. This article explains how to use the `<img>` element, annotate it with captions using `<figure>`, and the difference between HTML and CSS background images.

---

### **Prerequisites & Learning Outcomes** 🧠

* **Prerequisites:** Basic HTML, text-level semantics, headings, paragraphs, and lists.
* **Learning Outcomes:**
    * Understand "replaced elements."
    * Learn basic `<img>` tag syntax.
    * Use `src` for image resources.
    * Use `width` and `height` to prevent UI shifts.
    * Optimize media assets for the web.
    * Understand media asset licensing.

---

# 📝 How to Put an Image on a Webpage

To embed an image, use the `<img>` element. It's a void element, meaning it has no child content or end tag, and requires two main attributes:

* `src`: Contains a URL pointing to the image. Can be relative or absolute.
* `alt`: Provides a textual description of the image.

### **Best Practices** ✅

* Use descriptive filenames for SEO (e.g., `dinosaur.jpg` is better than `img835.png`).
* Host images on your own server and use relative URLs for better maintenance and efficiency.
* **⚠️ Warning:** Do not "hotlink" to images on other websites without permission.

---

# ✍️ Alternative Text (`alt`)

The `alt` attribute provides a textual description for situations where the image can't be seen or displayed.

### **When is `alt` text useful?** 🤔

* For visually impaired users using screen readers.
* When the image file or path is incorrect.
* If the browser doesn't support the image type.
* For text-only browsers.
* To provide context for search engines.
* When users have turned off images to save data.

### **What to write in `alt` text?** 💡

* **Decoration:** Use `alt=""` (a blank `alt` attribute).
* **Content:** Provide a brief description of the image's information.
* **Link:** If an image is a link, the `alt` text must provide accessible link text.
* **Text in images:** If unavoidable, supply the text from the image in the `alt` attribute.

---

# 📏 Width and Height

Use the `width` and `height` attributes to specify the image's dimensions in pixels. This is a crucial practice.

### **Why use `width` and `height`?** 🚀
* When a browser loads HTML, it will start displaying the content immediately.
* If image dimensions are not specified, the browser will have to move surrounding text once the image loads, which is distracting for users.
* Specifying `width` and `height` lets the browser reserve space for the image, preventing content shifts.

### **Important Note** 🚫
* Do not use these attributes to resize images. Use an image editor to set the correct size beforehand.
* Use CSS for resizing if necessary.

---

# 🏷️ Image Titles

The `title` attribute provides additional information that appears as a tooltip on mouse hover.

### **Why `title` is not recommended** ❌
* It has accessibility issues.
* Screen reader support is unpredictable.
* Most browsers only show it on mouse hover, making it inaccessible to keyboard users.
* It's better to include supporting information in the main article text.

---

# 🏛️ Media Assets and Licensing

Images found online are subject to various license types. Always ensure you have permission to use an image.

### **Common License Types** ⚖️
* **All rights reserved:** Exclusive rights to the creator. You must get permission, pay a license fee, or use it under fair use/dealing.
* **Permissive (e.g., MIT, BSD, CC):** Allows use without a fee, but you must fulfill specific conditions such as:
    * Crediting the creator.
    * Linking to the source.
    * Indicating changes made.
* **Public domain/CC0:** "No rights reserved." No copyright applies, and it can be used freely without conditions.

### **How to find permissively-licensed images** 🔍
* Use image search engines with filters for usage rights (e.g., Google Images' "Usage Rights" tool).
* Search image repositories like Flickr, ShutterStock, and Pixabay with their search options.
* Use sites that exclusively distribute permissively-licensed images, such as Picryl and The Noun Project.

---

# 🖼️ Annotating Images with `<figure>` and `<figcaption>`

Use the `<figure>` and `<figcaption>` elements to semantically link an image to its caption.

* `<figure>`: A semantic container for figures.
* `<figcaption>`: Clearly links the caption to the figure's content.

This is more accessible for screen readers than using a `<div>` and `<p>` tag.

---

# 🎨 CSS Background Images

The CSS `background-image` property can also embed images.

* **For decoration only:** CSS background images are purely for aesthetics and have no semantic meaning.
* **Invisible to screen readers:** They cannot have text equivalents.
* **Recommendation:** Use HTML `<img>` for images with meaning or content, and CSS background images for purely decorative purposes.

---

# **Summary** 📖

This article covered the use of HTML `<img>` elements, the importance of `src` and `alt` attributes, specifying `width` and `height` to improve user experience, the roles of `title` and licensing, and using `<figure>` and `<figcaption>` for accessibility. The next article will cover embedding video and audio.