LATEX       = pdflatex
CHECK_RERUN = grep "Rerun to get" $*.log

all: goals.pdf

%.pdf: %.tex
	${LATEX} $*
	( ${CHECK_RERUN} && ${LATEX} $* ) || echo "Done."
	( ${CHECK_RERUN} && ${LATEX} $* ) || echo "Done."
