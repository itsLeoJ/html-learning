## Test your skills: Audio and video

### 🛠️ **Task 1: Embedding an Audio File**

-----

The goal is to embed an audio file named `audio.mp3` and add controls and fallback text.

  - **Audio file path:** `https://github.com/mdn/learning-area/raw/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/audio.mp3`
  - **Required attributes:**
      - `controls` to display default playback controls.
      - `src` attribute with the audio file path.
  - **Fallback text:** A `<p>` element explaining the browser doesn't support HTML audio, with a link to download the track.

**Resulting HTML snippet:**

```html
<h1>Basic audio embed</h1>

<audio controls src="https://github.com/mdn/learning-area/raw/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/audio.mp3">
  <p>
    Your browser doesn't support HTML audio.
    <a href="https://github.com/mdn/learning-area/raw/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/audio.mp3">Download the track here</a>
    instead.
  </p>
</audio>
```

### 🎬 **Task 2: Embedding a Video Player**

-----

The goal is to create a more complex video player with multiple sources, subtitles, and other features.

  - **Video file paths:**
      - `https://github.com/mdn/learning-area/raw/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/video.mp4`
      - `https://github.com/mdn/learning-area/raw/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/video.webm`
  - **Subtitle file path:** `https://raw.githubusercontent.com/mdn/learning-area/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/subtitles_en.vtt`
  - **Required attributes:**
      - `controls` to display default playback controls.
      - `width` and `height` set to `320` and `240` respectively.
      - `muted` to mute the video by default.
  - **Required elements:**
      - Multiple `<source>` elements for different video formats, each with `src` and `type` attributes.
      - A `<track>` element for subtitles, with `kind`, `src`, `srclang`, and `label` attributes.
      - Fallback text for browsers that don't support HTML video.

**Resulting HTML snippet:**

```html
<h1>Video embed</h1>

<video controls width="320" height="240" muted>
  <source src="https://github.com/mdn/learning-area/raw/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/video.mp4" type="video/mp4" />
  <source src="https://github.com/mdn/learning-area/raw/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/video.webm" type="video/webm" />
  <track kind="subtitles" src="https://raw.githubusercontent.com/mdn/learning-area/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/subtitles_en.vtt" srclang="en" label="English" />
  <p>
    Your browser doesn't support HTML video.
    <a href="https://github.com/mdn/learning-area/raw/refs/heads/main/html/multimedia-and-embedding/tasks/media-embed/media/video.mp4">
      Download the track here
    </a>
    instead.
  </p>
</video>
```