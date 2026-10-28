# The Rough Book Cases

Sanjay Krishna's resume, told as a detective game. Five product cases from five years at Entri, a rainy-night apartment you can walk around in 3D, and the plain case file for anyone who just wants the resume.

## What's inside

- `index.html` is the whole site. HTML, CSS and JavaScript live in one file.
- `sanjay-krishna-resume.pdf` is the resume behind the case file's "Download the PDF" button.

## The game

- **Evidence board.** Five cases, in the order they happened. In each one you follow at least two leads, then make a deduction. His skills (pattern recognition, first principles, user empathy, data rigour, bias to action) speak up in the dialogue.
- **Final deduction.** Unlocks after three cases.
- **The apartment.** A Three.js room: streetlight through the blinds, rain on the glass, lamps on inside. Every object links somewhere on sjaykh.in.
- **Origin and case file.** How it started, and the one-page resume.

Progress is saved in the browser's localStorage. Number keys pick dialogue choices, and Escape goes back to the board.

## Run it locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

## Host it

Any static host works: GitHub Pages, Netlify, Cloudflare Pages, or a subdomain of sjaykh.in. Nothing needs building.

## Settings

To show an email or LinkedIn link in the case file and at the end of the game, fill in `CONTACT` near the top of the script in `index.html`:

```js
const CONTACT = { email: "", linkedin: "" };
```

## Built with

- [Three.js r128](https://threejs.org/) from cdnjs, loaded only when the apartment opens. If WebGL isn't available, a flat drawing of the room is shown instead.
- Fonts from Google Fonts: Gloock, Newsreader, Archivo Narrow, Cutive Mono, Nanum Pen Script and VT323.
- Sound is generated in the browser with the Web Audio API and is off by default.

The cases are dramatised from real work and the dialogue is invented. What actually happened, and everything in the case file, is real.
