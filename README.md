# Call for Book Chapters

Static website (GitHub Pages) listing calls for chapters in edited books.

## Structure

```
index.html                      ← landing page listing all book calls
assets/css/style.css            ← shared styles
assets/js/main.js               ← mobile menu
books/
  student-innovation-university-outreach/
    index.html                  ← call page for this book
.nojekyll                       ← tells GitHub Pages to serve files as-is
```

## Adding a new book

1. Copy `books/student-innovation-university-outreach/` to `books/<new-book-slug>/`.
2. Edit the new `index.html` (title, about, chapters, dates, editors, submission link).
3. In the root `index.html`, copy one `<article class="card book-card">` block and link it to the new folder.

## Publish on GitHub Pages

1. Create a public repository on GitHub (e.g. `Call_BookChapters`).
2. Push this folder to it.
3. Repository **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`.
4. The site appears at `https://<username>.github.io/Call_BookChapters/`.
