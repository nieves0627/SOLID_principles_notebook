# SOLID Principles Notes

This project is designed to take notes for a course using Jupyter notebooks and publish them using GitHub Pages. It utilizes the `ghp-import` library for deployment and Poetry for managing dependencies.

## Description
Notes for SOLID Principles course
## Installation

To get started, you'll need to install Poetry, which will help manage your dependencies:

1. **Install Poetry**: Follow the installation instructions from the [Poetry website](https://python-poetry.org/docs/#installation).

2. **Clone the repository**:

```bash
   git clone https://github.com/nieves0627/SOLID_principles_notebook
   cd PEP8_and_style_conventions_notebook
```
3. Install dependencies:
```bash
   poetry install
```
This command will install all necessary dependencies specified in the `pyproject.toml` file, including `ghp-import` and `Jupyter`.

## Usage
### Create Notes
1. Start Jupyter Notebook:
```bash
poetry run jupyter notebook
```
This will open the Jupyter Notebook interface in your web browser. You can create new notebooks to take notes.

## Build and Publish
Once you've created your notes, you can publish them to GitHub Pages:
1. Build the site:
```bash
 poetry run jupyter-book build ./solid_principles_notebook
```
 2. Import to GitHub Pages:
 Use `ghp-import` to publish the content to the `gh-pages` branch:
 ```bash
 poetry run ghp-import -n -p -f ./solid_principles_notebook/_build/html
 ```
 The -n flag prevents creating a new repository if it doesn't exist, -p pushes the changes to GitHub, and -f forces overwriting any existing files.

 ## Access Your Notes
 After publishing, your notes will be available at:
 ```bash
https://github.com/nieves0627/SOLID_principles_notebook
```