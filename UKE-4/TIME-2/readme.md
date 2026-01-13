```
- src	    Path to the video file
- controls	Shows play/pause/volume controls
- autoplay	Starts automatically (usually muted)
- loop	    Repeats the video
- muted	    Starts muted
- poster	Image shown before playback
- preload	How much data loads (none, metadata, auto)
```

Why <source> exists (the real reason)
🔹 Multiple formats (biggest reason)

Different browsers support different formats.
<video controls>
  <source src="video.mp4" type="video/mp4">
  <source src="video.webm" type="video/webm">
  Your browser does not support video.
</video>

The browser:
Tries the first <source>
If the file type is unsupported it tries the next and plays the first one it understands
You cannot do this with src alone.

With <source type="video/mp4"> the browser:
- Knows the format before downloading
- Skips unsupported files immediately
- Saves bandwidth and time

With only src, the browser may:
- Start downloading
- Fail later


# Video Text Tracks
<track src="subs.vtt" kind="subtitles">