# Introduction to Text Analysis Workshop 

Text-analysis is a heavily computer-dependent task. As such, this introduction will be an applied approach of text-analysis through the use of **quanteda** and **spaCyR**, two R packages used for content and text analysis. To take full advantage of the workshop, it is recommended that attendees have a working knowledge of R (but all are welcome!).  

We will learn the basic three-step process needed to set up research based on text: 1) creating a corpus from texts, 2) extracting quantitative features from the corpus into a matrix, and 3) using statistical methods to analyze this matrix and make inferences about the texts or the authors of the texts. 

Text-analysis opens the possibility to analyze a range of data that is plentiful and readily available, especially in politics. Politicians LOVE to speak. Bureaucrats LOVE to type. And we LOVE data. While computer-intensive, text-analysis is intuitive and, let's be honest, everybody loves a word cloud.<sup id="a1">[1](#f1)</sup> 

**The .Rmd (R Markdown), .htlm, and .pdf files for the complete workshop can be [found here](https://github.com/vallejo086/Text-Analysis-Workshop-U-Houston/tree/master/Workshop).**

  - [Instructions to install the required software](#instructions-to-install-the-required-software)
    - [quanteda (for R)](#quanteda-for-r)
    - [spaCyR (for R)](#spacyr-for-r)
    - [Extra packages](#extra-packages)
  - [Some final words](#some-final-words)
  
## Instructions to install the required software

From the [quanteda](https://tutorials.quanteda.io) homepage:

> **quanteda** runs solely on [base R](https://cran.r-project.org), but [RStudio](https://www.rstudio.com/products/rstudio/download/) makes it easy to write your code and inspect your objects. You will need to have base R installed, and we also recommend to install the latest version of RStudio.

### quanteda (for R)

First, you need to have **quanteda** installed. You can do this from inside RStudio, from the Tools > Install Packages, or executing a command.

```
install.packages("quanteda")
```

Note that on **Windows** platforms, it is also recommended that you install the [RTools suite](https://cran.r-project.org/bin/windows/Rtools/), and for **OS X** that you install [XCode](https://apps.apple.com/gb/app/xcode/id497799835?mt=12) from the App Store.

### spaCyR (for R)

The instructions for installing spaCyR can be found [here](https://github.com/vallejo086/Text-Analysis-Workshop-U-Houston/blob/master/Installing%20spaCyR/Installing_spaCyR.md).

### Extra packages

We will also use the *readtext* package to read in different types of text data in this tutorial. Again, you can do this using RStudio menu (Tools > Install Packages), or executing the following command.

```
install.packages("readtext")
```

If we have enought time left, we will explore a semi-supervised model to classify documents called Newsmap. You can download the pacakge from CRAN.

```
install.packages("newsmap")   
```

To make things look pretty, we will use the *ggplot2* package that can be installed directly from inside Rstudio, from the Tools > Install Packages, or executing a command.

```
install.packages("ggplot2")
```

Finally, [stringr](https://cran.r-project.org/web/packages/stringr/vignettes/stringr.html) is a great and handy package when it comes to dealing with character variables, something you will be doing often when handling text data. I have uploaded a [reference guide](https://github.com/vallejo086/Text-Analysis-Workshop-U-Houston/blob/master/Sanchez%20(2013)%20-%20Handling%20and%20Processing%20Strings%20in%20R.pdf) by Gastón Sánchez. He has a newer online version which you can check out [here](http://www.gastonsanchez.com/r4strings/). You can install *stringr* from inside RStudio, from the Tools > Install Packages, or executing a command.

```
install.packages("stringr")
```
## Some final words

As we get closer to the workshop, I will upload the dataset we will be using for the workshop. I will upload both the code I will use to create the dataset (in case you are interested in practicing your web scrapping) and the dataset itself (if you do not care about web scrapping). I will also make available all the code we will use in the workshop.   


> :warning: If you use the quanteda package in your research, please cite:
> Benoit, Kenneth, Kohei Watanabe, Haiyan Wang, Paul Nulty, Adam Obeng, Stefan Müller, and Akitaka Matsuo. 2018 “quanteda: An R package for the quantitative analysis of textual data.” Journal of Open Source Software 3(30), 774. https://doi.org/10.21105/joss.00774.


&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;

<b id="f1">1</b> Word clouds are silly. [↩](#a1)
