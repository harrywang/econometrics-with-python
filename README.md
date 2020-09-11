# About
Python version of "Introduction to Econometrics with R" at https://www.econometrics-with-r.org/


## Setup

- Install Jupyter Book for the local user on Mac: `pip install -U jupyter-book`
- Generate the template book at the root of this project: `jupyter-book create econometrics-with-python`, the following structure is created:

```
.
├── README.md
└── econometrics-with-python
    ├── _config.yml
    ├── _toc.yml
    ├── content.md
    ├── intro.md
    ├── logo.png
    ├── markdown.md
    ├── notebooks.ipynb
    ├── references.bib
    └── requirements.txt
```

- `_config.yml`: all book configurations: define metadata for your book (such as its title), add a book logo, turn on different “interactive” buttons (such as a Binder button for pages built from a Jupyter Notebook), and more.
- `_toc.yml`: the table of contents

To run the code via virtual environment:
```
python3 -m venv venv
source venv/bin/activate
pip install -r econometrics-with-python/requirements.txt 
```
then you can open the notebooks using `jupyter notebook` or VSCode `code .`

## Build and Publish

To build the book: `jupyter-book build econometrics-with-python` to generate the `_build` folder with HTML version of the book.

Run `ghp-import -n -p -f econometrics-with-python/_build/html` at the root folder to push the HTML files to the `gh-pages` branch to publish the book, which can be accessed at http://harrywang.me/econometrics-with-python