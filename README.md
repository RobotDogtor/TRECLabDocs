TRECLabDocs

**Installation**
Start by installing Python and the Sphinx package on your computer. (Follow: https://www.sphinx-doc.org/en/master/usage/installation.html)

Best quickstart to understand sphinx is (https://www.sphinx-doc.org/en/master/usage/quickstart.html)

Just create a folder anywhere you want called "ProjectName". Navigate into the folder and run 'sphinx-quickstart'.
Then run 'make html'
then select "..ProjectNameDirectory/build/html/index.html" to open docs


**Docs Structure**
The "..ProjectNameDirectory/source/index.rst" contains the toplevel structure for the documentation
If you add something to the toctree, be sure to actually add the directory architecture and files to the source folder


**Conf.py**
This contains the Configuration details for this read the docs build.