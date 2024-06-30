# This Makefile is based somewhat on the Makefile present here:
# https://github.com/tompollard/phd_thesis_markdown/blob/main/Makefile

PANDOC=pandoc

BASEDIR=$(CURDIR)
INPUTDIR=$(BASEDIR)/source
OUTPUTDIR=$(BASEDIR)/output
BIBFILE=$(INPUTDIR)/references.bib

CSL="../../../csls/ieee-with-url.csl"
CSSFILE=$(INPUTDIR)/style.css
TEMPLATE=$(INPUTDIR)/template.html

pdf:
	pandoc  \
		--output "$(OUTPUTDIR)/out.pdf" \
		--pdf-engine=xelatex \
		--pdf-engine-opt=--shell-escape \
		"$(INPUTDIR)"/*.md \
		"$(INPUTDIR)/metadata.yml" \
		--bibliography="$(BIBFILE)" \
		--citeproc \
		--csl="$(CSL)"

html:
	$(PANDOC) \
		--output "$(OUTPUTDIR)/out.html" \
		--include-in-header="$(CSSFILE)" \
		"$(INPUTDIR)"/*.md \
		"$(INPUTDIR)/metadata.yml" \
		--bibliography="$(BIBFILE)" \
		--toc \
		--number-sections \
		--citeproc \
		--mathjax="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js" \
		--csl="$(CSL)"


all: pdf

.PHONY: help install pdf docx html tex
