This repository contains analysis and science experiments regarding
[CALC][] data, mostly in the form of IPython/Jupyter notebooks.

## Reading the notebooks

If you only want to read the notebooks, you can actually just use
GitHub--look for the files ending in `.ipynb`. Here's a few to get
you started:

  * [Anomaly detection](contract-analysis/anomaly-detection.ipynb) can help us find invalid/incorrect data in CALC.

  * [Fun with CALC and pre-trained GloVe word embeddings](contract-analysis/glove_fun.ipynb) can help us perform _semantic_ search in CALC, e.g. searching for "tutor" and getting results like "Principal Instruction Technologist".

  * [Log analysis](log-analysis/log-analysis.ipynb) contains some open-ended exploration of CALC's API logs, to learn how people are using CALC (note that CALC's API is used by CALC's front page).

  * [Contract analysis](contract-analysis/contract-analysis.ipynb) contains open-ended exploration of CALC's contract data.

  * [SIN analysis](contract-analysis/sin-analysis.ipynb) attempts to parse and make sense of CALC's unstructured Special Item Number (SIN) data.

## Interacting with the notebooks

If you want to interactively explore the notebooks or create new ones,
you'll need to clone this repository locally.

This project's git repository uses [Git Large File Storage][git-lfs] to
store some of our large data assets. Please install it before cloning. (If
you've already cloned the repository, you can obtain the large files after
installing Git LFS by running `git lfs pull`.)

If you're familiar with virtualenvs and pip, you can use them
to install all dependencies:

```
virtualenv venv

# On Windows, replace the following line with 'venv\Scripts\activate'.
source venv/bin/activate

pip install -r requirements.txt
```

On the other hand, if you're not familiar with virtualenvs, you can
probably just install [Anaconda][], as it ships with most/all the
dependencies you'll need.

Once you've done either of those, just run `jupyter notebook` in the
root directory of the repository and use its web interface to explore
any of the notebooks.

[CALC]: https://github.com/18F/calc
[git-lfs]: https://git-lfs.github.com/
[Anaconda]: https://www.continuum.io/downloads
