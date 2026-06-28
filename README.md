# Personal Homepage

An academic-style personal homepage, published with GitHub Pages at
**https://AI4Science2025.github.io**.

## Files

| File | What it is |
|------|------------|
| `index.html` | Home page — bio, education, experience, news, selected publications |
| `publications.html` | Full publications list |
| `assets/style.css` | All styling (colors, fonts, layout) |
| `assets/profile.svg` | Placeholder photo — replace with your own |

## How to edit

Everything is plain HTML + CSS, no build step.

1. **Text & content** → edit `index.html` and `publications.html`.
   Look for `<!-- EDIT ME -->` comments marking the spots to change.
   To add an entry (a job, a paper, a news item), copy one of the existing
   blocks and change the text.
2. **Your photo** → drop a `profile.jpg` (or `.png`) into `assets/`, then
   change `src="assets/profile.svg"` to your file in `index.html`.
3. **Logos** → add small PNGs to `assets/` and point the `entry-logo`
   images at them (or delete the `<img>` tags if you don't want logos).
4. **Colors / fonts** → edit the variables at the top of `assets/style.css`
   (`--accent` is the link color, `--text` the body color, etc.).

## Preview locally

Open `index.html` directly in your browser, or run a tiny server:

```bash
cd my-homepage
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Publish changes

After editing, commit and push:

```bash
git add -A
git commit -m "Update homepage"
git push
```

GitHub Pages rebuilds automatically; the live site updates within ~1 minute.
