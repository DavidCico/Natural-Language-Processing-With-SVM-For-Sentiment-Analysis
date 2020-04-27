# Natural-Language-Processing-With-SVM-For-Sentiment-Analysis



There are a significant number of steps to carry out between viewing a text document on a web
site and using its content as input to an automated trading strategy. In particular the following
steps must be carried out:
• Automate the download of multiple, continually generated articles from external sources at
a potentially high throughput
• Parse these documents for the relevant sections of text/information that require analysis,
even if the format differs between documents
• Convert arbitrarily long passages of text (over many possible languages) into a consistent
data structure that can be understood by a classification system
• Determine a set of groups (or labels) that each document will be a member of. Examples
include “positive” and “negative” or “bullish” and “bearish”
• Create a training corpus of documents that have known labels associated with them. For
instance, a thousand financial articles may need tagging with the “bullish” or “bearish”
labels

Train the classifier(s) on this corpus by means of a software library such as Scikit-Learn
(which we will be using below)
• Use the classifier to label new documents, in an automated, ongoing manner.
• Assess the “classification rate” and other associated performance metrics of the classifier
• Integrate the classifier into an automated trading system, either by means of filtering other
trade signals or generating new ones.
• Continually monitor the system and adjust it as necessary if its performance begins to
degrade
In this particular section we will avoid discussion of how to download multiple articles from
external sources and make use of a given dataset that already comes with its own provided labels.
This will allow us to concentrate on the implementation of the classification pipeline, rather than
spend a substantial amount of time obtaining and tagging documents.
While beyond the scope of this section, it is possible to make use of Python libraries, such
as ScraPy and BeautifulSoup, to automatically obtain many web-based articles and effectively
extract their text-based data from the HTML making up the page data.
Under the assumption that we have a document corpus that is pre-labelled (the process of
which will be outlined below), we will begin by taking the training corpus and incorporating it
into a Python data structure that is suitable for pre-processing and consumption via the classifier.
