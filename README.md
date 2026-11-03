# Andrew Green — ENC 1102 Portfolio

A static HTML/CSS portfolio designed for GitHub Pages. The pages preserve the existing navy/blue visual style and the content supplied from the Google Sites embeds.

## Files

- `index.html` — portfolio homepage
- `outcome-1.html` — Generating Inquiry
- `outcome-2.html` — Information Literacy
- `style.css` — shared styling
- `assets/pdfs/` — put artifact PDFs here

## Add a PDF

1. Export your assignment as a PDF.
2. Put it in `assets/pdfs/`.
3. Use the filename shown on the matching artifact card, or update the two PDF links in that card to match your filename.
4. Commit and push the change. GitHub Pages will publish it with the site.

Current expected filenames:

- `research-proposal.pdf`
- `google-survey.pdf`
- `annotated-bibliography.pdf`
- `secondary-sources.pdf`

The PDF cards currently contain links but do not embed a preview until the corresponding PDF file exists. To embed a PDF in the page, add this inside the matching `.pdf-card`:

```html
<iframe
  class="pdf-preview"
  src="assets/pdfs/research-proposal.pdf"
  title="Research Proposal PDF"
  loading="lazy">
</iframe>
```

And add this to `style.css`:

```css
.pdf-preview {
  display: block;
  width: 100%;
  height: 650px;
  border: 1px solid var(--line);
  border-radius: 6px;
}
```

## Publish with GitHub Pages

1. Create a GitHub repository (for example, `andrew-green-1102-eportfolio`).
2. Upload the contents of this folder to the repository root. `index.html` must be at the root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for GitHub Pages to finish deploying. The public site URL will be shown in Settings → Pages.

This is a static site; no build command or framework is required.

## Before publishing

- Add the actual PDFs you want to share. Do not publish private or restricted class materials.
- The Google Survey artifact currently has no live form URL because one was not present in the supplied embed code. Add your public Google Forms link if you want visitors to open the form.
- Check that all assignment files and external source links are correct before submitting the portfolio.
