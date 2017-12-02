# Creating APA formatted documents with LaTeX

This guide is focused on using the APA format for homework assignments.

## Requirements

* MikTex
* Strawberry Perl
* latexmk (installed via MikTex package manager)
* Reference manager which supports BibTex format (for example Zotero)

## Configuring TexWorks

TexWorks must be manually configured to use latexmk.

Edit > Preferences > Typesetting

Click on + icon

Name:

    latexmk

Program:

    latexmk.exe

Arguments:

    -e
    $pdflatex=q/pdflatex $synctexoption %O %S/
    -pdf
    $fullname

View PDF after running (checked)
