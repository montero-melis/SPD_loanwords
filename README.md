# General

This is a repository for Susanne V, Sigi V, and Guillermo MM's final project for the course in Semantics, Pragmatics and discourse.
The main file is `ProjectProposal.tex` which contains the actual proposal.
Other files containing data in text/csv format, or figures, might be included as well.
To translate a data set into tabular data for LaTeX we can use R, which contains some useful wrappers (checkout `xtable` package).

# LaTeX matters

- Quotation marks in LaTex: 
	- double quot marks = \`\`bla'' 
	- single quot marks =  \`bla'
	- see *quote marks* in `http://en.wikibooks.org/wiki/LaTeX/Text_Formatting#Quote-marks`
- To reference a section, figure, or even an item in a list, use the `\label{}` command, then reference it with the `\ref{}` command

# Export references from Zotero to BibTeX

Let's use the shared Zotero library "SPD project" to export our references.
This will avoid having twice the same reference with slightly different formatting.
Everytime we want to export we do that directly from this shared library:

1. Select all items
1. Right click on them
1. Choose "Export selected items"

There might be some problem with the character encoding when you export Zotero entries to BibTex format.
What seems to solve this is the following:

1. Go to Zotero > Preferences > Export 
1. Under `character encoding` check the option "Display character encoding option on export"
1. Now when you export into BibTex format select the character encoding "English (US-ASCII)"
