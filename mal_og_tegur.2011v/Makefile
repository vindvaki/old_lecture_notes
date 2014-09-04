TEX := mal_og_tegur.2011v.tex
PDF := $(TEX:%tex=%pdf)
PS  := $(TEX:%tex=%ps)
DVI := $(TEX:%tex=%dvi)

$(PDF): $(TEX)
	latexmk -pdf $<

clean-tmp:
	latexmk -pdf -c -quiet $(TEX)

clean: clean-tmp
	rm -rf $(PDF) $(PS) $(DVI)

.PHONY: clean clean-tmp
