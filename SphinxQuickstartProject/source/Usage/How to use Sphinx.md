TRECLabDocs

**Installation**
Start by installing Python and the Sphinx package on your computer. (Follow: https://www.sphinx-doc.org/en/master/usage/installation.html)
choco install sphinx
choco install python --pre

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
