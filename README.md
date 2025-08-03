# Muhammad Umair - Professional CV/Resume

A modern, professional CV/Resume built using the Awesome CV LaTeX template. This project showcases a comprehensive curriculum vitae with modular sections, clean typography, and a matching cover letter template.

## 📋 Project Overview

This repository contains my professional CV built using the [Awesome CV LaTeX template](https://github.com/posquit0/Awesome-CV) by Claud D. Park. The project is designed with a modular architecture for easy maintenance and customization, featuring a clean, modern design optimized for both digital and print formats.

### Key Features

- **Modular Architecture**: Each section is in a separate `.tex` file for easy maintenance
- **Professional Design**: Clean, modern layout with customizable color schemes
- **Font Awesome Integration**: Professional icons for social links and sections
- **Responsive Layout**: Optimized for both A4 and letter paper sizes
- **Cover Letter Template**: Matching cover letter template included
- **Cross-Platform**: Works on Windows, macOS, and Linux

## 🏗️ Project Structure

```
cv-umair/
├── awesome-cv.cls          # Main LaTeX class file for styling
├── resume.tex              # Main resume document
├── coverletter.tex         # Cover letter template
├── fonts/                  # Font files directory
│   ├── FontAwesome.ttf     # Icon font
│   ├── Roboto-Bold.ttf     # Typography fonts
│   ├── Roboto-BoldItalic.ttf
│   ├── Roboto-Italic.ttf
│   ├── Roboto-Light.ttf
│   ├── Roboto-LightItalic.ttf
│   ├── Roboto-Medium.ttf
│   ├── Roboto-MediumItalic.ttf
│   ├── Roboto-Regular.ttf
│   ├── Roboto-Thin.ttf
│   └── Roboto-ThinItalic.ttf
└── resume/                 # Modular resume sections
    ├── summary.tex         # Professional summary
    ├── skills.tex          # Technical skills
    ├── experience.tex      # Work experience
    ├── projects.tex        # Projects portfolio
    ├── education.tex       # Educational background
    ├── honors.tex          # Awards and honors
    └── certification.tex   # Certifications
```

## 🎯 Professional Background

**Muhammad Umair** - Full Stack Engineer & React Native Engineer

- **Current Role**: Mid-Senior Full Stack Engineer at Codejunkie Co., Ltd.
- **Location**: Rawalpindi, Pakistan
- **Specialization**: Web & Mobile Development, React.js, React Native, Node.js
- **Experience**: 4+ years in full-stack development and mobile app development

### Core Competencies

- **Frontend**: React.js, Next.js, React Native, Redux, Zustand
- **Backend**: Node.js, Express.js, REST/GraphQL APIs
- **Mobile**: React Native, Reanimated, Gesture Handler
- **Database**: Firebase, Supabase, SQL/NoSQL
- **Tools**: Git, Figma, Performance Optimization

## 🛠️ Technical Requirements

### Prerequisites

- **LaTeX Distribution**: TeX Live, MiKTeX, or MacTeX
- **XeLaTeX Compiler**: Required for advanced font handling
- **Font Files**: Roboto and FontAwesome fonts (included in `fonts/` directory)

### System Requirements

- **Windows**: MiKTeX or TeX Live
- **macOS**: MacTeX
- **Linux**: TeX Live

## 📦 Installation & Setup

### 1. Clone the Repository

```bash
git clone <repository-url>
cd cv-umair
```

### 2. Install LaTeX Distribution

**Windows:**

```bash
# Install MiKTeX from https://miktex.org/
# Or install TeX Live from https://www.tug.org/texlive/
```

**macOS:**

```bash
# Install MacTeX
brew install --cask mactex
```

**Linux:**

```bash
# Ubuntu/Debian
sudo apt-get install texlive-full

# CentOS/RHEL
sudo yum install texlive-scheme-full
```

### 3. Verify Installation

```bash
xelatex --version
```

## 🚀 Usage Guide

### Compiling the Resume

Generate the PDF resume:

```bash
xelatex resume.tex
```

### Compiling the Cover Letter

Generate the PDF cover letter:

```bash
xelatex coverletter.tex
```

### Best Practices

For optimal results, compile twice to ensure proper formatting:

```bash
xelatex resume.tex
xelatex resume.tex
```

### Output Files

After compilation, you'll get:

- `resume.pdf` - Professional resume
- `coverletter.pdf` - Cover letter template

## 🎨 Customization Guide

### Color Schemes

The template supports multiple professional color schemes. In `resume.tex` and `coverletter.tex`, modify:

```latex
\colorlet{awesome}{awesome-red}  % Change to your preferred color
```

**Available Color Options:**

- `awesome-emerald` - Professional green
- `awesome-skyblue` - Modern blue
- `awesome-red` - Classic red
- `awesome-pink` - Contemporary pink
- `awesome-orange` - Energetic orange
- `awesome-nephritis` - Sophisticated green
- `awesome-concrete` - Neutral gray
- `awesome-darknight` - Dark theme

### Personal Information

Update your personal information in both `resume.tex` and `coverletter.tex`:

```latex
\name{Your}{Name}
\position{Your Position}
\address{Your Address}
\mobile{Your Phone}
\email{your.email@example.com}
\github{your-github}
\linkedin{your-linkedin}
```

### Section Management

To add or remove sections, modify the input statements in `resume.tex`:

```latex
\input{resume/summary.tex}
\input{resume/skills.tex}
\input{resume/experience.tex}
% Add or comment out sections as needed
```

## 🔧 Troubleshooting

### Common Issues & Solutions

#### 1. Font Not Found

**Problem**: Font-related compilation errors
**Solution**:

- Ensure all `.ttf` files are in the `fonts/` directory
- Verify the `\fontdir[fonts/]` line is present in your documents
- Use XeLaTeX, not pdfLaTeX

#### 2. Compilation Errors

**Problem**: LaTeX compilation fails
**Solution**:

- Ensure you're using XeLaTeX: `xelatex resume.tex`
- Install required LaTeX packages for your distribution
- Check for syntax errors in `.tex` files

#### 3. Missing Packages

**Problem**: Package not found errors
**Solution**:

- Update your LaTeX distribution
- Install missing packages through your LaTeX package manager
- For MiKTeX: Use MiKTeX Console to install packages
- For TeX Live: Use `tlmgr install <package-name>`

### Performance Optimization

For faster compilation:

```bash
# Clean auxiliary files
rm *.aux *.log *.out *.fls *.fdb_latexmk

# Use latexmk for automatic compilation
latexmk -xelatex resume.tex
```

## 📄 Document Structure

### Resume Sections

1. **Summary** - Professional overview and career objectives
2. **Skills** - Technical competencies and tools
3. **Experience** - Work history and achievements
4. **Projects** - Portfolio of significant projects
5. **Education** - Academic background
6. **Honors** - Awards and recognitions
7. **Certifications** - Professional certifications

### Cover Letter Features

- Matching design with resume
- Professional formatting
- Customizable content sections
- Print-ready layout

## 📝 License Information

This project uses the Awesome CV template with the following licenses:

- **Template**: CC BY-SA 4.0 (Creative Commons Attribution-ShareAlike 4.0)
- **Class File**: LPPL v1.3c (LaTeX Project Public License)

## 👤 About the Author

**Muhammad Umair**

- **Role**: Full Stack Engineer & React Native Engineer
- **Location**: Rawalpindi, Pakistan
- **Experience**: 4+ years in software development
- **Specialization**: Web & Mobile Development, Performance Optimization
- **Contact**: muhammadumair523@gmail.com

### Professional Links

- **GitHub**: [sudo-umair](https://github.com/sudo-umair)
- **LinkedIn**: [sudo-umair](https://linkedin.com/in/sudo-umair)
- **Portfolio**: [Portfolio](https://portfolio-umair-five.vercel.app)

## 🤝 Contributing

While this is a personal CV project, suggestions for improvements are welcome:

- **Documentation**: Improve README clarity and completeness
- **LaTeX Structure**: Enhance template organization
- **Bug Reports**: Report compilation issues or formatting problems
- **Feature Requests**: Suggest new features or improvements

## 📞 Contact & Support

For questions about this CV template, LaTeX setup, or professional inquiries:

- **Email**: muhammadumair523@gmail.com
- **GitHub**: [sudo-umair](https://github.com/sudo-umair)
- **LinkedIn**: [sudo-umair](https://linkedin.com/in/sudo-umair)

## 🔗 Related Resources

- [Awesome CV Template](https://github.com/posquit0/Awesome-CV) - Original template
- [LaTeX Documentation](https://www.latex-project.org/) - LaTeX reference
- [XeLaTeX Guide](https://en.wikibooks.org/wiki/LaTeX/XeLaTeX) - XeLaTeX documentation

---

_Built with the Awesome CV LaTeX template - A professional and elegant CV template for LaTeX users._

_Last updated: December 2024_
