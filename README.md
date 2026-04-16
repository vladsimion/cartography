# Cartography & Its Trade-offs

A non-linear history of cartography — 39 maps, 7 eras.

**One file. No API key. No backend. No installs.**

Just upload `index.html` to GitHub Pages and it works.

---

## Deploy in 5 minutes

### 1. Create a GitHub repository

1. Go to [github.com](https://github.com) → log in
2. Click **+** (top right) → **New repository**
3. Name it `cartography` (or anything you like)
4. Set to **Public** ← required for free GitHub Pages
5. Tick **Add a README file**
6. Click **Create repository**

### 2. Upload index.html

1. On your new repository page, click **Add file** → **Upload files**
2. Drag `index.html` into the upload box
3. Click **Commit changes**

### 3. Enable GitHub Pages

1. Go to **Settings** → **Pages** (left sidebar)
2. Under Source, select **Deploy from a branch**
3. Branch: **main** · Folder: **/ (root)**
4. Click **Save**

### 4. Wait ~1 minute, then visit:

```
https://YOUR-USERNAME.github.io/cartography/
```

That's it. Done.

---

## Making changes

**To update text or add maps:**

1. Open `index.html` in any text editor (Notepad, TextEdit, etc.)
2. Find the section you want to edit (see below)
3. Go to your GitHub repository → click `index.html` → click the pencil icon
4. Paste your updated content → click **Commit changes**

GitHub Pages updates within about 1 minute.

### Where to find things in index.html

- **Map descriptions** — search for `const MAP_TEXT =` (near the bottom, in the `<script>` section)
- **Era descriptions** — search for `const ERA_TEXT =`
- **Map data** (gained/sacrificed/axes scores) — search for `const ERAS = [`
- **Adding a new map** — find the right era in `ERAS` and add an entry:

```js
{
  name: "Your Map Name",
  year: "1492",
  region: "Portugal",
  gained: ["First gain", "Second gain", "Third gain"],
  sacrificed: ["First sacrifice", "Second sacrifice", "Third sacrifice"],
  axes: {
    accuracy: 3, usability: 4, navigation: 3,
    symbolism: 2, politics: 5, completeness: 3, richness: 3,
  },
},
```

Then add a description entry in `MAP_TEXT`:
```js
"Your Map Name": `First paragraph.\n\nSecond paragraph.\n\nThird paragraph.`,
```

---

## What's in the app

- **7 eras** from Ancient (6200 BCE) to the Digital age
- **39 maps** — each with gained/sacrificed analysis and 7-axis scoring
- **Radar charts** for every map
- **Axis definitions** — click any axis label to read its full rubric
- **Compare mode** — pick any two maps to see them side by side
- **Pre-written scholarly text** for every era and map — no AI needed

---

## Cost

Free. GitHub Pages is free for public repositories. No API, no backend, no running costs.
