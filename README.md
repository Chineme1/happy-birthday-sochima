# Happy Birthday, Sochima

A single-page birthday site. No build step, no dependencies, nothing to install. Two things inside:

```
index.html   the whole site (HTML, CSS, and JS in one file)
photos/      19 cleaned and compressed photos
```

## Put it online with GitHub Pages (free, ~3 minutes)

1. Go to https://github.com/new and create a repository. Name it something like `happy-birthday-sochima`. Set it to **Public** (Pages on free accounts needs a public repo). Don't tick any of the "initialize" boxes.
2. On the empty repo page, click **uploading an existing file**. Drag in `index.html` and the whole `photos` folder together, then click **Commit changes**.
3. In the repo, open **Settings → Pages**. Under *Build and deployment*, set Source to **Deploy from a branch**, pick **main** and **/ (root)**, then **Save**.
4. Wait a minute, then refresh the Pages settings page. Your link will look like:

   `https://YOUR-USERNAME.github.io/happy-birthday-sochima/`

Send her that link. Any change you push later goes live automatically.

Netlify Drop (https://app.netlify.com/drop) also works: drag the folder onto the page and you get a link instantly.

## Things you'll probably want to edit

Open `index.html` and find the block that starts with `EDIT ME`. Everything personal is there in plain text:

- **`birthYear`** — currently `null`. Fill it in (e.g. `1996`) and the site will say which birthday it is and show her age on the day.
- **`letter`** — the note at the bottom of the page. I wrote a version from the photos; make it yours. The sign-off currently says "your family" so it works from whoever sends it.
- **`ticker`** — the words that scroll across the band under the counter.
- **`chapters`** — the gallery. Each photo has a caption (`cap`). I kept captions to what I could see in the photos, so double-check names of places and fix anything I got wrong. You can reorder photos, move them between chapters, or add new ones by dropping a file in `photos/` and adding a line.
- The Igbo line under the headline (`Ezi ụbọchị ọmụmụ, nwanne m.`) is in the HTML near the top. Change or remove it if you'd prefer.

## What the site does

- **Today (September 12):** "Today is the day" with a live countdown of how many hours of birthday are left, plus a spinning "it's today" sticker on her portrait and a bigger confetti drop on load.
- **Every other day:** counts down to her next birthday in days, hours, minutes and seconds, and counts up how many days it's been since the last one. It works out the year automatically forever, so the link stays alive.
- **Cake:** tap the flames or use the "Blow with your microphone" button and actually blow. When the last candle goes out, confetti. "Light them again" resets it.
- **Photos:** three chapters. Tap any photo for a full-screen viewer with arrow keys and swipe.
- Works on phones, respects reduced-motion settings, keyboard accessible.
