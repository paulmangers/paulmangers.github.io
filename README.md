# Personal academic page

Plain HTML and CSS. No build step, no dependencies, nothing to install.

## Files

| File | What it's for |
|---|---|
| `index.html` | All your content. This is the only file you need to edit. |
| `style.css` | Layout and colours. Leave alone unless you want to change the look. |
| `photo.jpg` | Add this yourself. Roughly 3:4, at least 440×520 px. |
| `cv.pdf` | Add this yourself if you want the CV link to work. |

## Putting it online

1. Create a repository named `yourusername.github.io` (the name must match your GitHub username exactly).
2. Drop these files in the root of the repository and push.
3. In the repository, go to Settings → Pages and set the source to the `main` branch, folder `/ (root)`.
4. Your page appears at `https://yourusername.github.io` within a minute or two.

To preview locally before pushing, just open `index.html` in a browser. Everything works from the filesystem.

## Editing

Every spot that needs your text is marked with an `EDIT` comment in `index.html`. To add another publication, talk, or course, copy an existing `<li>` block and change the text inside it.

Sections you can delete outright if they don't apply: news, talks, the footer, and any line in the contact list.

## Adjusting the look

Everything visual is at the top of `style.css`:

- `--link` sets the link colour, which is the only accent on the page.
- `--sidebar` sets the width of the left column (currently 200px).
- The `prefers-color-scheme: dark` block sets the dark-mode palette. Delete that whole block if you want the page to stay light for everyone.

The layout collapses to a single column below 640px, and there's a print stylesheet so the page saves to PDF cleanly.
