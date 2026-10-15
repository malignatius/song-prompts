# Song Prompts

A cue deck for making music in a DAW. Draw a brief of 1–4 cards, each from a different category: a mode, a rhythm, a sound constraint, a production trick. Lock the cards you like, re-roll the rest, then go make the track.

Inspired by Brian Eno and Peter Schmidt's *Oblique Strategies*, but more concrete and aimed at people working in a DAW.

## Features

- 180+ cues in 16 categories: Mode, Chords & Key, Melody, Tempo, Meter, Rhythm, Dynamics, Sound, Effects, Structure, Limits, Vocals, Genre, Mood, Process and Wildcard
- Lock cards and re-roll the rest, or re-roll a single card
- Random values on some cards: tempo (60–180 BPM), key and time signature
- Turn categories on and off
- Session log of your recent briefs, with copy to clipboard
- Light and dark mode
- Space bar draws a new brief

## Use it

Open `index.html` in a browser, or publish the repository with GitHub Pages and use the link.

No build step and no dependencies. Fonts and icons load from Google Fonts.

## Edit the cues

All cues live in [`prompts.md`](prompts.md):

```markdown
## Rhythm & Groove

- Rhythm: Use a bossa nova rhythm
- Rhythm: Use a reggae one-drop
```

- Each `## Heading` becomes a category.
- Each `- Label: Cue` line becomes a card.
- Any other line is ignored, so you can keep notes in the file.
- `{bpm}`, `{key}` and `{meter}` are replaced with a random value on every draw.

When the page is served from a web server (for example GitHub Pages), it reads `prompts.md` directly. When you open `index.html` straight from your disk, the browser won't let it read the file, so the page uses a built-in copy instead. To use your edited list locally, click **Load .md file** or drop the file onto the page.

## Credits

Made by Pontus Jarenskog, 2026.
