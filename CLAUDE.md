# Uskudar University Thesis Repository - Academic Paper Templates

## Repository Overview
This repository contains academic paper templates and research content for a master's thesis on ship detection using deep learning technology. The main research focuses on developing a YOLOv8-based ship detection system for the Istanbul Bosphorus strait.

## Research Topic
**"BOSPHORUS SHIP DETECTION SYSTEM: A Sophisticated Web Application for Maritime Surveillance Using YOLO Deep Learning Technology"**

- **Author**: Recep Ertugrul Eksi
- **Institution**: Uskudar University, Computer Engineering Department, Istanbul, Turkey
- **Research Focus**: YOLOv8-based ship detection for maritime surveillance
- **Key Performance**: 89% mAP@0.5 accuracy, real-time processing at 35 FPS

## Repository Structure

### Published Papers (Different Journal Formats)
1. **Computer Science Journal/** - Paper formatted for Computer Science journal (AGH)
2. **Journal of Computer Science and Technology/** - Same paper formatted for JCST journal

### Template Directories (Provided by Thesis Advisor)
1. **Template - Computer Science Journal/** - Complete template and documentation
2. **Template - Journal of Computer Science and Technology/** - Official JCST template

## Template Details

### Computer Science Journal (AGH) Template
**Location**: `Template - Computer Science Journal/`

**Key Files**:
- `template.tex` - Clean template with basic structure
- `sample-please-use-one-of-templates.tex` - Comprehensive 953-line tutorial and documentation
- `csagh.sty` - Complete LaTeX style package (628 lines)
- `cs-agh.bst` - Bibliography style file
- `moreverb.sty` - Enhanced verbatim environments
- `bibliography.bib` - Example bibliography entries
- `pdf/` - Sample figures directory

**Template Features**:
- Multi-author support with automatic affiliations
- Abstract and keywords formatting
- Custom section styling
- Mathematical formula support (AmS-LaTeX integration)
- Figure/table caption formatting
- Automatic page layout optimization
- Date/time stamping functionality
- Bibliography management with BibTeX

**Usage Instructions**:
```latex
\documentclass[10pt]{article}
\usepackage[pdftex]{graphicx}
\usepackage{csagh}

\begin{document}
\begin{opening}
\title{Your Paper Title}
\author[Institution, address, email]{Author Name}
\begin{abstract}
Your abstract here (max 250 words)
\end{abstract}
\keywords{keyword1, keyword2, keyword3}
\end{opening}

% Your content here

\bibliographystyle{cs-agh}
\bibliography{bibliography}
\end{document}
```

### Journal of Computer Science and Technology Template
**Location**: `Template - Journal of Computer Science and Technology/`

**Key Files**:
- `JCST-Template-_submit_202105.tex` - Official template with submission guidelines
- `JCST-Template-_submit_202105.pdf` - Compiled PDF showing expected output
- `JCST.bst` - Bibliography style for JCST journal
- `picins.sty` - Picture insertion and text wrapping package
- `photo.eps` - Sample image file

**Template Features**:
- Two-column layout for main content
- Multi-language support (CJK for Chinese characters)
- Comprehensive package imports for advanced mathematical typesetting
- Custom page layout and margins optimized for JCST
- Fancy headers with journal branding
- Abstract and keywords formatting
- Author affiliation management

## Research Content Summary

### Technical Approach
- **Architecture**: Three-tier web application (HTML5/CSS3, Flask, PostgreSQL)
- **Core Model**: YOLOv8s with maritime-specific optimizations
- **Dataset**: 150 high-resolution Bosphorus images with 852 annotated vessels
- **Performance**: 89% mAP@0.5, 87% precision, 84% recall

### Key Innovations
1. **Multi-Scale Detection Pipeline**: Processes images at three resolutions (640px, 832px, 1024px)
2. **Maritime Context Filtering**: Post-processing pipeline to reduce false positives
3. **Adaptive Thresholding**: Dynamic confidence adjustment based on image quality
4. **DBSCAN Clustering**: Intelligent merging of multi-scale detections

### Performance Comparison
| Method | mAP@0.5 | mAP@0.5:0.95 | FPS |
|--------|---------|--------------|-----|
| Faster R-CNN | 0.84 | 0.72 | 12 |
| RetinaNet | 0.82 | 0.69 | 15 |
| YOLOv5s | 0.85 | 0.73 | 31 |
| YOLOv8s (baseline) | 0.86 | 0.74 | 35 |
| **Our Method** | **0.89** | **0.77** | **35** |

## Working with Templates

### For Computer Science Journal Submission
1. Use `Template - Computer Science Journal/template.tex` as starting point
2. Refer to `sample-please-use-one-of-templates.tex` for comprehensive documentation
3. Include graphics in `pdf/` directory in PDF format
4. Use `cs-agh.bst` bibliography style
5. Follow the `\begin{opening}` structure for front matter

### For JCST Submission
1. Use `Template - Journal of Computer Science and Technology/JCST-Template-_submit_202105.tex`
2. Follow two-column format for main content
3. Include Chinese abstract if applicable (CJK support available)
4. Use `JCST.bst` bibliography style
5. Follow submission guidelines in template comments

### Common LaTeX Packages Used
- `amsmath`, `amssymb`, `amsthm` - Advanced mathematics
- `graphicx` - Graphics inclusion
- `booktabs` - Professional table formatting
- `cite` - Citation management
- `fancyhdr` - Custom headers/footers
- `multicol` - Multi-column layouts

## Bibliography Management
Both templates use BibTeX for reference management:
- **CS AGH**: Use `cs-agh.bst` style
- **JCST**: Use `JCST.bst` style
- Example entries available in `bibliography.bib`

## File Organization Best Practices
1. Keep main `.tex` file in root of template directory
2. Place figures in `pdf/` subdirectory (for CS AGH) or same directory (for JCST)
3. Use PDF format for vector graphics, PNG for bitmaps
4. Maintain separate `.bib` file for references
5. Use consistent naming conventions for labels and references

## Thesis Advisor Notes
- Templates provided for standardized formatting across journal submissions
- Same research content can be adapted to different journal requirements
- Focus on maintaining consistent technical content while adapting formatting
- Both journals are indexed in major databases (ESCI Web of Science, SCOPUS)

## Current Status
- Research completed and written for both journal formats
- Templates ready for future paper submissions
- Complete toolkit for academic paper preparation in LaTeX