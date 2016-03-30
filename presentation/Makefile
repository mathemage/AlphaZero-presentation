all: AlphaGo.pdf

# LaTeX must be run multiple times to get references right
AlphaGo.pdf: AlphaGo.tex $(wildcard *.tex) bibliography.bib
	xelatex $<
	bibtex AlphaGo
	xelatex $<
	xelatex $<

minimal_example.pdf: minimal_example.tex $(wildcard *.tex)
	xelatex $<
	xelatex $<

clean:
	rm -f *.log *.dvi *.aux *.toc *.lof *.lot *.out *.bbl *.blg
	rm -f AlphaGo.pdf minimal_example.pdf
