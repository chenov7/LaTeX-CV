# LaTeX-CV

A clean, modern, and customizable LaTeX template for a professional CV/Resume with a two-column layout design.

## Features

- **Modern Design**: Professional two-column layout with blue accent colors
- **Easy Customization**: Simple placeholders for all sections
- **Responsive Layout**: Optimized for A4 paper format
- **Multiple Sections**:
  - Education
  - Academic Projects
  - Professional Experience
  - Skills (organized by proficiency)
  - Languages
  - Strengths
  - Interests
- **Professional Typography**: Custom styling with proper spacing and hierarchy
- **Icon Support**: FontAwesome5 icons for contact information (phone, email, LinkedIn, location)

## Project Structure

```
LaTeX-CV/
├── mainCV.tex          # Main CV template with placeholders
├── preview/
│   └── previewCV.tex   # Example CV with sample data (Engineer profile)
|   └── previewCV.pdf   # Compiled PDF of the example CV
└── README.md           # This file
```

## How to Use

### 1. Edit Your CV

Open `mainCV.tex` and replace the placeholder content with your information:
- Update personal information in the header
- Fill in your education history
- Add your academic projects
- Include your professional experience
- List your technical skills
- Add languages and proficiency levels
- Include your strengths and interests

### 2. Customize Colors

The template uses a primary blue color by default. To change it, modify the color definition:

```latex
\definecolor{primary}{RGB}{39,76,175}
```

### 3. Compile the PDF

Use any LaTeX compiler to generate the PDF:

```bash
pdflatex mainCV.tex
```

Or use an online LaTeX editor like Overleaf.

## Customizable Elements

- **Primary Color**: Defined in the `\definecolor{primary}` command
- **Page Margins**: Adjust in the `\geometry` command (currently 1cm on all sides)
- **Column Ratio**: Change `\columnratio{0.63}` to adjust left/right column width
- **Spacing**: Modify `\vspace` commands to adjust spacing between sections

## Template Sections

### Left Column
- Education
- Academic Projects
- Professional Experience

### Right Column
- Strengths
- Skills (technical skills and currently learning)
- Languages
- Interests

## Requirements

This template requires the following LaTeX packages:
- `geometry` - Page layout
- `xcolor` - Colors
- `paracol` - Two-column layout
- `fontawesome5` - Icons
- `hyperref` - Hyperlinks
- `setspace` - Line spacing

## Example

A complete example CV with a software engineer profile is provided in `preview/previewCV.tex`.

## Notes

- Ensure all necessary packages are installed in your LaTeX distribution
- The template is optimized for A4 paper size
- Adjust line breaks and spacing based on your content length
- FontAwesome5 icons require the `fontawesome5` package to be installed

## License

This template is free to use and modify for personal or professional purposes.
