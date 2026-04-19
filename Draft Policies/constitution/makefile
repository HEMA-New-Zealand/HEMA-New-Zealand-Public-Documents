MD_ARGS = -V colorlinks=true -V linkcolor=blue -V date="`date +'%-dth %B %Y'`" --toc --toc-depth=2 --number-sections --shift-heading-level-by=-1
MDS = $(wildcard *.md)
PDFS = $(MDS:.md=.pdf)


.PHONY: all clean

all: $(PDFS)

%.pdf: %.md
	pandoc $(MD_ARGS) -o $@ $<


clean:
	-rm constitution.pdf
