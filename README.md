# Lab_Protocols

This repository contains Whitehead Lab laboratory protocols. 

Update as protocols change.

All protocols should be written in markdown- github flavored markdown is a good choice. 

## Options for writing in markdown  

this is just a sampling. Many people do many things....

1. Plain text editor
	- for example, Sublime text, Atom, text wrangler, etc.
	- Atom
		+ has built in markdown preview (access using ctl+m)
	- sublime text
		+ can install packages that allow for markdown previewing
	- Atom and sublime text have syntax highlighting, not sure about text wrangler

2. markdown text editor
	- mou, mac down.
	- Instantaneously preview your markdown file

3. Plain text editor + grip
	- My current preferred choice bc it previews in github flavored markdown
	- can preview your md file as html in browser (automatically updates when you save).
	- then can print to pdf and/or actually print
	- Preview file with grip
		+ `grip -b FILEPATH`
	- Save to html
		+ `grip FILEPATH --export optionalname.html`

4. plain editor + pandoc
	- pandoc can be used to md convert to html, pdf, etc.
	- `pandoc -o output.html input.md`

