all: leaflet.pdf

leaflet.pdf: leaflet.tex
	pdflatex $<

clean:
	rm -f *.log *.dvi *.aux *.toc *.lof *.lot *.out *.bbl *.blg *._aux *._log *.nav *.synctex.gz *.project.vim .tmp/*
	rm -f leaflet.pdf
