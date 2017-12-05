# Reproducible and Interactive Data Science

## Syllabus

The aim of this course is to introduce students to the [Jupyter Notebook](http://jupyter.org) which
is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, machine learning and much more. Through the notebooks, research results and the underlying analysis can be transparently reproduced as well as shared.
As an example of a Notebook on gravitational waves published in _Phys. Rev. Lett._, see [here.](http://nbviewer.jupyter.org/github/minrk/ligo-binder/blob/master/index.ipynb)

During three days with alternating lectures and hands-on exercises, the participants will learn to construct well-documented, electronic notebooks that perform advanced data analysis and produce publication ready plots.
While the course is based on Python, this is not a prerequisite, and many [other programming languages](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels) can be used.

## Credits

4 ECTS.

## _Preliminary_ Program (final version available on Friday 8th of December)

_Lectures on **December 11, 14, 15 (2017)** and project presentations: **January 5th, 2018**_. All dates from 10:15 to 15:00.

The course consists of four full days: three with alternating lectures and hands-on exercises, and one day with project presentations.
Lectures are available as Notebooks on this site in the [lectures](lectures) folder.

- Day 1. Introduction
  - Introduction and overview of Jupyter notebooks
  - Installation and package management (Anaconda, managing environments)
  - Documenting using Markdown: rich text, equations, images, tables.
  - Other languages (bash, R, ruby, perl, etc.)
  - Online viewing, conversion, sharing, version control (Github, Binder, NBviewer, NBconvert, Zenodo)
  - Online resources and getting help
  - Calling C/C++/fortran routines; Cython.
  - Interfacing with clusters (LUNARC)
  
- Day 2. Plotting and visualization
  - Plotting in Notebooks (`matplotlib`, `seaborn`, `root`)
  - Arranging plots, customizing
  - Making plots publication ready
  - Exporting to vectorized file formats
  - Interactive visialization (`ipywidgets`, `bokeh`)
  
- Day 3. Numerical methods and data science
  - Numerical and scientific python (`numpy`, `scipy`)
  - Symbolic math (`sympy`)
  - Data parsing and import (csv, excel, json, pickle, pdf, custom files, etc.)
  - Working with large datasets (`pandas`)

- Day 4. Project presentations

## Prerequisites

- No prior knowledge in Python is required, but familiarity with programming concepts is helpful.
- A laptop running Unix, MacOS, or Windows and with Anaconda installed, see below.

If you have little experience with Python or shell programming, the following two tutorials may be helpful:

- https://swcarpentry.github.io/shell-novice
- https://swcarpentry.github.io/python-novice-inflammation


## Preparations before the first lecture

1. Install [miniconda3](https://conda.io/miniconda.html) alternatively the full [anaconda3](https://www.anaconda.com/download) enviroment on your laptop (the latter is **much** larger).
2. [Download](https://github.com/mlund/jupyter-course/archive/master.zip) the course material (this github repository) and unzip.
3. install and activate the `LUcompute` environment described by the file [`environment.yml`](/environment.yml) by running the following in a terminal:

   ```bash
   conda env create -f environment.yml
   source activate LUcompute
   jupyter nbextension enable rubberband/main
   jupyter nbextension enable exercise2/main
   ```
   (See instructions for Windows [here](https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file)).

## Project Work

The project work consists of three steps:

1. Each student will make a Notebook project covering topics from day 1-3 with either

  - research, presenting data analysis and theory behind
    a manuscript or published paper. The Notebook should ideally be written
    such that it can act as supporting information (SI) for a journal.
    Here's some [inspiration.](http://nbviewer.jupyter.org/github/jansoe/FUImaging/blob/master/examples/IOSsegmentation/regNMF.ipynb)
   
  - _or_ a Notebook presenting a text-book topic of choice and aimed at students.
    Here's some [inspiration](http://nbviewer.jupyter.org/github/demotu/BMC/blob/master/notebooks/Transformation2D.ipynb).

2. A peer-review process where each student reviews and comments on _two_ other notebooks. The review should be based on the criteria listed below and for each point, include specific suggestions for improvements. Please email your review to the notebook creator before day 4 and CC the instructors.
 
3. Notebook presentation to the class (day 4)

### Notebook Requirements

The project notebook _must_:

- [ ] contain name and contact information of the author
- [ ] include rich documentation using Markdown, equations, tables, links, etc.
- [ ] import or generate data. If generating, data should be exported to disk.
- [ ] perform data operations using `numpy`, `scipy`, `pandas` or equivalent.
- [ ] create plots of _publication ready_ quality. For an editorial guide on _Graphical Excellence_, see [here.](http://dx.doi.org/10/cg2g)
- [ ] include instructions on how to run the notebook, include the required packages. This could be an `environment.yml` file.

The project notebook _could_:

- [ ] be placed on github
- [ ] act as supporting information for an article
- [ ] have an digital object identifyer (DOI)
