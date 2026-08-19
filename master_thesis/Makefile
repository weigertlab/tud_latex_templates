.PHONY: all clean

all: main.pdf

main.pdf: main.tex references.bib $(wildcard assets/*.pdf) $(wildcard frontmatter/*.tex) $(wildcard chapters/*.tex)
	latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex

clean:
	latexmk -c main.tex
