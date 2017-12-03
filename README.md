# Creating APA formatted documents with LaTeX

This guide is focused on using the APA format for homework assignments.

## Requirements

* MikTex
* Strawberry Perl
* latexmk (installed via MikTex package manager)
* Reference manager which supports BibTex format (for example Zotero)

## Configuring TexWorks

TexWorks must be manually configured to use latexmk.

1. Edit > Preferences > Typesetting
2. Click on the + icon

    Name:
        latexmk

    Program:
        latexmk.exe

    Arguments:
        -e
        $pdflatex=q/pdflatex $synctexoption %O %S/
        -pdf
        $fullname

    View PDF after running:
        (checked)

## Reference Management

Use a reference manager which supports exporting to the BibTex or BibLaTex
formats. Several options are available including Zotero and Mendeley.

### Zotero

One note about using Zotero. Exporting refernces using BibTex appears to
produce better results compared to BibLaTex, atleast when dealing with
journals that used named issues.
