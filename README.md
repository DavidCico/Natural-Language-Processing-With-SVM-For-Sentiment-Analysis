# Natural-Language-Processing-With-SVM-For-Sentiment-Analysis



<p align="justify"> There are a significant number of steps to carry out between viewing a text document on a web site and using its content as input to an automated trading strategy. In particular the following steps must be carried out:</p>

<ul>
    <li><p align="justify">Automate the download of multiple, continually generated articles from external sources at a potentially high throughput.</p></li>
    <li><p align="justify">Parse these documents for the relevant sections of text/information that require analysis, even if the format differs between documents.</p></li>
    <li><p align="justify">Convert arbitrarily long passages of text (over many possible languages) into a consistent data structure that can be understood by a classification system.</p></li>
    <li><p align="justify">Determine a set of groups (or labels) that each document will be a member of. Examples include “positive” and “negative” or “bullish” and “bearish”.</p></li>
    <li><p align="justify">Create a training corpus of documents that have known labels associated with them. For instance, a thousand financial articles may need tagging with the “bullish” or “bearish” labels.</p></li>
    <li><p align="justify">Train the classifier(s) on this corpus by means of a software library such as Scikit-Learn.</p></li>
    <li><p align="justify">Use the classifier to label new documents, in an automated, ongoing manner.</p></li>
    <li><p align="justify">Assess the “classification rate” and other associated performance metrics of the classifier.</p></li>
    <li><p align="justify">Integrate the classifier into an automated trading system, either by means of filtering other trade signals or generating new ones.</p></li>
    <li><p align="justify">Continually monitor the system and adjust it as necessary if its performance begins to degrade.</p></li>

<p align="justify">In this particular script we make use of a given dataset that already comes with its own provided labels. This will allow us to concentrate on the implementation of the classification pipeline, rather than spending a substantial amount of time obtaining and tagging documents. While beyond the scope of this study, it is possible to make use of Python libraries, such as <a href="https://scrapy.org/">ScraPy</a> and <a href="https://www.crummy.com/software/BeautifulSoup/">BeautifulSoup</a>, to automatically obtain many web-based articles and effectively extract their text-based data from the HTML making up the page data. Under the assumption that we have a document corpus that is pre-labelled (the process of which will be outlined below), we will begin by taking the training corpus and incorporating it into a Python data structure that is suitable for pre-processing and consumption via the classifier.</p>

## Getting Started

<p align="justify">These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.</p>

### Prerequisites

<p align="justify">You need Python 3.x to run the following code.  You can have multiple Python versions (2.x and 3.x) installed on the same system without problems. Python needs to be first installed then SciPy, and finally Seaborn as there are dependencies on packages.</p>

In Ubuntu, Mint and Debian you can install Python 3 like this:

    sudo apt-get install python3 python3-pip

Alongside Python, the SciPy packages are also required. In Ubuntu and Debian, the SciPy ecosystem can be installed by:

    sudo apt-get install python-numpy python-scipy python-matplotlib ipython ipython-notebook python-pandas python-sympy python-nose

Finally, the latest release of Seaborn visualization package, which can be installed with pip:
    
    pip install seaborn

For other Linux flavors, OS X and Windows, packages are available at:

http://www.python.org/getit/  
https://www.scipy.org/install.html  
https://seaborn.pydata.org/installing.html#installing


### File descriptions
<ul>
    <li>'<em>ETF_data</em>' which is a univariate time series of the price history of the ETF.</li>
    <li>'<em>Main.py</em>' which contains the main procedure, as well as the data pre-processing of the xlsx file 'ETF_data.xlsx'</li>
    <li>'<em>Monte_Carlo_GBM.py</em>' which contains the different algorithms used for comparison.</li>
<li><div align="justify">'<em>Post_processing.py</em>' where all the functions for post-processing (plots, information, descriptive statistics) are implemented.</div></li>
<li><div align="justify">'<em>Analysis.pdf</em>', the PDF file where the different steps of the financial study are explained.</div></li>
</ul>

### Running the program

The different "<em>.py</em>" files need to be placed in the same folder for the main script to be run. The code is then ready to be used, and just requires running the following command:

    python Main.py

## Contributing

Please read [CONTRIBUTING.md](https://github.com/DavidCico/Natural-Language-Processing-With-SVM-For-Sentiment-Analysis/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **David Cicoria** - *Initial work* - [DavidCico](https://github.com/DavidCico)

See also the list of [contributors](https://github.com/DavidCico/Natural-Language-Processing-With-SVM-For-Sentiment-Analysis/graphs/contributors) who participated in this project.
