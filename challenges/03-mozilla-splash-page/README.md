### 🛠️ Challenge: Mozilla Splash Page

***

#### 🎯 Project Brief
The goal is to add media (images and a video) to a pre-existing Mozilla splash page HTML file. The CSS is already done, so you only need to focus on the HTML within the `<body>` element.

***

#### 🎬 Getting Started
* **Source Files:** Download the HTML (`index.html`) and image files from the `mdn-splash-page-start` directory on GitHub.
* **Local Setup:** Save `index.html` and `pattern.png` in a new local directory. Save the images from the `originals` directory in a separate folder, as some will need editing.
* **Online Alternative:** You can also use an online editor like CodePen or JSFiddle.

***

#### 🖼️ Preparing Images
* **Resize:** Use an image editor to create 400px wide versions of `firefox_logo-only_RGB.png`, `firefox-addons.jpg`, and `mozilla-dinosaur-head.png`.
* **Icons:** These resized images, along with `mdn.svg`, will serve as icons for further resources.
* **Header Logo:** The small Firefox logo will also be used in the site's header.
* **Red Panda:** Create a 1200px wide landscape version of `red-panda.jpg` and save it with a new name.
* **Optimization:** Optimize all JPG and PNG images for web use (e.g., using a service like tinypng.com).
* **File Location:** Save all the prepared images in the same directory as `index.html`.

***

#### 🔧 HTML Tasks
* **Add Header Logo:** Insert an `<img>` element with the small Firefox logo inside the `<header>` element.
* **Embed Video:** Embed the YouTube video from `https://www.youtube.com/watch?v=ojcNcvb1olg` inside the `<article>` element. The video should be 400px wide.
* **Add Further Info Images:** In the `<div>` with the class `further-info`, add an `<img>` element to each of the four `<a>` links, matching the correct image to each link.
* **Insert Red Panda:** Insert an `<img>` element displaying the large red panda image inside the `<div>` with the class `red-panda`.

***

#### 💡 Hints & Tips
* You do not need to edit any CSS.
* The provided HTML and styling handle most of the work.
* Use the [W3C Nu HTML Checker](https://validator.w3.org/nu/) to check for HTML errors.
* For the YouTube video, you may need to look up how to embed it online.