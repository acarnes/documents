
TEXINPUTS := ./sty:./tex

all: qft.pdf

qft.pdf: qft.tex
	pdflatex --output-format=pdf qft.tex 
	bibtex qft 
	pdflatex --output-format=pdf qft.tex 
	pdflatex --output-format=pdf qft.tex 

clean: 
	rm -f qft.pdf
	rm -f qft.bib.info qft.bib qft.bbl
	rm -f qft.log qft.lot qft.dvi qft.aux qft.out qft.toc qft.lof
	rm -f *~ tex/*~ tex/*.aux


