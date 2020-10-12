.PHONY: default dvi

default: inf3200-a2-membership.pdf

# Compatibility with Vim-Tex plugin's default make command
dvi: default

%.pdf: %.tex $(wildcard *.bib)
	pdflatex $(PDFLATEXFLAGS) $<
	biber $(basename $<)
	pdflatex $(PDFLATEXFLAGS) $<
	pdflatex $(PDFLATEXFLAGS) $<
