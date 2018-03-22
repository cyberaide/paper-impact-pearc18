paper-tas
======================================================================

mkdir cyberaide
cd cyberaide
git clone git@github.com:cyberaide/tex.git
git clone git@github.com:cyberaide/bib.git
git clone git@github.com:cyberaide/paper-tas-2.git
ln ../bib bib
ln ../tex tex


Adding Bibs
----------------------------------------------------------------------

::

  cd bib 

Use jabref to open and add refernces. Than do ::

  git commit -a 

and do the usual git tuff::

  git push

If everything is ok do::

  cd ..

You should be back in the paper dir


Creating the paper
--------------------

::

  make

View The paper
----------------------------------------------------------------------

:: 

  make view

Clean
----------------------------------------------------------------------

::
  
  make clean
