# Nishad Raval — Portfolio

A single-file portfolio site. No build step, no dependencies. Everything is in `index.html`.

## Run locally
Open `index.html` in a browser (or run `npx serve` in this folder).

## Edit your content
Open `index.html` and search for `const CONFIG`. It sits near the top of the `<script>`.

- `resume`: put your PDF in this folder as `resume.pdf`, then set `resume:"resume.pdf"`.
- `links`: add your LinkedIn and GitHub URLs.
- `skills`: each entry is `["Name","Category","Using" or "Learning"]`. Categories: Languages, Database, Tools.
- `projects`: add a new object to the array (copy the SpendSense one). Give it a unique `id`.
  - `cover` and `gallery` take image paths, e.g. `"images/spendsense-cover.jpg"`.
  - `live` and `repo` take full URLs. The buttons only show when these are filled in.

## Deploy
- Vercel / Netlify: import the GitHub repo, no build command, output directory is the root.
- GitHub Pages: repo Settings, Pages, deploy from branch `main`, folder `/ (root)`.
