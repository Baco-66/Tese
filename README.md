latexmk -xelatex template.tex --outdir=dissertacao
biber .\dissertacao\template
rm -r .\dissertacao\*

biber --validate_datamodel .\dissertacao\template

Posso utilizar a opção -g para forçar recompilar em vez de estar a apagar
latexmk -g -xelatex template.tex --outdir=dissertacao
