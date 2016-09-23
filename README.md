# zhaw-templates
This repo contains LaTeX templates for zhaw documents.

## zhawreprt.cls
This is the documentclass for zhaw documents. It formats the document and loads the needed packages. There are two package options you should know about:
- `german`/`ngerman` or `english` - switches some predefined texts to the passed language.
- `final` - ignores all the notes written in the file. If this flag is not passed on to the package, the gray colored notes will be displayed in the pdf.

It also provides the user with new or modified commands such as:
- `\maketitle` - modified title page using the zhaw standard.
- `\makedeclarationoforiginality` - prints the language specific declaration of originality.
- `\printtheindex` - alternative to the original `\printindex` fixing the hierarchy of the index.
- `\nelistoffigures` and `\nelistoftables` - they only print the list if such labels exist in the first place.
- `\notes{...}` - print grey colored notes on the pdf. They disappear when the package option flag `final` was set.
- `\logofilename{...}` - sets the path of the desired logo. Browser the `./images/logos/` folder for all the possible logos.
- `\projecttype{...}` - either `PA`(project work) or `BA`(bachelor's thesis). Affects the title and the declaration of orginality.
- `\major{...}` - sets the name of the major.
- `\shorttitle{...}` - sets the short form of the title page to be used in the header.
- `\authors{...}` - sets the authors. Affects the title page.
- `\mainreferee{...}` - sets the main referee.
- `\referee{...}` - sets the referee.
- `\industrypartner{...}` - sets the industry partner.
- `\extreferee{...}` - sets the external referee.
- `\setdate{...}` - sets the date to be displayed.

## zhawDocument.tex
This is the document of interest. It basically holds all the documentation for the project in it. Parts that are not needed can easily be commented out.

## zhawFunctionalSpecificationDocument.tex
This document provides basic commands to build up the functional specifications(FSD).

## zhawGanttDiagram.tex
This here provides a template for a Gantt diagram.

## zhawNetworkPlan.tex
The network plan is the following step after the FSD.
