.SUFFIXES: .pdf .dvi .tex
.PHONY: default clean distclean

FILE = acl

all: $(FILE).pdf

%.pdf: %.tex *.bib figures/*.pdf
	latexmk -pdf $*
clean:
	@$(RM) *.aux *.lof *.log *.lot *.out *.toc *.nav *.gz *.pag *.snm *.bbl *.blg *~ \#*\# *.fdb_latexmk

distclean: clean
	@$(RM) $(FILE).pdf $(FILE).dvi $(FILE).ps
