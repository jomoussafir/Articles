LATEX = latex
BIBTEX = bibtex
MAKEINDEX = makeindex
DVIPS = dvips -f
PS2PDF = ps2pdf13
PDFLATEX = pdflatex
PSNUP = psnup
ACROREAD = acroread

SRC = EB.tex EB.bib
ROOT = EB

dvi: $(SRC)	
	$(LATEX) $(ROOT)
	$(DVIPS) $(ROOT).dvi > $(ROOT).ps

pdf: $(SRC)	
	$(PS2PDF) $(ROOT).ps

bib: $(SRC)
	$(BIBTEX) $(ROOT)

clean:
	rm -f *.aux *.log *.bbl *.out *.dvi *~
