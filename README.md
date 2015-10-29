ocr-pdf
=======

Public Domain.

Requirements
------------

zsh
poppler-utils
libtiff-utils
tesseract-ocr
pdftk
make

Description
-----------

I wanted to OCR all of the scanner-created PDF files in a directory. I
went online and looked for programs that do it, and found some, but
each of the ones I tried made the files a lot bigger than they
were. After looking inside of the files using "pdfimages" and
"pdfinfo", I learned that the problem was that they were always
ripping the page images as RGB, but my PDF are mostly grayscale
scans. So, I wrote this script and Makefile to do the job.

The resulting PDF are slightly larger, of course, since they now
contain the OCR'ed text, but the scanned page images inside of them
are the same size as they were before, and still grayscale instead of
rgb.
