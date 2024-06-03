latexmk -xelatex template.tex --outdir=dissertacao
biber .\dissertacao\template
rm -r .\dissertacao\*

biber --validate_datamodel .\dissertacao\template

Posso utilizar a opção -g para forçar recompilar e -gg para apagar tudo
latexmk -g -xelatex template.tex --outdir=dissertacao


latexmk -shell-escape -file-line-error -xelatex template 

