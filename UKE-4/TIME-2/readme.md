# video & media tag attributter
```
- src	    Path to the video file
- controls	Shows play/pause/volume controls
- autoplay	Starts automatically (usually muted)
- loop	    Repeats the video
- muted	    Starts muted
- poster	Image shown before playback
- preload	How much data loads (none, metadata, auto)
```

# VIDEO
<video controls>
  <source src="video.mp4" type="video/mp4">
  <source src="video.webm" type="video/webm">
  Your browser does not support video.
</video>

# SOURCE
Når du bruker source tag så vil nettleseren sjekke hver source om nettleseren støtter dette formatet, helt til den finner en den støtter. Da vil den laste ned filen og du slipper unødvendig bruk av bandwith og tid.

Med <source type="video/mp4"> så vil nettleseren:
- Vite formatet på filen FØR den laster den ned
- Unngå å laste ned video/audio filer som den ikke støtter
- Spare bånnbredde og tid. (bandwith)

Du kan ha så mange eller så få source tags du vil inni audio eller video, og det lar deg ha en "fallback" som betyr at du har flere alternaiver, skulle en feile. Rett og slett et sikkerhetsnett.

Unngår du å bruke source taggen og heller bruker src attributten. E.g:
<video src="...">
<audio src="...">

Så vil den kunne feile, ikke ha noen fallback og laste ned filer den ikke støtter helt unødvendig.