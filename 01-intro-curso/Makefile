name-of-the-file = aoc-01-intro-curso

$(name-of-the-file).pdf: $(name-of-the-file).ps 
	ps2pdf $(name-of-the-file).ps

$(name-of-the-file).ps: $(name-of-the-file).dvi
	dvips $(name-of-the-file).dvi

$(name-of-the-file).dvi: $(name-of-the-file).tex ../slides-common/preambule.tex
	latex $(name-of-the-file).tex
	latex $(name-of-the-file).tex

view:
	evince $(name-of-the-file).pdf &

clean:
	rm *.aux *.dvi *.log *.ps *.toc *.bm
