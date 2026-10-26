# The Lectern

Daily practice for the voice, the words and the room. One app built from The Floor, The Room and The Register, with The Shelf's daily, review and reflection engine, plus two new pillars: the Lexicon (vocabulary by register, each word with the sentence you'd say) and the Lectern (public speaking passages with breath marks, a read timer and a recorder).

Everything is said out loud. Said silently, none of it does anything.

## Publish with GitHub Pages

1. Create a new **public** repository called `the-lectern` on GitHub.
2. **Add file > Upload files** and drag in everything in this folder so `index.html` sits at the top level: `index.html`, the five `content-*.js` files, `manifest.webmanifest`, `sw.js`, the `icons` folder and this README. Commit.
3. **Settings > Pages**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, save.
4. After a minute or two it's live at `https://djsumd.github.io/the-lectern/`.

## Install it on the phone

Open the link in Chrome, three-dot menu, **Install app**. If Chrome's install record is poisoned (the "Could not open app" toast), install it from Samsung Internet instead, which keeps its own install state.

iPhone: open the link in Safari, Share, **Add to Home Screen**, with "Open as web app" on.

The first visit downloads about 2 MB once; after that it opens from the phone, online or not.

## What's in it

- **Today**: one scenario, one spoken line, one word, one held beat, one clean-speech pair, one passage. Done is done; no streaks.
- **Library**: every scenario (The Room's 209 judgment scenarios and The Register's 219 rapport, thread and cut scenarios), every spoken line (The Register's 242 drills, The Floor's 40 directness drills and 46 interventions, plus 448 strong lines lifted from The Room), 120 clean-speech pairs, 141 diction drills, the 91-card Deck, and the warm-up (breath patterns, tongue and lip, resonance, the six-minute routine).
- **Lexicon**: 319 words and phrases by register, each with the sentence to say aloud.
- **Lectern**: 24 passages for concerts, council, parents, staff, the Festival, the bandstand and occasions. Breath marks, stressed words, a read timer against a target length, and a recorder that keeps takes on the phone.
- **Review**: anything marked "Needs work" comes back tomorrow, then at doubling intervals, until it's yours.
- **Journal**: reflections after real meetings, linked to the item they matched. Export as Markdown.
- **Backup**: one JSON file with your reps, review queue and reflections. Recordings stay on the phone and aren't in it.

## Updating

Upload the changed files and commit. Installed copies check for updates whenever they open with a connection and switch to them the time after. Whenever you change any file, also change `VERSION` at the top of `sw.js` (for example `lectern-v2`).

## Adding content

Each `content-*.js` file is plain data. New passages go in `content-lectern.js`, new words in `content-lexicon.js`. Keep the same fields as the entries already there. In a passage, ` | ` is a breath, `||` is a full stop you hold, and `*word*` marks the word to land.
