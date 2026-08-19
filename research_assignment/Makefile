.PHONY: all clean

all: main.pdf

main.pdf: main.tex $(wildcard assets/*.pdf)
	latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex

clean:
	latexmk -c main.tex
