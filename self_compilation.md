## Authorea to AMS LaTeX

Export the LaTeX file and put it in the same directory as:  
* Figures  
* Bibtex file  
* ametsoc.cls  
* ametsoc2014.bst  

Update minor aspects of the LaTeX file:  
* Change journal to jcli  
* Fix affiliation  
* Make sure title isn't too long on one line  
* Move bibliography reference down to end of document and and remove .bib file ending  
* Put figures in correct location and remove relative path  
* Any subsections that are the only subsection of their section need to use a *  

```
\authors{Damien Irving\correspondingauthor{Damien Irving, 
School of Earth Sciences, University of Melbourne, Victoria, Australia.}
and Ian Simmonds}

%% Follow this form:
    % \affiliation{American Meteorological Society, 
    % Boston, Massachusetts.}

\affiliation{School of Earth Sciences, University of Melbourne, Victoria, Australia.}

%% Follow this form:
    %\email{latex@ametsoc.org}

\email{irving.damien@gmail.com}
```  

Common errors:  
* Can't have paragraphs in the abstract   
* If the abstract is too long (i.e. > 250 words) it will leave a blank page under the header  
* Title can't be too long on one line (hit return to break up)  

Reference issues:  
* Must use the official abbreviations here: http://cassi.cas.org/search.jsp  
* Journals like Geophys. Res. Lett. have an eid field instead of pages   
* Don't include the following fields or else they'll show up when they shouldn't:  
  * URL  
  * Issue number  