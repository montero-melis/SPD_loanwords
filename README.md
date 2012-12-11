# General

This is a repository for Susanne V, Sigi V, and Guillermo MM's final project for the course in Semantics, Pragmatics and discourse.
The main file is `ProjectProposal.tex` which contains the actual proposal.
Other files containing data in text/csv format, or figures, might be included as well.
To translate a data set into tabular data for LaTeX we can use R, which contains some useful wrappers (checkout `xtable` package).

Blooh blaaah blèèèh blublublublubluh



LaTeX matters
=============


Things to avoid
---------------

Here's some stuff which caused problems when trying to compile the document. Avoid it!

- You have to escape special characters like
	- ampersands (write this: `\&`)
	- underscores `_`. If you wanted to use italics then use the `\emph{}` command
- Commands are case-sensitive so `\section{}` is fine but `\Section{}` isn't.



Useful stuff
------------

- Quotation marks in LaTex: 
	- double quot marks = \`\`bla'' 
	- single quot marks =  \`bla'
	- see *quote marks* in http://en.wikibooks.org/wiki/LaTeX/Text_Formatting#Quote-marks
- To reference a section, figure, or even an item in a list, use the `\label{}` command, then reference it with the `\ref{}` command in the text. See *Labels and Cross-referencing* at http://en.wikibooks.org/wiki/LaTeX/Labels_and_Cross-referencing





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
1. Under "character encoding" check the option "Display character encoding option on export"
1. Now when you export into BibTex format select the character encoding "English (US-ASCII)"



Collaborating with Git and GitHub
======================


Joining the git repo
--------------------

The repo we’re working with has the following url:
https://github.com/montero-melis/SPD_loanwords

1. Guillermo adds you both as collaborators
2. Clone the repo into your computer. To do that use `git clone https://github.com/montero-melis/SPD_loanwords.git` or `git clone git@github.com:montero-melis/SPD_loanwords.git`. If you use a GUI there’ll be some corresponding command.


Everyday work
-------------

We’ll be all working on the same branch (master), so we will NOT use forking (NB Sigva!).
The `git clone` command makes sure that your local repository syncs with the master branch at GitHub, so in practice you only need to do two things.

1. Commit changes with `git commit` (after adding them with `git add .` or `git add -A`)
1. If you're using the Git Bash and you end up in the unfriendly Vi editor, then: write your commit message on the first line. Then click `Esc`, then type `:wq!`. Ok, the commit is done! (Ignore this point if you're using the GUI)
1. Make sure you have the last changes made to master. You do this by pulling from master (`git pull`)
1. Now you can push your last changes to the master branch at GitHub with `git push`.

Now, it may happen that someone else in the meantime has made some changes to a file that are incompatible with the changes you have made to the same file (NB: Git is rather smart at detecting when these changes really are incompatible).
In that case you will be prompted to resolve the conflicts manually when you pull.
Here’s how you do it:

1. Open the file that causes the conflict.
2. Make the appropriate changes, that is, open the file, and remove the parts that you don’t want, i.e. manually erase the part of the document that is unwanted, or combine the documents in a way that is satisfying. (Check out this link: http://www.kernel.org/pub/software/scm/git/docs/v1.7.3/user-manual.html#resolving-a-merge)
3. If you aren’t sure how to resolve the conflict then you e-mail or phone the person that has made the changes and you agree on a solution.
4. Once the conflict has been resolved, push the new version to master (`git push`).


This is pretty much it.

Remember: *We’ll try to avoid using branches!*

