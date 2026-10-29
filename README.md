# Academic website

A single-page academic site (About, Research, Publications & talks, Teaching & Supervision, Hobbies, Contact) that runs on GitHub Pages with no build step.

## Put it online with GitHub Pages

1. Create a GitHub account if you don't have one.
2. Create a new **public** repository named exactly `YOUR-USERNAME.github.io`
   (e.g. if your username is `jdoe`, name it `jdoe.github.io`).
3. Upload the contents of this folder (`index.html`, `README.md`, `.nojekyll`, and the `img/` and `files/` folders) to the repository:
   *Add file → Upload files*, drag them in, then *Commit changes*.
4. Go to *Settings → Pages*. Under "Build and deployment", choose *Deploy from a branch*, branch `main`, folder `/ (root)`, and save.
5. After a minute or two your site is live at `https://YOUR-USERNAME.github.io`.

## Edit your content

Open `index.html` and edit the block marked **EDIT YOUR CONTENT HERE** near the top. Everything on the page — name, bio, projects, publications, talks, links — comes from there. You can edit it directly on GitHub (click the file, then the pencil icon); the site updates automatically after you commit.

- **Photo:** upload a square image as `img/photo.jpg`. Until then, your initials are shown.
- **CV:** upload your CV as `files/CV.pdf`, or set `cv: ""` to hide the button.
- **Publications:** add one entry per paper. Set `selected: true` on the ones shown under "Selected"; "All" shows every paper. "Major contributions" automatically lists papers where your name (`highlightAuthor`) is among the first three authors, so write at least the first three authors in `authors` (add `major: true/false` to override). A `status` such as "submitted" adds a small badge.
- **Talks:** add one entry per talk in `talks` (newest first) with `when`, `title`, `event`, `place` and `kind` ("invited", "seminar" or "contributed"). Set `selected: true` on the ones shown under "Selected talks". Add `links: { Recording: "https://..." }` to link a recording or slides.
- **Project images:** put pictures in `img/` and set `image: "img/your-picture.jpg"` on a research project. Add `credit: "..."` for an image credit, and `link` plus `linkLabel` for the link shown under the card.
- **Hobbies:** each has an emoji `icon`, a `title` and a short `text`; add `image: "img/hiking.jpg"` to show a photo instead of the emoji.
- **Background video:** the faint DESI flythrough behind the page plays from YouTube on computers (`youtube`: the video id), from `img/bg-mobile.*` on phones, and shows `img/bg-poster.jpg` as a still frame for visitors who prefer reduced motion. Set `backgroundVideo: null` to turn it off.
- **Hide something:** use `""` for a field or `[]` for a list (e.g. `talks: []` hides the Talks column).

## Custom domain (optional)

If you own a domain like `yourname.com`, add it under *Settings → Pages → Custom domain* and follow GitHub's DNS instructions.
