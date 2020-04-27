GS=/usr/local/bin/gs

# Convert text to paths using GhostScript, to block students from
# copy-pasting code from PDFs
worksheets_iot_nocopy.pdf: worksheets_iot.pdf
	$(GS) -o "$@" -dNoOutputFonts -sDEVICE=pdfwrite $<

worksheets_iot.pdf: worksheets_iot.tex
	pdflatex $<
	pdflatex $<
