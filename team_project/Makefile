.PHONY: all clean

all: main.pdf

main.pdf: main.tex appendix.tex references.bib $(wildcard assets/*.pdf) $(wildcard figs/*)
	latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex

clean:
	latexmk -c main.tex
