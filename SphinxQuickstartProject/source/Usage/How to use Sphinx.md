TRECLabDocs

***Installation***
**Windows:**
Start by installing Python and the Sphinx package on your computer. (Follow: https://www.sphinx-doc.org/en/master/usage/installation.html)
Can install python from https://www.python.org/, select custom installation and check "add python to environment valiables" and "install for all users"
Then 'pip install -U sphinx'
Also 'pip install myst-parser' to install a markdown processor for sphinx

Packages located in c:\users\ben beiter\appdata\roaming\python\python39\site-packages

Best quickstart to understand sphinx is (https://www.sphinx-doc.org/en/master/usage/quickstart.html)

Just create a folder anywhere you want called "ProjectName". Navigate into the folder and run 'sphinx-quickstart'.
Then run 'make html' 
then select "..ProjectNameDirectory/build/html/index.html" to open docs
'make latex' will generate a pdf for you 

really you want to run the sphinx-build program: 'sphinx-build -b html sourcedir builddir'
but the quickStart creates a make.bat file that will run this command for you

**Docs Structure**
The "..ProjectNameDirectory/source/index.rst" contains the toplevel structure for the documentation
If you add something to the toctree, be sure to actually add the directory architecture and files to the source folder
Files can be text files (.txt), markdown (.md), or reStructuredText (.rst)

**Conf.py**
This contains the Configuration details for this read the docs build.

Important:

# Add any Sphinx extension module names here, as strings. They can be
# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
# ones.
extensions = ['myst_parser']

# Source Files Recognized by Sphinx
source_suffix = {
    '.rst': 'restructuredtext',
    '.txt': 'restructuredtext',
    '.md': 'markdown',
}








https://readthedocs.org/
https://docs.readthedocs.io/en/stable/development/install.html
https://docs.readthedocs.io/en/stable/versions.html
https://www.sphinx-doc.org/en/master/tutorial/index.html#structuring-your-documentation-across-multiple-pages
https://www.sphinx-doc.org/en/master/usage/theming.html
https://www.sphinx-doc.org/en/master/templating.html#templating
https://www.writethedocs.org/guide/writing/beginners-guide-to-docs/
https://holzhaus.github.io/sphinx-multiversion/master/index.html
