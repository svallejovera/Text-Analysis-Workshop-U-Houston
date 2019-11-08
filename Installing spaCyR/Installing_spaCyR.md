Installing spaCyR
-----------------

There are a number of computational tools we can use for text analysis.
We will be working with the spaCyR and quanteda packages. spaCyR is an

> R wrapper to the spaCy \`\`industrial strength natural language
> processing'' Python library from <http://spacy.io>.

As such, you need to first install Pynthon in your computer, then
install spaCy for Python, and then install spacyR in R to link back to
the Python library.

### Installing spacyR in Windows

**The instructions to install spacyR in Windows can be found
[here](https://github.com/quanteda/spacyr/blob/master/inst/doc/WINDOWS.md)**

*Sorry Windows users, I am not familiar with that operating system and
have not installed spaCyR in Windows before. It is not a straightforward
process so you should follow closely the instructions.*

### Installing spacyR in Mac

*The instructions to install spaCyR for Mac are taken almost verbatim
from
[here](https://github.com/quanteda/spacyr/blob/master/inst/doc/MAC.md)*

1.  Install x-code from the Terminal

        xcode-select --install

2.  Install Homebrew from the Terminal

        /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

3.  Install Python3 from the Terminal

        brew install python3

    *Note: if you already have installed Python in your computer, check
    the path where it is installed. You can do that by typing in
    Terminal:*

        which python3

    *The output should look like this `/usr/local/bin/python3`. If
    Python is not installed in that path (if you installed Python
    through Anaconda or Miniconda) then you will have problems running
    spaCyR. spaCyR uses the path `/usr/local/bin/python3` as default to
    call Python, and manually specifying an alternative path can give
    you problems. The best alternative is to install another Python3 on
    that path.*

4.  Setup pip3 in Terminal

        pip3 install --upgrade setuptools
        pip3 install --upgrade pip3

5.  Install spaCy in Terminal

        pip3 install -U spacy

6.  Install the English language model

        python3 -m spacy download en

    \*Note: spaCy supports many beautiful languages trained through
    different algorithms. A full list can be found
    [here](https://spacy.io/usage/models). To download the language of
    Cervantes, for example, you can run

        python3 -m spacy download es

7.  Check that the installation succeeded in Terminal

        python3 -c "import spacy; spacy.load('en'); print('OK')"

8.  Install spaCyR in R

        install.packages("spacyr")

9.  Check that all is working properly (in R)

        library("spacyr") 
        spacy_initialize(model = "en")
