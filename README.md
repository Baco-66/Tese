latexmk -xelatex template.tex --outdir=dissertacao
biber .\dissertacao\template
rm -r .\dissertacao\*

biber --validate_datamodel .\dissertacao\template