# The Rough Book Cases

My resume, as five cases I've already solved. Follow along, look at the evidence, and guess what I did. Live at [resume.sjaykh.in](https://resume.sjaykh.in).

There's also a rainy-night apartment you can walk around in 3D, and a boring version: the plain one-page resume.

## Why

I always wanted to be a detective. I love patterns, psychology and working things out. Maybe it comes from my late grandfather, who I'm told was a kickass officer in the CID. My approach to product management is much the same, so this is my resume as a set of cases.

## How it plays

Each case has four steps: the case, the evidence (examine at least two pieces), your call (pick what you think I did; a wrong guess gets a hint), and what I actually did. Every step has one main button, and you can jump between cases from the top of each one. After three cases, the final question unlocks.

Progress is saved in your browser. Number keys pick options, and Escape goes back to all cases. Sound is off until you turn it on.

## What's inside

- `index.html`: the whole site. HTML, CSS and JavaScript in one file.
- `audio/`: rain, thunder and page sounds, loaded only when sound is turned on.
- `sanjay-krishna-resume.pdf`: the resume behind the "Download the PDF" button.
- `CNAME`: points GitHub Pages at resume.sjaykh.in.

## Run it locally

Serve the folder (the sounds need http, not a file:// path):

```sh
python3 -m http.server 8000
```

## Settings

To show an email or LinkedIn link, fill in `CONTACT` near the top of the script in `index.html`:

```js
const CONTACT = { email: "", linkedin: "" };
```

## Credits

- Soft rain by barkenov ([Freesound](https://freesound.org/people/barkenov/sounds/640655/)), CC0.
- Heavy Rain by D W ([Freesound](https://freesound.org/people/D%20W/sounds/136971/)), CC BY. Trimmed and re-encoded.
- Thunderstorm by RHumphries ([Freesound](https://freesound.org/people/RHumphries/sounds/2523/)), CC BY. Three thunder rolls cut out and re-encoded.
- Page flip, book open and thud from Kenney's RPG Audio pack ([kenney.nl](https://kenney.nl)), CC0.
- [Three.js r128](https://threejs.org/) from cdnjs for the apartment.
- Fonts from Google Fonts: Gloock, Newsreader, Archivo Narrow, Cutive Mono, Nanum Pen Script and VT323.

The cases are dramatised from real work and the dialogue is invented. What actually happened is real.
