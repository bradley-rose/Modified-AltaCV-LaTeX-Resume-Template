# Modified AltaCV LaTeX Resume Template

## Explanation
This is a resume template built using the [AltaCV](https://www.overleaf.com/latex/templates/altacv-template/trgqjpwnmtgv) resume template. I've modified this to work better with most Application Tracking Systems. The original AltaCV format looks excellent, but there's two critical issues:  

1. ATS have a really tough time interpreting two columns, and will often incorrectly parse data making the resume pointless. Getting past the ATS is the most important step of a resume.
2. Graphics are impossible to run through ATS as well. Again, most of the graphics are removed apart from small ones based on unicode for contact information and applicant details. These obviously don't get translated well through ATS, but they don't cause enough of an issue that removing them makes a difference. I still like the look of them, so I've kept them assuming that they'll be looked at once they pass through ATS.

## Basic Usage
Open the `resume.tex` file and edit the appropriate sections. The file is commented out to explain all of the specifics of editing the file, with one key exception that I wanted to lay out clearly here: 

The `altacv.cls` file has had its `\newcommand{\cvevent}` customized to make the final PDF more compact. The accent colours still do a good job at separating the subtext where required, so it's not too much of an issue. If you would prefer the original AltaCV layout, I've left the original code in `altacv.cls` immediately below the modifications just commented out. Delete the active code block and uncomment the original code to return it to it's original format.

## Compiling
Once you've completed making your edits, compile the `resume.tex` file with your LaTeX compiler of choice. I've been utilizing `pdflatex` quite happily, but I know there are alternative preferences. In it's current state, the following command will generate the appropriate template PDF:  
> `pdflatex resume.tex`  

## Troubleshooting
Note the original [AltaCV](https://www.overleaf.com/latex/templates/altacv-template/trgqjpwnmtgv) documentation for any class modifications.