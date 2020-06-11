1. While installing TeXLive from the '[website](https://www.tug.org/texlive/doc/texlive-en/texlive-en.html#installation)', select to create symlinks in standard directories, this is not checked by default. In case you did not do it, like me, you will have to add symbolic paths.
2. I was able to access tlmgr as a normal user but not as root
3. tlmgr has to be accessed as su to install classes
4. The problem can be resolved like following as described [here](https://github.com/scottkosty/install-tl-ubuntu/issues/13)
  0. In case you do not already have perl-tk, install it `sudo apt-get install perl-tk`. This is needed to use tlmgr in gui mode
	1. do `which tlmgr` this will give you the path to tlmgr
  2. check whether it is part of your root user's PATH by `sudo env | grep ^PATH`
  3. If it is then this is not the solution for you, look elsewhere. If it is not, direct the su PATH to this PATH and open tlmgr in gui mode `sudo -E env "PATH=$PATH" tlmgr -gui`.
  4. Go to 'Actions->Handle symlinks' and select 'Update symbolic links'
