TARGET=cinuf.pdf
SRC=$(TARGET:.pdf=.tex)
LATEX=pdflatex

all: $(TARGET)

clean:
	$(RM) $(TARGET) *.aux *.log *.out *.dvi *.bbl *.blg

.PHONY: clean

SUFFIXES: .pdf .tex

%.pdf: %.tex
	$(LATEX) $<
	$(RM) $(TARGET)
	$(LATEX) $<
	$(RM) $(TARGET)
	$(LATEX) $<
