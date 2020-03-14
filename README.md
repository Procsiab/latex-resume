# LaTeX Resume

[![Build Status](https://ci.procsiab.cf/api/badges/Procsiab/latex-resume/status.svg)](https://ci.procsiab.cf/Procsiab/latex-resume)
[![Website](https://img.shields.io/website?up_message=online&url=https%3A%2F%2Fbook.procsiab.cf%2Florenzo_prosseda.pdf)](https://book.procsiab.cf/lorenzo_prosseda.pdf)
[![License](https://img.shields.io/badge/license-GDPR-yellowgreen)](https://raw.githubusercontent.com/Procsiab/latex-resume/master/LICENSE)


This is a repository for my resume project, integrated into my CD server.

## Project structure

- `main.tex`: file principale, contenente preambolo, pagina del titolo e inclusione dei file per i capitoli;
- `main.tex`: main file containing preamble, title and content inclusions;
- `content.tex`: pure content file, without boilerplate code;
- `title.tex`: file containing the style for the document.

## Get the PDF version

The PDF file is built through a continues delivery system, which ensures the latest code is compiled to a document.

The CD server published the build product at this [address](https://book.procsiab.cf), where documents from other integrated repositories will be uploaded.

I've chose *Drone* as the CD server because its ease of set up through Linux Containers; the base image used during the compile step is a custom TexLive install, which you can learn more about [here](https://github.com/Procsiab/texlive-it).

### Compiling the code

You may just use the `make all` command in the repository's root and you will get the PDF file in the *pdf* folder. The requirements to compile are the following:
- a *texlive* installation newer than 2019;
- *make*;
- *latexmk*.

### The ***devel** branch

In the `devel` branch there will be the work in progress for this document.
