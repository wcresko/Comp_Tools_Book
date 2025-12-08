# Foundational Computational Tools for Bioengineers

A comprehensive Quarto book for graduate students in bioengineering and life sciences, covering essential computational skills including Unix/Linux, R programming, version control with Git/GitHub, and high-performance computing.

## About

This book accompanies a graduate-level course taught at the University of Oregon's Phil and Penny Knight Campus for Accelerating Scientific Impact. It provides practical, hands-on instruction in foundational computational tools that are essential for modern research.

## Contents

1. **Introduction to Computational Tools** - Why computational skills matter
2. **Computer Systems Architecture** - Understanding hardware and operating systems
3. **Unix Fundamentals** - Navigation and basic commands
4. **Files, Pipes, and Redirection** - Data processing pipelines
5. **GREP and Regular Expressions** - Pattern matching
6. **Shell Scripting** - Automation and reproducibility
7. **R Programming Fundamentals** - Statistical computing basics
8. **Tidy Data Principles** - Data organization best practices
9. **Version Control with Git and GitHub** - Tracking changes and collaboration
10. **High-Performance Computing with Talapas** - Using computing clusters

## Building the Book

### Prerequisites

- [Quarto](https://quarto.org/) (version 1.4 or later)
- [R](https://www.r-project.org/) (version 4.0 or later)
- R packages: `tidyverse`, `gt`, `knitr`

### Build Commands

```bash
# Preview the book (opens in browser with live reload)
quarto preview

# Render the complete book
quarto render

# Render to specific format
quarto render --to html
quarto render --to pdf
```

### Output

- HTML output is written to the `docs/` directory for GitHub Pages deployment
- PDF output is generated alongside HTML

## Deploying to GitHub Pages

1. Push the repository to GitHub
2. Go to Settings → Pages
3. Set Source to "Deploy from a branch"
4. Select branch `main` and folder `/docs`
5. Your site will be available at `https://username.github.io/repository-name/`

## Directory Structure

```
bioe_comp_tools_book/
├── _quarto.yml          # Book configuration
├── index.qmd            # Preface
├── references.qmd       # Bibliography page
├── references.bib       # BibTeX references
├── custom.scss          # Custom styling
├── apa.csl              # Citation style
├── chapters/            # Chapter content
│   ├── 01-introduction.qmd
│   ├── 02-computer-systems.qmd
│   ├── 03-unix-fundamentals.qmd
│   ├── 04-files-pipes.qmd
│   ├── 05-grep-regex.qmd
│   ├── 06-shell-scripting.qmd
│   ├── 07-r-programming.qmd
│   ├── 08-tidy-data.qmd
│   ├── 09-git-github.qmd
│   ├── 10-hpc-talapas.qmd
│   └── appendix-commands.qmd
├── images/              # Image assets
└── docs/                # Rendered output (for GitHub Pages)
```

## Customization

### Styling

Edit `custom.scss` to modify colors, fonts, and other visual elements. The book uses University of Oregon colors by default.

### Adding Chapters

1. Create a new `.qmd` file in the `chapters/` directory
2. Add the chapter to the `chapters:` list in `_quarto.yml`
3. Render the book

### Images

Place images in the `images/` directory and reference them in chapters:

```markdown
![Caption](../images/filename.png)
```

## Author

**William A. Cresko**  
Professor of Biology  
Phil and Penny Knight Campus for Accelerating Scientific Impact  
University of Oregon

## License

This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0).

## Acknowledgments

- Research Advanced Computing Services (RACS) at the University of Oregon
- Software Carpentry for foundational teaching materials
- The R and Quarto communities
