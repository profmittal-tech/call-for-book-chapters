# Call for Book Chapters

Static website (GitHub Pages) listing calls for chapters in edited books.

## Structure

```
index.html                      ← landing page listing all book calls
assets/css/style.css            ← shared styles
assets/images/                  ← shared images (publisher logos)
books/
  student-innovation-university-outreach/
    index.html                  ← call page for this book
    images/                     ← editor photos
    *-Brochure.pdf              ← downloadable brochure
.nojekyll                       ← tells GitHub Pages to serve files as-is
```

## Adding a new book

1. Copy `books/student-innovation-university-outreach/` to `books/<new-book-slug>/`.
2. Edit the new `index.html` (title, about, chapters, dates, editors, submission link), replace the photos in `images/` and the brochure PDF.
3. In the root `index.html`, copy one `<div class="book-item">` block and link it to the new folder.

## Publish on GitHub Pages

1. Create a public repository `call-for-book-chapters` under the `profmittal-tech` account.
2. Push this folder to it.
3. Repository **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`.
4. The site appears at `https://profmittal-tech.github.io/call-for-book-chapters/`.
