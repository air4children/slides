INKSCAPE?=inkscape	# Inkscape (svg support)
#
#https://scaron.info/blog/makefiles-for-latex.html

FIGURES_SVG=$(wildcard svg/*.svg)
FIGURES_PDF=$(subst svg/,pdf/,$(FIGURES_SVG:.svg=.pdf))

all:	$(FIGURES_PDF)

# Pattern rule for converting SVG to PDF
pdf/%.pdf: svg/%.svg  ## Figures for the manuscript
	$(INKSCAPE) --export-pdf $(@) $(<)

view:
	evince $(FIGURES_PDF)

clean:  ## Clean LaTeX and output figure files
	rm -f $(FIGURES_PDF) $(FIGURES_PNG)



