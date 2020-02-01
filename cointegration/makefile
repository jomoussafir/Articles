LATEX = latex
BIBTEX = bibtex
MAKEINDEX = makeindex
DVIPS = dvips -f
DVIPDFM = dvipdfm
PDFLATEX = pdflatex
PSNUP = psnup
ACROREAD = acroread

ROOT = cointegration

dvi	: $(ROOT).tex
	$(LATEX) $(ROOT)
	$(DVIPS) $(ROOT).dvi > $(ROOT).ps

pdf	: $(ROOT).dvi
	$(DVIPDFM) $(ROOT)

bib	: $(ROOT).bib
	$(BIBTEX) $(ROOT)

clean	:
	rm *.aux *.log *~
