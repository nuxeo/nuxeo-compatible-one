	ALL=L4.1.1.pdf nuxeo-requirements.pdf nuxeo-requirements-sp1.pdf

all: $(ALL)

%.md: %.rst
	pandoc -o $@ $<

%.pdf: %.md
	markdown2pdf $<

clean:
	rm -f $(ALL) *.out *.dvi *.aux *.log *.idx *.toc
