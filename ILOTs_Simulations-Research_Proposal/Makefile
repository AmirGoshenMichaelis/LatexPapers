
.PHONY: clean all distclean

all: pdf
	evince main.pdf
pdf: main.tex
	pdflatex main.tex
dvi: main.tex
	latex main.tex
bibtex: db.bib pdf
	bibtex main.aux
	pdflatex main.tex
clean: distclean
	rm -f *.pdf *.dvi
distclean:
	rm -f *.aux *.log *.bbl *.blg
