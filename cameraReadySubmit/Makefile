FILE=vonLaszewski-scimp-pearc18
VIEW=vonLaszewski-scimp-pearc18

all:
	pdflatex ${FILE}
	bibtex ${FILE}
	pdflatex ${FILE}
	pdflatex ${FILE}

real-clean: clean
	rm -rf *.pdf

clean:
	rm -rf *~ *.aux *.bbl *.dvi *.log *.out *.blg *.toc *.fdb_latexmk *.fls *.tdo *.synctex.gz

view:
	open ${VIEW}.pdf

# all dependce tracking taking care of by Latexmk
fast:
	latexmk -pdf ${FILE}

watch:
	latexmk -pvc -view=pdf ${VIEW}

.PHONY: all clean view fast watch
