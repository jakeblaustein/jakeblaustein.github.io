# Jake Blaustein — Portfolio

A plain HTML/CSS site. No build step: edit a file, save, refresh the browser.

## Files

| File | What it is |
|---|---|
| `index.html` | Home page |
| `about.html` | About page (bio, education, skills, honors, leadership) |
| `projects.html` | Grid of project cards |
| `projects/*.html` | One page per project |
| `resume.html` + `resume.pdf` | Resume page and the PDF it shows |
| `contact.html` | Contact page |
| `styles.css` | All colors, fonts, and layout |
| `images/` | Put photos, CAD renders, and logos here |

## Common edits

**Change text** — open the page in a text editor (VS Code or Notepad), find the words, change them. Only edit the text *between* tags, e.g. `<p>edit this</p>`.

**Add an image** — save it in `images/`, then replace a placeholder:

```html
<!-- before -->
<figure><div class="ph">Image · Drone</div></figure>

<!-- after (project pages are in a subfolder, so use ../images/) -->
<figure><img src="../images/drone.jpg" alt="Finished quadcopter"></figure>
```

Same idea for the portrait on `about.html` (`images/portrait.jpg`, no `../`) and the logo squares on `projects.html`:

```html
<div class="card-logo"><img src="images/superdial-logo.png" alt="SuperDial logo"></div>
```

**Update the resume** — replace `resume.pdf` with the new file, keeping the same name.

**Change colors or fonts** — edit the variables at the top of `styles.css` (e.g. `--accent`).

**Add a project** — copy one file in `projects/`, rename it, edit the text, then copy one `<a class="card">…</a>` block in `projects.html` and point its `href` at the new file.
