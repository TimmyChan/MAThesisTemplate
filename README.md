# MAThesisTemplate
LaTeX files for MA theses at San Francisco State University
[Version 1.1 of 22 Apr 2017]
## Contents
This archive should contain the following files:
```
abstract.tex
acknowledgements.tex
content.tex
intrograph.pdf
MAThesisOutputFormat.sty
README.md
sfsuthesis.cls
thesis.bib
thesis.tex
```
## Instructions

* Copy all of the files in the same directory. You may do this also by pulling directly from the github.

* ```thesis.tex``` is the "mother file," which calls up the other files. LaTeX should compile this file. There are two modes: draft-editing and final version. The draft mode produces single-spaced output with 1-inch margins and a simple title page. The final-version mode produces an output that should be acceptable to the Graduate Division: double spacing, the right margins, copyright, signatures, abstract, acknowledgment pages, table of content, list of figures, etc. You can switch between both modes by going to line 21 in ```thesis.tex``` from

```\usepackage[draft]{MAThesisOutputFormat} ``` to ```\usepackage[final]{MAThesisOutputFormat}```

Custom definitions and packages should be made and included in thesis.tex, so that they will be useable in both modes. For running the ```final``` mode, you will need the tocloft package, which might not be installed by default in your TeX distribution. If it isn't google 'tocloft' (the current website is http://www.ctan.org/tex-archive/help/Catalogue/entries/tocloft.html).

* ```MAThesisOutputFormat.sty``` contains the TeX formatting for the draft-editing and final mode. In principle, you shouldn't have to alter this file. This file also contains the TeX formatting for the final version and the front matter for the final thesis. It uses sfsuthesis.cls as the class file. Some data (committee names, abstract, acknowledgments, etc.) has to be included into this file, but you shouldn't have to alter the layout definitions. One possible exception is the margins, since they can depend on the printer you're using. If they are off, the problem is most likely the text height; try changing the number in the line ```\textheight=7.1in``` of the file.

* ```content.tex``` will eventually contain the main body of your thesis, starting with Chapter 1. For now, this file contains various tips and tricks about LaTeX (which you will delete once you're ready for your thesis). The file intrograph.pdf is needed to produce the figures in this sample file. You can delete this file once you're working on your own text.

* ```thesis.bib``` contains the bibliography entries (which can be obtained from databases such as MathSciNet). Run LaTeX, BibTeX, LaTeX on thesis.tex to produce the bibliography.

* ```abstract.tex``` contains the optional abstract section - simply leave this file empty if you do not wish to have an abstract.

* ```acknowledgements.tex``` contains the optional acknowledgments section - simply leave this file empty if you do not wish to give acknowledgements.

For comments, problems, or suggestions, please contact Matt Beck (```mattbeck@sfsu.edu```).

## Filing the Thesis
Postscript: Here is an "algorithm" how to file your thesis (thanks to Eric Etu):
1) Print out all of your "preamble" pages (Cover Page, Copyright, Certification of Approval, Abstract, Table of Contents, List of Figures, etc.), the first couple pages of your first
chapter, and examples of figures, tables and appendices.
2) Bring all this to the Grad Office (ADM 254) to have them do a preliminary format check (you can just drop by).
3) After this first format check, make necessary changes instructed by the format check reviewer. 
4) Do not print your thesis on "thesis paper" (e.g., at Rapid Copy, in Cesar Chavez or the Bookstore) until instructed by the format check reviewer and verbally approved by your
thesis committee.
5) Get signatures from your committee members on the "Certification of Approval" page and by your committee chair on the "Abstract" page on that good copy.
6) Bring the entire unbound thesis to the Grad Office.  
    a) They re-verify proper formatting, correct thesis paper and original signatures.  
    b) If not ok, they'll send it back to you, you'll have to fix things, re-print, get signatures, and re-submit.  
    c) Once everything looks good, they'll give you the thesis back, along with a signed thesis receipt.  
7) Bring the thesis, thesis receipt, and (if applicable) CD's of code in individual paper CD sleeves, to Rapid Copy (2nd floor of Cesar Chavez, Room 110).   
    a) They print & bind all your copies (pay appropriate binding fees).  You'll need to print one copy for the library, possibly one for your department, your adviser, your grandmother, etc.  
    b) Rapid Copy will provide you with a receipt to keep for your records and will send a receipt directly back to the Grad Office to verify that you've turned in your thesis. Keep your Thesis Receipt until you receive official verification from the Division of Graduate Studies that you have earned your degree.  
    c) Once the copies are printed & bound, Rapid Copy will contact you to pick them up.  
8) Distribute the copies to all the people above.
