# Maragkakis Lab Website

Built with [Hugo](https://gohugo.io) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

---

## Editing content

All content lives under `content/`. Each section has its own subdirectory.

### People

Files: `content/people/<name>.md`

To add a new person, copy an existing file:

Add the photo as a JPEG or PNG to `static/images/people/`. The filename should match the `image` field in the `<name>.md`. Recommended size: 400×400 px, cropped to a square.

### Publications

Files: `content/publications/<year>-<short-title>.md`

To add a new publication, copy an existing one:

The `link` field is displayed as a "View on PubMed" button at the bottom of the page.

---

## Local preview

**1. Create and activate the Hugo conda environment**

```bash
conda create -n hugo -c conda-forge hugo
conda activate hugo
```

**2. Clone the repo (including the PaperMod submodule)**

```bash
git clone --recurse-submodules <repo-url>
cd <repo-name>
```

**3. Start the local dev server**

```bash
conda run -n hugo hugo server
```

Open [http://localhost:1313](http://localhost:1313). The server hot-reloads on every file save.
