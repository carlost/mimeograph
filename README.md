			            ||                                                              '||      
			.. .. ..   ...  .. .. ..     ....    ...     ... . ... ..   ....   ... ...   || ..   
			 || || ||   ||   || || ||  .|...|| .|  '|.  || ||   ||' '' '' .||   ||'  ||  ||' ||  
			 || || ||   ||   || || ||  ||      ||   ||   |''    ||     .|' ||   ||    |  ||  ||  
			.|| || ||. .||. .|| || ||.  '|...'  '|..|'  '||||. .||.    '|..'|'  ||...'  .||. ||. 
			                                           .|....'                  ||               
			                                                                   ''''              
## Description
mimeograph is a simple CoffeeScript library to extract text from a PDF, OCRing where necessary.  None of the 
actual PDF operation is performed by the CoffeeScript, everything is farmed out to pdftotext, imagemagick 
and tesseract.

## System Requirements
- poppler-utils (pdftotext)
- libtiff
- Leptonica
- tesseract
- ImageMagick

## Install

	$ git clone git@github.com:morologous/mimeograph.git
	$ cd mimeograph
	$ make link
	
## Running

	Usage:
	  mimeograph [OPTIONS] filename

	Available options:
	  -h, --help         Displays options
	  -v, --version      Shows certain's version.
	  -w, --workers      Number of workers to create. Ex.: 5 (default)
	  -s, --start        Starts a Mimeograph daemon.
	  -r, --request      Kicks of the processing of a new file.

	v0.1.0
	
	eg.  mimeograph -r test/test.pdf
	     mimeograph -w 10 -s

## License

MIT License

Copyright (c) 2011 Jason Yankus

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

#### Author: [Jason Yankus]()
#### Contributors: [Sean McDaniel]()

