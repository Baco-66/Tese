latexmk -xelatex template.tex --outdir=dissertacao
biber .\dissertacao\template

biber --validate_datamodel .\dissertacao\template