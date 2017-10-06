# Reproducible and Interactive Data Science

## Syllabus

The aim of this course is to introduce students to the [Jupyter Notebook](http://jupyter.org) which
is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, machine learning and much more. Through the notebooks, research results and the underlying analysis can be transparently reproduced as well as shared.
As an example of a Notebook on gravitational waves published in _Phys. Rev. Lett._, see [here.](http://nbviewer.jupyter.org/github/minrk/ligo-binder/blob/master/index.ipynb)

During three days with alternating lectures and hands-on exercises, the participants will learn to construct well-documented, electronic notebooks that perform advanced data analysis and produce publication ready plots.
While the course is based on Python, this is not a prerequisite, and many [other programming languages](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels) can be used.

## Credits

4 ECTS.

## Program

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
  - Calling C/C++/fortran routines; Cython.
  - Interfacing with clusters (LUNARC)

- Day 4. Project presentations

## Prerequisites

- No prior knowledge in Python is required, but familiarity with programming concepts is helpful.
- A laptop running Unix, MacOS, or Windows

If you have little experience with Python or shell programming, the following two tutorials may be helpful:

- https://swcarpentry.github.io/shell-novice
- https://swcarpentry.github.io/python-novice-inflammation


## Preparations before the first lecture

1. Install [Anaconda 3.x](https://www.anaconda.com/download) on your laptop.
2. Using Anaconda, install and activate the `LUcompute` environment described by the file [`environment.yml`](/environment.yml) by running the following in a terminal:

   ```bash
   conda env create -f environment.yml
   source activate LUcompute
   ```
   (See instructions for Windows [here](https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file)).

## Evaluation

The evaluation consists of three steps:

1. Each student will make a Notebook project covering topics from day 1-3 with either

  - research, presenting data analysis and theory behind
    a manuscript or published paper. The Notebook should be written
    such that it can act as supporting information (SI) for a journal.
    Here's some [inspiration.](http://nbviewer.jupyter.org/github/jansoe/FUImaging/blob/master/examples/IOSsegmentation/regNMF.ipynb)
   
  - _or_ a Notebook presenting a text-book topic of choice and aimed at students.
    The notebook should include rich documentation, use interactive graphs, and
    numerical methods. Here's some [inspiration](http://nbviewer.jupyter.org/github/demotu/BMC/blob/master/notebooks/Transformation2D.ipynb).

2. A peer-review process where each student reviews and comments on two other notebooks.

3. Notebook presentation to the class (day 4)
