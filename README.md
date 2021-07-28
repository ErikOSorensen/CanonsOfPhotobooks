# Canons of photobooks

The ambition is to create a database of photobooks that are referenced
in at least one of the attempts to create canons of great photobooks. 
This development is widely recognized to have started with Andrew Roth's 
*The Book of 101 Books* in 2001, and the Hasselblad Center's *The Open Book*
in 2004, but of course the broadest and probably most impactful surveys are 
the three volumes of Parr and Badger (2004, 2006, 2014). There are other 
global survey (such as the collection survey from the Auer collection published by 
Editions M+M), and a whole slew of surveys that are specific to geographical 
regions or time periods. My intention is to cover the surveys that are readily
available to me (starting with my home library).

The plan for entering data is to start with the Auer
collection book since it provides the easiest access to bibliographic data (standardized to one book per page).

# Organization of data

The plan is to organize one master bibliographic database (in `Biblatex` format) 
and then create separate files of references to these, one for each survey, with
reference to the bibliography and other fields that might be specific to each
survey. The Bibtex data can be processed fairly easily, the separate file of references
will be plain text files (.csv). 

## Comments on the Bib fields

- **author** The Biblatex database will typically reference the photographer as the *author* for
standard monographs. In some cases, there will instead be one or more editors listed
as the main creators of the book (in which case the *author* field will be empty). 
- **year** This will be the year of the first edition.
- **location** This will in some cases be the city, country, or city and state. In some cases there won't be such information, but at the end of the address field there will always be a semi-colon delimiter and a 3-letter ISO code for the country of origin. 
- **bibtexkey** Lastname of the (first) author/editor (all last names squashed together) and the year of publication (such as `Daguerre1839`).

