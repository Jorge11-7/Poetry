# Los Amores — A. Donis

This folder contains the poetry collection **Los Amores** by A. Donis.

## Files

| File | Description |
|------|-------------|
| `los_amores.md` | Full collection in Markdown (source of truth) |
| `los_amores.pdf` | PDF version (placeholder — see instructions below) |
| `los_amores.epub` | EPUB version (placeholder — see instructions below) |

---

## How to Generate PDF and EPUB

### Option 1: Pandoc (recommended, free)

Install [Pandoc](https://pandoc.org/installing.html), then from this folder run:

```bash
# Generate PDF (requires LaTeX, e.g. TeX Live or MiKTeX)
pandoc los_amores.md -o los_amores.pdf \
  --pdf-engine=xelatex \
  -V mainfont="Georgia" \
  -V fontsize=12pt \
  -V geometry:margin=1in \
  --metadata title="Los Amores"

# Generate EPUB
pandoc los_amores.md -o los_amores.epub \
  --metadata title="Los Amores" \
  --metadata author="A. Donis"
```

### Option 2: VS Code extension

Install the **Markdown PDF** extension in VS Code, open `los_amores.md`, and use the command palette:  
`Markdown PDF: Export (pdf)`

### Option 3: Online converter

Upload `los_amores.md` to [Pandoc Try](https://pandoc.org/try/) or [CloudConvert](https://cloudconvert.com/md-to-pdf) and download the PDF.

---

## Notes

- The placeholder `.pdf` and `.epub` files are empty. Replace them with the generated files before distributing.
- All text is encoded in **UTF-8**. Ensure your PDF/EPUB generator preserves Spanish accents and special characters.
- For professional print distribution, consider hiring a book designer or using a service like Reedsy or IngramSpark.
