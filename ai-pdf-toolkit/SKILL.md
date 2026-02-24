# AI PDF Toolkit

_AI-powered PDF creation, editing, and manipulation assistant_

## When to Use

Use this skill when you need to:
- Create PDFs from scratch or templates
- Edit existing PDF documents
- Convert documents to/from PDF
- Extract content from PDFs
- Merge or split PDF files
- Add annotations, signatures, watermarks
- Compress or optimize PDFs
- Create fillable PDF forms

## Core Capabilities

### PDF Creation
- Generate PDF from markdown, HTML, text
- Create PDF from AI-generated content
- Build templated PDFs (invoices, reports, contracts)
- Batch create multiple PDFs

### PDF Editing
- Modify text, images, layout
- Add/removing pages
- Rotate, crop, resize pages
- Extract specific sections

### Content Extraction
- Extract text from scanned PDFs (OCR)
- Pull images from PDFs
- Extract tables to Excel/CSV
- Parse forms and field data

### Automation
- Watch folder for automatic processing
- Scheduled PDF operations
- Integration with cloud storage

## Tools & Services

- **Adobe Acrobat API** - Full PDF manipulation
- **pdf-lib** - JavaScript PDF editing
- **PyPDF2** - Python PDF operations
- **PDF.js** - Browser-based PDF rendering
- **CloudConvert API** - Format conversions

## Workflows

1. **Document Generation**: Input data → Template selection → PDF generation → Save/Email
2. **Batch Processing**: Multiple files → Queue processing → Output folder
3. **OCR Pipeline**: Scan document → OCR processing → Searchable PDF

## Tips

- Always keep original files backed up
- Use compression for email-friendly sizes
- OCR quality depends on original document clarity
- Form fields need proper naming for data extraction
