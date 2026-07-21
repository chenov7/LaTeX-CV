# LaTeX-CV

A collection of clean, modern, and customizable LaTeX templates for a professional CV/Resume, each with a two-column layout design.

## Templates

### 1. Classic

A two-column layout with FontAwesome5 icons for contact information.

- **Modern Design**: Professional two-column layout with blue accent colors
- **Icon Support**: FontAwesome5 icons for contact information (phone, email, LinkedIn, location)
- **Sections**: Education, Academic Projects, Experience, Strengths, Skills, Languages, Interests

Files: [`templates/classic/mainCV.tex`](templates/classic/mainCV.tex) (template) · [`templates/classic/preview/previewCV.tex`](templates/classic/preview/previewCV.tex) (filled example) · [`templates/classic/preview/preview_CV.pdf`](templates/classic/preview/preview_CV.pdf) (compiled preview)

### 2. Modern

A two-column layout with a photo header, an accent-ruled section style, and a denser layout suited to longer profiles (projects, certifications, activities).

- **Photo Header**: Name, headline and contact details alongside a profile photo
- **Sections**: Professional Summary, Education, Professional Experience, Projects, Areas of Expertise, Languages, Certifications, Activities & Associations, Interests

Files: [`templates/modern/mainCV.tex`](templates/modern/mainCV.tex) (template) · [`templates/modern/preview/previewCV.tex`](templates/modern/preview/previewCV.tex) (filled example)

> Note: the Modern template requires a photo file (referenced as `photo.jpg` next to the `.tex` file) to compile — add your own image before running `pdflatex`.

## Project Structure

```
LaTeX-CV/
├── templates/
│   ├── classic/
│   │   ├── mainCV.tex          # Classic template with placeholders
│   │   └── preview/
│   │       ├── previewCV.tex   # Example CV with sample data (Engineer profile)
│   │       └── preview_CV.pdf  # Compiled preview
│   └── modern/
│       ├── mainCV.tex          # Modern template with placeholders
│       └── preview/
│           └── previewCV.tex   # Example CV with sample data (Engineer profile)
└── README.md                   # This file
```

## How to Use

### 1. Pick a Template

Choose `templates/classic/mainCV.tex` or `templates/modern/mainCV.tex` as your starting point.

### 2. Edit Your CV

Replace the placeholder content with your information:
- Update personal information in the header (and add a photo for the Modern template)
- Fill in your education history
- Add your academic/personal projects
- Include your professional experience
- List your technical skills
- Add languages and proficiency levels
- Include your strengths/interests (and certifications/activities for the Modern template)

### 3. Customize Colors

Both templates use a primary blue accent color by default. To change it, modify the color definition:

```latex
% Classic
\definecolor{primary}{RGB}{39,76,175}

% Modern
\definecolor{accent}{RGB}{39,76,175}
```

### 4. Compile the PDF

Use any LaTeX compiler to generate the PDF:

```bash
pdflatex templates/classic/mainCV.tex
pdflatex templates/modern/mainCV.tex
```

Or use an online LaTeX editor like Overleaf.

## Customizable Elements

- **Accent Color**: Defined via `\definecolor{primary}` (Classic) or `\definecolor{accent}` (Modern)
- **Page Margins**: Adjust in the `\geometry` command
- **Column Ratio**: Change `\columnratio{...}` to adjust left/right column width
- **Spacing**: Modify `\vspace` commands to adjust spacing between sections

## Requirements

- **Classic** requires: `geometry`, `xcolor`, `paracol`, `fontawesome5`, `hyperref`, `setspace`
- **Modern** requires: `extarticle` class, `geometry`, `xcolor`, `paracol`, `mathpazo`, `microtype`, `graphicx`, `hyperref`, `enumitem`, `silence`

## Notes

- Ensure all necessary packages are installed in your LaTeX distribution
- Both templates are optimized for A4 paper size
- Adjust line breaks and spacing based on your content length
- FontAwesome5 icons (Classic template) require the `fontawesome5` package to be installed

## License

These templates are free to use and modify for personal or professional purposes.
