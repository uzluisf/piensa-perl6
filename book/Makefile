
### Input file
FILENAME = thinkperl6
OUTPUT_NAME = thinkperl6

all: tmpDir/$(FILENAME).pdf

### Compilation flags for pdflatex
PDFLATEX_FLAGS  = -halt-on-error\
				  -interaction=batchmode\
				  -output-format pdf\
				  -output-directory tmpDir\
				  -jobname=$(OUTPUT_NAME)
TEXINPUTS = .:tmpDir/
TEXMFOUTPUT = tmpDir

### Compile tex into pdf
tmpDir/:
	mkdir -p tmpDir/

tmpDir/$(FILENAME).aux: tmpDir/
	pdflatex $(PDFLATEX_FLAGS) $(FILENAME)

tmpDir/$(FILENAME).pdf: tmpDir/$(FILENAME).aux
	pdflatex $(PDFLATEX_FLAGS) $(FILENAME)

### Clean
# Clean temporary files (including created PDF file) by removing
# the directory tmpDir/ created during the compilation process.

clean:
	rm -rfv tmpDir/
