title.ps: sheet.tex page1.tex page2.tex
	latex sheet.tex
	latex sheet.tex
	dvips -x 1500 -y 1500 -O -4.0cm,-5.0cm -o sheet2.ps sheet.dvi
	dvips -b 2 -x 1500 -y 1500 -O -4.0cm,-5.0cm -o sheet.ps sheet.dvi
	mpage -T -o -2 sheet.ps > title.ps

.PHONY: clean
clean:
	rm -rf *.aux *.log *.dvi *.bbl *.blg *.toc *.ps
