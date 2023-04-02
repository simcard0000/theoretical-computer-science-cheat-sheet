EXTRAS = unit.tex angle.tex triangle.tex

cheatsheet.ps: cheatsheet.dvi
	dvips -f < cheatsheet.dvi > cheatsheet.ps
	ps2pdf cheatsheet.ps

# cheatsheet.pdf: $(EXTRAS) ecsher.png
#	pdftex cheatsheet.tex > cheatsheet.log

cheatsheet.dvi: $(EXTRAS) ecsher.eps
	tex cheatsheet.tex > cheatsheet.log 

unit.tex: unit.fig
	./bin/fig2tex -m 0.5 unit.fig

angle.tex: angle.fig
	./bin/fig2tex -m 0.3 angle.fig

triangle.tex: triangle.fig
	./bin/fig2tex -m 0.8 triangle.fig

ecsher.png: ecsher.eps
	convert -density 300 ecsher.eps -units PixelsPerInch  -colorspace gray +matte -colors 2 -depth 1 ecsher.png

clean:
	rm -f ecsher.png angle.tex triangle.tex unit.tex angle.pic triangle.pic unit.pic cheatsheet.dvi cheatsheet.pdf *.log *.bak cheatsheet.ps

tar:	clean
	cd /home/seiden_bit; tar cfv cheat.tar CHEAT; mv cheat.tar CHEAT
	gzip cheat.tar

# DO NOT DELETE THIS LINE -- make depend depends on it.

