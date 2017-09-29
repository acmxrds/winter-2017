# Identifying Hate Speech in Social Media

**Alexandra Schofield and Thomas Davidson \
Winter 2017**

*Hate speech* refers to language negatively targeting people based upon their affinity group. Though it is demonstrably present in social media, defining it in a way specific enough to filter it can prove challenging.

In this article, we provide a brief Python tutorial of how to build a classifier to distinguish tweets containing hate speech from other tweets using standard text classification techniques. This demonstration also shows some of why identifying hate speech can be challenging and subjective.

Installing Python and Jupyter
----------

We use an Jupyter Notebook written in Python 3 in our tutorial. If you have not installed Python 3, a convenient way to do so is using [Anaconda](https://www.anaconda.com/download/), which will install Jupyter as well. If you already have Python 3 installed, you can install Jupyter in the command line using `pip`.

```
$ pip3 install jupyter
```

If you want to use Python 2, you will need to alter the print statements so they use spacing instead of parentheses, e.g.

```
# Python 3 line
print("Hello, world!")
# Python 2 line
print "Hello, world!"
```

### Other packages
This notebook uses several other Python packages: `nltk`, `numpy`, `pandas`, and `scikit-learn`. All of these may be installed using `conda` if you are using Python via Anaconda:

```
$ conda install nltk
```

If using an alternate version of Python 3, use `pip`:

```
$ pip3 install nltk
```


Running the notebook
--------

To run Jupyter, open a command line window, navigate to the directory containing this IPython notebook, and run

```
$ jupyter notebook
```

[Identifying Hate Speech in Social Media]: #