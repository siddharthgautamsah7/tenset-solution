FINAL VERSION — DARK THEME + REAL PDF FIRST-PAGE THUMBNAILS

Firebase is NOT used.

PDF thumbnails:
This version uses PDF.js from cdnjs and renders page 1 of each PDF into the card. It is already wired into every subject page.

Add a PDF:
1. Upload it to the deployed project, e.g.:
   solutions/science/Science Set 1.pdf

2. Edit solutions.json:
{
  "science": [
    {
      "title": "Science Set 1",
      "file": "solutions/science/Science Set 1.pdf"
    }
  ],
  "maths": [],
  "english": [],
  "nepali": [],
  "social": []
}

3. Publish/deploy the complete project.

Important:
- The PDF must be online at the exact path in solutions.json.
- PDF.js is loaded from cdnjs, so visitors need internet access.
- Same-origin PDFs are recommended; this avoids CORS problems.
- The thumbnail is the actual first page, not a placeholder.
