# Curriculum Vitae Generator

This project provides the source files and resources to generate a professional curriculum vitae (CV) in PDF format. It uses [md2html](https://github.com/dabresua/md2html), a Markdown to HTML converter, to transform a Markdown CV into a styled HTML page, which can then be exported or printed as a PDF.

## Project Structure

- `src/DBS_CV_remote.md`: The main CV content in Markdown format.
- `responsive.css`: Custom CSS for styling the CV.
- `index.html`: The generated HTML file (output).
- `img/`: Folder containing images used in the CV.

## How to Generate the Files

1. **Initialize the project:**
   - Run:
     ```sh
     make init
     ```
   - This will download and set up the required `md2html` tool and any dependencies.

2. **Generate the HTML file:**
   - Run:
     ```sh
     make
     ```
   - This will convert the Markdown CV to a styled HTML file (`index.html`).
   - This also will generate the file `DBS_CV_remote.pdv`

3. **Push changes to the repository:** 
    - Run:
     ```sh
     cp out/DBS_CV_remote.pdf DBS_CV_remote.pdf
     git add DBS_CV_remote.pdf
     git commit -m "Updated CV on PDF format"
     git push
     ```

For more details, see the comments in the `Makefile` and the documentation for `md2html`.