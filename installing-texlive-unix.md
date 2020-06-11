### Installing TeX in Unix
Install TeXLive(TL) by downloading the installation package from the TL website instead of doing `apt-get install`. This way one can avoid running into problems like [this](https://github.com/termux/termux-packages/issues/5167)


In case you are reinstalling or reattempting a failed installation, clean up everything. [See here for how to](https://tex.stackexchange.com/a/95502)


Download the software from the website. [Link to the page](https://www.tug.org/texlive/acquire-netinstall.html)


Once you have the software and have unpacked it, cd to the directory, e.g. in my case, I downloded and unpacked it in Downloads, 


```
cd /Download/<install-tl-somenumbers>
perl install-tl
```

if you click i, TL is installed with the default options. In the submenus, one can instead select the specific packages one wants to install. The TL scheme menu is set to *full scheme (everything)* by default. It is advisable to install the *basic scheme(plain and latex)* only. For example most of us do not need the support that TL provides for various languages. The choice can be further refined using the *collections* menu. tlmgr can be used to install, extra packages as you go about using TL.


In the *Options customization*, creating symlinks is unselect by default, select this, this avoids having to manually add PATH to the directories.


click `i`


If you did not click to add symlinks during the installation, do so manually by adding the following lines to `/.profile`


```
vim ~/.profile
PATH=/usr/local/texlive/2020/bin/x86_64-linux:$PATH; export PATH
MANPATH=/usr/local/texlive/2020/texmf-dist/doc/man:$MANPATH; export MANPATH
INFOPATH=/usr/local/texlive/2020/texmf-dist/doc/info:$INFOPATH; export INFOPATH
```

Test the installation
`tex --version` should give you information about the TL installed in your system, if it does not, there is a problem with the PATH defined for the user.


`latex sample2e.tex` should generate a log file
`xdvi sample2e.dvi` can be used to preview the file generated
`dvips sample2e.dvi -o sample2e.ps` is for generating a ps file for printing
`pdflatex sample2e.tex` generates the pdf file


REVTeX, the macro maintained by APS uses XeTeX, in case you have installed the xetex package, check by doing
`xetex opentype-info.tex`


#### Installing additional packages ####
If and when you get an error `blabla.cls not found` or `blabla.sty not found`, blabla being a package name, it can be installed using tlmgr


check whether the package is installed
`tlmgr show blabla`
if it says, installed:no
`tlmgr install blabla`
You may also have to update tlmgr, `tlmgr update self`


Reference
1. [The TeX Live Guide—2020](https://www.tug.org/texlive/doc/texlive-en/texlive-en.html#x1-380003.5)
2. [tlmgr - TeX Live package manager](https://tug.org/texlive/tlmgr.html)
