# 🎬 Audio and Video on the Web

---

### **Video and Audio Elements**

* The `<video>` and `<audio>` elements are the native HTML solutions for embedding media, replacing older, proprietary plugins like Flash.
* They provide basic controls and can be controlled with JavaScript APIs for more advanced functionality.

### **The `<video>` Element**

* Uses the **`src`** attribute to point to the video file, similar to **`<img>`**.
* The **`controls`** attribute adds the browser's default playback interface (play/pause, volume, etc.).
* Fallback content, placed inside the `<video>` tags, is shown if the browser doesn't support the element.

### **Supporting Multiple Formats**

* Different browsers support different **container formats** (e.g., OGG, MP4, WebM) and **codecs** (e.g., Vorbis, H.264).
* To ensure compatibility, use the `<source>` element within `<video>` or `<audio>` to provide multiple file formats.
* The browser will play the first format it can support.
* Include the **`type`** attribute with the MIME type (**`video/mp4`**, **`video/webm`**) to allow the browser to skip unsupported files without downloading them.

### **Video Attributes**

* **`width`** and **`height`**: Control the video's size while maintaining its aspect ratio.
* **`autoplay`**: Starts playback automatically (use with caution, as it can be annoying for users).
* **`loop`**: Repeats the video once it finishes.
* **`muted`**: Plays the video with the sound off by default.
* **`poster`**: Displays an image before the video starts playing.
* **`preload`**: Buffers the file; values include **`"none"`**, **`"auto"`**, or **`"metadata"`**.

### **The `<audio>` Element**

* Works similarly to `<video>` but without a visual component.
* It supports **`controls`**, **`autoplay`**, **`loop`**, **`muted`**, and **`preload`**.
* It does **not** support **`width`**, **`height`**, or **`poster`**.

### **Adding Text Tracks**

* Use the `<track>` element and the **WebVTT** file format to provide subtitles, captions, or descriptions.
* Text tracks are essential for accessibility, noisy environments, and non-native speakers.
* The `<track>` element goes inside `<video>` or `<audio>` after the `<source>` elements.
* Key attributes for `<track>`:
    * **`kind`**: Specifies the type of cue (**`"subtitles"`**, **`"captions"`**, **`"descriptions"`**).
    * **`src`**: The URL of the WebVTT file.
    * **`srclang`**: The language of the track (e.g., **`"es"`** for Spanish).
    * **`label`**: A user-friendly name for the track.