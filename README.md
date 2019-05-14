# MAThesisTemplate
LaTeX files for MA theses at San Francisco State University
[Version 1.2 --- May 11th 2019]
## Contents
This archive contains the following files:
```
abstract.tex
acknowledgements.tex
content.tex <--- Actual content, or chapters with links to subfiles.
intrograph.pdf
MAThesisOutputFormat.sty
README.md
sfsuthesis.cls
thesis.bib <--- BibLaTeX references go here
thesis.tex <--- Compile this for formatting
```
## Instructions

* Copy all of the files in the same directory. You may do this also by pulling directly from the github.

* ```thesis.tex``` is the "mother file," which calls up the other files. LaTeX should compile this file. There are two modes: draft-editing and final version. The draft mode produces single-spaced output with 1-inch margins and a simple title page. The final-version mode produces an output that should be acceptable to the Graduate Division: double spacing, the right margins, copyright, signatures, abstract, acknowledgment pages, table of content, list of figures, etc. You can switch between both modes by going to line 21 in ```thesis.tex``` from

```\usepackage[draft]{MAThesisOutputFormat} ``` to ```\usepackage[final]{MAThesisOutputFormat}```

Custom definitions and packages should be made and included in thesis.tex, so that they will be useable in both modes. For running the ```final``` mode, you will need the tocloft package, which might not be installed by default in your TeX distribution. If it isn't google 'tocloft' (the current website is http://www.ctan.org/tex-archive/help/Catalogue/entries/tocloft.html).

* ```MAThesisOutputFormat.sty``` contains the TeX formatting for the draft-editing and final mode. In principle, you shouldn't have to alter this file. This file also contains the TeX formatting for the final version and the front matter for the final thesis. It uses sfsuthesis.cls as the class file. Some data (committee names, abstract, acknowledgments, etc.) has to be included into this file, but you shouldn't have to alter the layout definitions. One possible exception is the margins, since they can depend on the printer you're using. If they are off, the problem is most likely the text height; try changing the number in the line ```\textheight=7.1in``` of the file.

* ```content.tex``` will eventually contain the main body of your thesis, starting with Chapter 1. For now, this file contains various tips and tricks about LaTeX (which you will delete once you're ready for your thesis). The file intrograph.pdf is needed to produce the figures in this sample file. You can delete this file once you're working on your own text. I strongly recommend using content.tex to outline your work using ```\chapter{name}``` or ```\section{name}``` commands, and use ```\input{file}``` to call upon files, so that when you can compartmentalize your code. 

* ```thesis.bib``` contains the bibliography entries (which can be obtained from databases such as MathSciNet). Run LaTeX, BibTeX, LaTeX on thesis.tex to produce the bibliography.

* ```abstract.tex``` contains the abstract section - simply leave this file empty if you do not wish to have an abstract.

* ```acknowledgements.tex``` contains the optional acknowledgments section - simply leave this file empty if you do not wish to give acknowledgements.

For comments, problems, or suggestions, please contact Dr. Matthias Beck (```mattbeck AT sfsu.edu```).


## Filing the Thesis
Postscript: Here is an "algorithm" how to file your thesis (Updated Spring 2019):
1. Preliminary format check (ADM 254): 
    1. Print out all of your "preamble" pages (Cover Page, Copyright, Certification of Approval, Abstract, Table of Contents, List of Figures, etc.), the first couple pages of your first chapter, and examples of figures, tables and appendices.  
    2. Bring all this to the Grad Office (ADM 254) to have them do a preliminary format check (you can just drop by).   
    3. Make necessary changes instructed by the format check reviewer.    
    4. Do not print your thesis on "thesis paper" (e.g., at Rapid Copy, in Cesar Chavez or the Bookstore) until instructed by the format check reviewer and verbally approved by your thesis committee.
2. Immediately after your defense:
    1. Obtain signatures from your committee members on the "Certification of Approval" page,
    2. Obtain signature from your committee chair on the "Abstract" page.
    3. Obtain signature from your committee chair on the Thesis Receipt (given at the preliminary format check), and complete the Public Access/Embargo section.
3. Final format check (ADM 254):   
    1. Graduate Studies will re-verify proper formatting and original signatures. Bring your final printed copy for this step.
    2. If the formatting is not acceptable, then they'll send it back to you, you'll have to fix the formatting, re-print, get signatures, and re-submit.  
    3. Once everything looks good, they'll give you the thesis back, along with a signed thesis receipt.
    * If your thesis committee changed, submit a petition for committee revision, found on the Graduate Studies website.
4. Binding Fee + Submission (Bursur's Office + Library Room 80):
    1. Bring the thesis down to the Bursur's Office on the first floor of the Administration building, and keep the receipt as proof of payment. 
    2. Take your unbound thesis and proof of payment to the Digital Scholarship Center.
    3. Maintain your copy of the Thesis Receipt until you receive confirmation from the university that you have earned your degree.
    * If you took an extended semester with a grace period, be sure to submit petition to change grade for your thesis course (898) from ```RP``` to  ```CR```. 




















