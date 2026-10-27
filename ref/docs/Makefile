.PHONY: all clean

all:
	mkdir -p build/tex-cache
	TEXMFVAR="$(CURDIR)/build/tex-cache" TEXMFCACHE="$(CURDIR)/build/tex-cache" latexmk -lualatex -interaction=nonstopmode -halt-on-error -auxdir=build -outdir=. explanation.tex

clean:
	latexmk -c -auxdir=build -outdir=. explanation.tex
