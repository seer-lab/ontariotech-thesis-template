# A UOIT Thesis Template

This is a collaborate effort to establish a UOIT LaTeX thesis template. Currently this template is being created/maintained by M.Sc graduate students, which is why this template is geared towards them).

## Getting Started

It is highly recommended that you use a Unix based operating system.

As for actually editing your thesis you can use a LaTeX program (i.e., [TexMaker][1]) or simply any text editor.

With preference to a text editor you can use the awesome [latexmk][2] script to handle auto-compilation upon saving any part of your thesis. The following is how to invoke the script from command-line:

    latexmk -pdf -pvc -silent -r .latexmkrc thesis

The aforementioned command should be executed within the `src` directory of your thesis. This command will create a PDF of thesis every time you save any part of it. The `-r .latexmkrc` is required as this template makes use of the [glossaries][3] LaTeX package for handling abbreviations (it is required to run the `makeglossaries thesis` command between each compilation, which is automatically done now due to the configuration in `.latexmkrc`).

[1]: http://www.xm1math.net/texmaker/ "TexMaker"
[2]: http://www.phys.psu.edu/~collins/software/latexmk-jcc/ "latekmk"
[3]: http://www.ctan.org/tex-archive/macros/latex/contrib/glossaries "glossaries"
