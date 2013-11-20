Research Level Classifier
==========

Predict research level from text: http://www.sciencedirect.com/science/article/pii/S1751157713000825

Installing
----------

It may be easiest to run this from a Python virtual environment (https://pypi.python.org/pypi/virtualenv)

To install the Python dependencies:

    $ pip install -r requirements.txt
    
Running
-------

Input files should be tab-delimited text files with three columns: id, title, abstract.
A sample input file `data/sample-data.txt` is included.

You should be able to run the classifier like this:

    $ python rlev_model.py data/sample-data.txt > output.txt
    
Output is written to `stdout` and is tab-delimited text with 5 columns: id, prob1, prob2, prob3, prob4.
Here prob1 is the probability that the document belongs to research-level 1, and so on.
