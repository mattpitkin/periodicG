# Makefile

default: pdf

pdf: comment.tex comment.bib
	latex comment.tex
	bibtex comment
	latex comment.tex
	latex comment.tex
	dvips comment.dvi
	ps2pdf comment.ps

clean:
	rm -f *.aux *.log *.out *.blg *.dvi *.bbl *.backup
