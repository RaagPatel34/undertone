# Undertone

A browser-based prototype for sampling skin colors and exploring nearby shade references.

## Try it

Upload a photo or use your camera, select 3–5 skin areas, and compare the closest demo shades. The sample palette lets you try the flow without a photo.

## Run locally

No dependencies or build step are needed. From this folder:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000. Camera capture requires HTTPS or localhost and browser permission.

## Features

- Local photo upload and camera snapshot
- Multiple selected-area samples
- CIELAB / Delta E 76 digital shade ranking
- Sample consistency indicator
- Warmth and lightness adjustments
- Downloadable JSON summary

## Privacy and limitations

Photos are processed in the browser and are not uploaded. The current catalog consists of fictional references, not measured cosmetics. Sample consistency is not a calibrated accuracy score. Skin type and finish are self-reported preferences, not inferred from images. Real product recommendations and mixing recipes require measured products, physical testing, and validation across skin tones and capture conditions.

## Public app and private repository

Live app: https://undertone-shade-studio-raag.raagpatel34.chatgpt.site

The GitHub repository is private. The app is hosted separately on Sites and is publicly accessible. GitHub commits do not automatically deploy to Sites. Browser-delivered HTML, CSS, and JavaScript are visible to app visitors even though the repository and its history are private.

## Files

- index.html: interface
- style.css: responsive styling
- app.js: image sampling, matching, and export
