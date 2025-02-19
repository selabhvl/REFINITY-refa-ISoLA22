.PHONY: main clean FORCE

export OSFONTDIR := $OSFONTDIR;./fonts

main: p.pdf p-notes.pdf

%.pdf: FORCE
	latexmk -pdflatex='lualatex -interaction nonstopmode' -pdf $(patsubst %.pdf,%.tex,$@)

clean:
	latexmk -pdf -C
