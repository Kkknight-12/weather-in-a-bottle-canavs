# Weather in a Bottle

A cinematic, interactive miniature water cycle. Built with HTML, CSS, Canvas 2D and procedural Web Audio.

## Run locally

No package installation or API keys are required.

```sh
python3 -m http.server 8000
```

Open http://localhost:8000. Any static web server works. For Vercel, import this repository with Framework Preset **Other**, no build command, and the root directory as the output.

## Explore

Scroll through cloud formation, rainfall, runoff and evaporation. Drag horizontally or use the wind slider to influence rain, foliage and water. Sound requires browser permission through a user gesture. Mute, volume, pause and lightning controls are available; reduced-motion preferences start the scene paused with lightning disabled.

Build 3.13 uses layered artwork and image-space deformation rather than a full 3D fluid simulation. Water vapor is invisible; the faint low haze represents condensed mist. This is an artistic simplification, not a meteorological model.

## Credits and provenance

- Created with OpenAI Codex coding assistance.
- Bottle landscape artwork generated for this project with OpenAI image generation.
- Rain and thunder audio are original procedural Web Audio, without external recordings.
- Wave propagation and drop-impulse mathematics adapted from [jquery.ripples](https://github.com/sirxemic/jquery.ripples), Copyright (c) 2017 Pim Schreurs, MIT. The complete applicable notice is in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
- Educational reference: [NOAA, The water cycle](https://www.noaa.gov/education/resource-collections/freshwater/water-cycle).

The third-party MIT notice applies to the identified adapted code; it does not declare a blanket license for all project artwork or original code.

## Validation and limits

Browser checked in Chromium at desktop and phone-sized layouts. Controls, wind response, cloud-only lightning, pause, sound activation/mute, softer rain-linked pond impacts and local foliage motion were checked. Independent simulation tests covered normal/reduced motion and audio state handling. Physical iPhone/Safari testing and speaker audition remain outstanding. Generated imagery and image-space motion can reveal raster artifacts at extreme zoom.

No backend, accounts, location access or live weather data. Only the local mute preference is stored.
