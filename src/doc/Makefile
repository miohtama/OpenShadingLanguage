
# by default, just make the document
all: languagespec.pdf


# document making rule: use pdflatex
languagespec.pdf: *.tex languagespec.aux macros.aux Figures/*.pdf
	pdflatex languagespec



# special command 'make index' to regenerate the index
index: languagespec_index

languagespec_index:
	pdflatex languagespec
	pdflatex languagespec
	makeindex languagespec
	pdflatex languagespec

