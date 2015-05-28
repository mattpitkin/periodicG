# Makefile

# to convert figures from svg, as produced by the ipython notebook, to eps and keep the vector graphics
# I can use inkscape in command line mode e.g.
# inkscape -f file.svg -E file.eps

default: pdf

pdf: comment.tex comment.bib
	latex comment.tex
	bibtex comment
	latex comment.tex
	latex comment.tex
	dvips comment.dvi
	ps2pdf comment.ps

revised: comment_revised.tex comment_revised.bib
	latex comment_revised.tex
	bibtex comment_revised
	latex comment_revised.tex
	latex comment_revised.tex
	dvips comment_revised.dvi
	ps2pdf comment_revised.ps

clean:
	rm -f *.aux *.log *.out *.blg *.dvi *.backup
