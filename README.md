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

## Creator and project links

Built by **Mayank Sarasiya**. These links are visible above the scene on desktop and mobile:

- [DevProjects](https://dev-projects-hq.vercel.app/)
- [Portfolio](https://mayank-portfolio-seven.vercel.app/)
- [GitHub profile](https://github.com/Kkknight-12)
- [Public Weather source](https://github.com/Kkknight-12/weather-in-a-bottle-canavs)

Build 3.14 adds this compact creator strip and a keyboard-accessible Credits & references disclosure. It stays above the animation, keeps the existing scroll timeline, and leaves motion, wind, lightning and sound settings unchanged. The full credits panel scrolls independently on smaller screens. On phones, opening Credits or Effects closes the other disclosure so both remain readable; weather settings are retained.

## Credits and provenance

- Created with OpenAI Codex coding assistance.
- Bottle landscape artwork generated for this project with OpenAI image generation.
- Rain and thunder audio are original procedural Web Audio, without external recordings.
- Wave propagation and drop-impulse mathematics adapted from [jquery.ripples](https://github.com/sirxemic/jquery.ripples), Copyright (c) 2017 Pim Schreurs, MIT. The complete applicable notice is in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
### Research and further reading

These links are separate from the adapted jquery.ripples code. Their libraries and demos are not bundled:

- [Evan Wallace, WebGL Water](https://github.com/evanw/webgl-water): water-rendering reference.
- [three.js Water](https://github.com/mrdoob/three.js/blob/dev/examples/jsm/objects/Water.js): water-rendering reference.
- [weather-animations](https://github.com/g3sthousen/weather-animations): Canvas weather-effects reference and further reading.
- [NOAA, The water cycle](https://www.noaa.gov/education/resource-collections/freshwater/water-cycle): educational science reference.

The third-party MIT notice applies to the identified adapted code; it does not declare a blanket license for all project artwork or original code.

## Validation and limits

Browser checked in Chromium at desktop and phone-sized layouts. Controls, wind response, cloud-only lightning, pause, sound activation/mute, softer rain-linked pond impacts and local foliage motion were checked. Independent simulation tests covered normal/reduced motion and audio state handling. Physical iPhone/Safari testing and speaker audition remain outstanding. Generated imagery and image-space motion can reveal raster artifacts at extreme zoom.

No backend, accounts, location access or live weather data. Only the local mute preference is stored.
