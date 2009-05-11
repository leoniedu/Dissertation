all:
	latex main
	bibtex main
	latex main
	latex main

fast:
	latex main

clean:
	@-rm main.aux main.log main.out main.bak main.blg main.bbl main.toc main.lof main.lot 2> /dev/null
        
pdf:
	@if [ -f main.ps ]; then rm main.ps; fi
	@if [ -f main.pdf ]; then rm main.pdf; fi
	@make
	@dvips -t letter main.dvi -o main.ps
	@ps2pdf main.ps
	@rm main.ps
