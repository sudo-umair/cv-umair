# Muhammad Umair - CV/Resume Project

A professional CV/Resume built using the Awesome CV LaTeX template. This project contains a complete LaTeX-based curriculum vitae with modular sections and a cover letter template.

## 📋 Project Overview

This repository contains my personal CV built using the [Awesome CV LaTeX template](https://github.com/posquit0/Awesome-CV) by Claud D. Park. The project is structured to maintain a professional, clean, and easily maintainable resume.

## 🏗️ Project Structure

```
cv-umair/
├── awesome-cv.cls          # Main LaTeX class file for styling
├── resume.tex              # Main resume document
├── coverletter.tex         # Cover letter template
├── fonts/                  # Font files directory
│   ├── FontAwesome.ttf
│   ├── Roboto-Bold.ttf
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

## 🎯 Features

- **Modular Design**: Each section is in a separate `.tex` file for easy maintenance
- **Professional Styling**: Clean, modern design with customizable colors
- **Font Awesome Icons**: Professional icons for social links and sections
- **Responsive Layout**: Optimized for both A4 and letter paper sizes
- **Cover Letter Template**: Matching cover letter template included
- **Customizable Colors**: Multiple color schemes available

## 🛠️ Requirements

To compile this project, you need:

- **LaTeX Distribution**: TeX Live, MiKTeX, or MacTeX
- **XeLaTeX Compiler**: Required for font handling
- **Font Files**: Roboto and FontAwesome fonts (included in `fonts/` directory)

## 📦 Installation & Setup

1. **Clone the repository**:

   ```bash
   git clone <repository-url>
   cd cv-umair
   ```

2. **Ensure LaTeX is installed**:

   - **Windows**: Install MiKTeX or TeX Live
   - **macOS**: Install MacTeX
   - **Linux**: Install TeX Live

3. **Verify XeLaTeX is available**:
   ```bash
   xelatex --version
   ```

## 🚀 Usage

### Compiling the Resume

To generate the PDF resume:

```bash
xelatex resume.tex
```

### Compiling the Cover Letter

To generate the PDF cover letter:

```bash
xelatex coverletter.tex
```

### Multiple Compilations

For best results, compile twice to ensure proper formatting:

```bash
xelatex resume.tex
xelatex resume.tex
```

## 🎨 Customization

### Changing Colors

The template supports multiple color schemes. In `resume.tex` and `coverletter.tex`, modify:

```latex
\colorlet{awesome}{awesome-red}  % Change to your preferred color
```

Available colors:

- `awesome-emerald`
- `awesome-skyblue`
- `awesome-red`
- `awesome-pink`
- `awesome-orange`
- `awesome-nephritis`
- `awesome-concrete`
- `awesome-darknight`

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

### Adding/Removing Sections

To add or remove sections, modify the input statements in `resume.tex`:

```latex
\input{resume/summary.tex}
\input{resume/skills.tex}
\input{resume/experience.tex}
% Add or comment out sections as needed
```

## 📄 Output Files

After compilation, you'll get:

- `resume.pdf` - Your professional resume
- `coverletter.pdf` - Your cover letter template

## 🔧 Troubleshooting

### Common Issues

1. **Font Not Found**: Ensure all font files are in the `fonts/` directory
2. **Compilation Errors**: Make sure you're using XeLaTeX, not pdfLaTeX
3. **Missing Packages**: Install required LaTeX packages for your distribution

### Font Issues

If you encounter font-related errors:

1. Verify all `.ttf` files are in the `fonts/` directory
2. Ensure XeLaTeX is being used for compilation
3. Check that the `\fontdir[fonts/]` line is present in your documents

## 📝 License

This project uses the Awesome CV template which is licensed under:

- **Template**: CC BY-SA 4.0
- **Class File**: LPPL v1.3c

## 👤 About

**Muhammad Umair**

- Full Stack Engineer & React Native Engineer
- Based in Rawalpindi, Pakistan
- Contact: muhammadumair523@gmail.com
- GitHub: [sudo-umair](https://github.com/sudo-umair)
- LinkedIn: [sudo-umair](https://linkedin.com/in/sudo-umair)

## 🤝 Contributing

While this is a personal CV project, suggestions for improvements to the LaTeX structure or documentation are welcome.

## 📞 Contact

For questions about this CV template or LaTeX setup:

- Email: muhammadumair523@gmail.com
- GitHub: [sudo-umair](https://github.com/sudo-umair)

---

_Built with the Awesome CV LaTeX template - A professional and elegant CV template for LaTeX users._
