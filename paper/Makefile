NAME=main

all:
	pdflatex -shell-escape ${NAME}.tex
	bibtex ${NAME}
	pdflatex -shell-escape ${NAME}.tex
	pdflatex -shell-escape ${NAME}.tex

clean:
	rm -f ${NAME}.aux
	rm -f ${NAME}.auxlock
	rm -f ${NAME}.bbl
	rm -f ${NAME}.blg
	rm -f ${NAME}.log
	rm -f ${NAME}.out
	rm -f ${NAME}.run.xml
	rm -f ${NAME}-blx.bib
	rm -f *.*~
	rm -f sections/*.tex~

squeaky: clean
	rm -rf .texpadtmp
	rm -f ${NAME}.dvi
	rm -f ${NAME}.ps
	rm -f ${NAME}.pdf

