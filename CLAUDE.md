# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static academic portfolio website for Lingjie Liu, hosted on GitHub Pages at `lingjie0206.github.io`. The site serves as a personal academic homepage showcasing research publications, CV, and professional information in computer graphics and AI.

## Architecture

**Frontend Technology Stack:**
- HTML5/CSS3/JavaScript static website
- Bootstrap 3.x framework for responsive layout
- jQuery for DOM manipulation and interactions
- Owl Carousel for image galleries
- Font Awesome for icons
- SCSS for CSS preprocessing

**Key Directory Structure:**
- `index.html` - Main homepage with personal info and research overview
- `index_bycategory.html` - Alternative view organizing content by categories
- `css/` - Compiled CSS files including Bootstrap and custom styles
- `scss/` - SCSS source files with modular styling
- `js/` - JavaScript libraries and custom scripts
- `images/` - Research project images, GIFs, and personal photos
- `papers/` - Individual project pages with HTML templates, assets, and PDFs
- `documentation/` - Template documentation (appears to be from original theme)
- `php/` - Contact form processing (may not be functional on GitHub Pages)

**Content Management:**
- Research publications are organized in `papers/` subdirectories
- Each project has its own folder with index.html, assets, and PDF
- Project images and media files stored in `images/`
- Academic CV stored as `LingjieLiu_CV.pdf`

## Development Workflow

**No Build System:**
This is a static HTML website with no build process or package.json. Changes are made directly to HTML/CSS/JS files.

**SCSS Compilation:**
- SCSS files in `scss/` directory need compilation to `css/style.css`
- Main entry point: `scss/style.scss`
- Modular structure with separate files for variables, mixins, typography

**Deployment:**
- Hosted on GitHub Pages
- Files are served directly from the repository
- Any changes to master branch are automatically deployed

## Common Development Tasks

**Adding New Research Publications:**
1. Create new directory in `papers/[project-name]/`
2. Add project HTML page using existing templates as reference
3. Include project assets (images, videos, PDFs) in project directory
4. Add project thumbnail and description to main `index.html`
5. Update both `index.html` and `index_bycategory.html` if needed

**Updating Styling:**
1. Modify SCSS files in `scss/` directory
2. Compile SCSS to CSS (manual process - no automated build)
3. Ensure responsive behavior across devices

**Content Updates:**
- Personal information: Edit `index.html` directly
- CV: Replace `LingjieLiu_CV.pdf` file
- Project media: Add to `images/` directory with descriptive names

## File Organization Patterns

**Project Pages:** Each research project follows a consistent structure in `papers/[name]/`:
- `index.htm` - Project page HTML
- `css/` - Project-specific styling
- `images/` - Project images and logos
- `mp4/` - Video demonstrations
- `logos/` - Institution logos
- `data/` - BibTeX and supplementary files

**Image Naming:** Project images use descriptive names (e.g., `curvefusion.jpg`, `nerfdiff.gif`)

**Academic Content:** Publications include proper BibTeX citations and links to papers, code, and supplementary materials.