# _AboutThisSite
This site provides a collection of scripts to edit PDF files which are used as forms to submitted to various authorities. It is also intended to contain a collection of the data files needed to apply edits to particular forms.

## Scripts and/or programs

1. [Pdf Edit Bash](https://github.com/cli-pdf-editors/PdfEditBash/) A set of Bash shell scripts to create the data sets needed for a given form, and use that data to edit the PDF form.
2. Pdf Edit Ruby - this is planned for the future. The purpose is to make the use of this system possibly easier for Windows users than installing Bash on their computers.

## Premade forms

1. [TM7](https://github.com/cli-pdf-editors/TM7/) The form used to apply for an extension of stay in the Kingdom of Thailand.

## Limitations

Multi-byte UTF-8 characters may not be used presently. This is because the system works by bursting the original PDF form into single pages, converting the pages to be edited into _postscript_ files, adding the users edits to such files, then converting back to PDF and re-assembling the PDF document. Whilst UTF-8 is quite useable in _postcript_ documents, the data gets mangled on conversion back to PDF.

In future, I plan to move the system on to direct editing of the PDF forms in the hope that it will make UTF-8 multi-byte characters useable in the edits.

