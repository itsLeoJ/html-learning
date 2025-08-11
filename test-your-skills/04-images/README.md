## 📋 Test Your Skills: HTML Images

-----

The aim of this skill test is to help you assess whether you understand images and how to embed them in HTML.

### Task 1: Embedding an Image 🖼️

-----

  - **Goal:** Embed an image of blueberries into the page.
  - **Steps:**
    1.  Add the path to the image using the appropriate attribute.
    2.  Add alternative text to describe the image for screen readers.
    3.  Set an appropriate width to maintain the correct aspect ratio.
  - **Image Details:**
      - **Path:** `https://github.com/mdn/learning-area/blob/main/html/multimedia-and-embedding/tasks/images/images/blueberries.jpg?raw=true`
      - **Alt text:** "A pile of small blue berries"
      - **Intrinsic size:** 615 x 419 pixels
      - **Recommended width:** 400 pixels
  - **Solution (Finished HTML):**
    ```html
    <h1>Basic image embed</h1>
    <img src="https://github.com/mdn/learning-area/blob/main/html/multimedia-and-embedding/tasks/images/images/blueberries.jpg?raw=true" alt="A pile of small blue berries" width="400" />
    ```

### Task 2: Adding a Tooltip 💬

-----

  - **Goal:** Add a tooltip that appears when the image is moused over.
  - **Steps:**
    1.  Add an appropriate attribute with tooltip information.
  - **Image Details:**
      - **Path:** `https://github.com/mdn/learning-area/blob/main/html/multimedia-and-embedding/tasks/images/larch.jpg?raw=true`
      - **Alt text:** "Several tall evergreen trees called larches"
      - **Tooltip text:** "And now, Number 1, The Larch"
  - **Solution (Finished HTML):**
    ```html
    <h1>Basic image title</h1>
    <img src="https://github.com/mdn/learning-area/blob/main/html/multimedia-and-embedding/tasks/images/larch.jpg?raw=true" alt="Several tall evergreen trees called larches" title="And now, Number 1, The Larch" />
    ```

### Task 3: Associating Image with Caption 📝

-----

  - **Goal:** Associate an image with its caption text.
  - **Steps:**
    1.  Use elements to link the image and caption.
  - **Image Details:**
      - **Path:** `https://github.com/mdn/learning-area/blob/main/html/multimedia-and-embedding/tasks/images/firefox.png?raw=true`
      - **Alt text:** "An abstract flaming fox wrapping around a blue sphere"
      - **Dimensions:** `width="446" height="460"`
  - **Caption Text:** "The 2019 Firefox logo"
  - **Solution (Finished HTML):**
    ```html
    <h1>Image and caption</h1>
    <figure>
      <img src="https://github.com/mdn/learning-area/blob/main/html/multimedia-and-embedding/tasks/images/firefox.png?raw=true" alt="An abstract flaming fox wrapping around a blue sphere" width="446" height="460" />
      <figcaption>The 2019 Firefox logo</figcaption>
    </figure>
    ```