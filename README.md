[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/mlund/jupyter-course/master)

# Reproducible and Interactive Data Science

## Syllabus

The aim of this course is to introduce students to the [Jupyter Notebook](http://jupyter.org) which
is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, machine learning and much more. Through the notebooks, research results and the underlying analysis can be transparently reproduced as well as shared.
As an example of a Notebook on gravitational waves published in _Phys. Rev. Lett._, see [here.](http://nbviewer.jupyter.org/github/minrk/ligo-binder/blob/master/index.ipynb)

During three days with alternating video lectures and hands-on exercises, the participants will learn to construct well-documented, electronic notebooks that perform advanced data analysis and produce publication ready plots.
While the course is based on Python, this is not a prerequisite, and many [other programming languages](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels) can be used.

## Credits

4 ECTS.

## Program

_Sessions on **December 3-5, 2018** and project presentations: **January 14-15, 2019**_.
All dates from 10:15 to 15:00.

**Location:** Sölvegatan 27 (The observatory), Department of Astronomy and Theoretical Physics,
Rooms _Cassiopeia_ (Monday morning; Thursday afternoon; and all Friday) or _Andromeda_.

The course consists of four full days: three with alternating video lectures and hands-on exercises, and two
days with project presentations. Lectures are available as Notebooks on this site in the [lectures](lectures) folder.

- Day 1. Introduction
  - Introduction and overview of Jupyter notebooks
  - Installation and package management (Anaconda, managing environments)
  - Navigating cells and iPython "Magic" commands
  - Online resources and getting help
  - Documenting using Markdown: rich text, equations, images, tables, video.
  - Other languages (bash, cython, R, etc.)
  - Online viewing, conversion, sharing, version control (Github, Zenodo, Binder, NBviewer)
  
- Day 2. Numerical Methods, Plotting, and visualization
  - Storage and manipulation of numerical arrays (`numpy`)
  - Plotting in Notebooks (`matplotlib`, `seaborn`)
  - Arranging plots, customizing
  - Making plots publication ready
  - Exporting to vectorized file formats
  - Interactive visialization (`ipywidgets`)
  
- Day 3. Numerical methods and data science
  - Scientific python (`scipy`)
  - Symbolic math (`sympy`)
  - Data parsing and import (csv, excel, json, pickle, pdf, custom files, etc.)
  - Working with large datasets (`pandas`)

- Day 4 and 5. Project presentations

## Prerequisites

- No prior knowledge in Python is required, but familiarity with programming concepts is helpful.
- A laptop connected to the internet (eduroam, for example) and running Unix, MacOS, or Windows and with Anaconda installed, see below.
- Ear phones for silently watching lectures during the sessions.

If you have little experience with Python or shell programming, the following two tutorials may be helpful:

- https://swcarpentry.github.io/shell-novice
- https://swcarpentry.github.io/python-novice-inflammation


## Preparations before the first session

1. Watch the video lectures which will be provided here one week before course start.
2. Install [miniconda3](https://conda.io/miniconda.html) alternatively the full
   [anaconda3](https://www.anaconda.com/download) enviroment on your laptop (the latter is **much** larger).
3. [Download](https://github.com/mlund/jupyter-course/archive/master.zip) the course material
   (this github repository) and unzip.
4. Install and activate the `LUcompute` environment described by the file [`environment.yml`](/environment.yml)
   by running the following in a terminal:

   ```bash
   conda env create -f environment.yml
   source activate LUcompute
   jupyter nbextension enable rubberband/main
   jupyter nbextension enable exercise2/main
   jupyter nbextension enable --py widgetsnbextension
   ```

Instructions for Windows:

1. Install [miniconda3](https://conda.io/miniconda.html).
2. [Download](https://github.com/mlund/jupyter-course/archive/master.zip) the course material (this github repository)
   and unzip.
3. Open the `anaconda prompt` from the start menu.
4. Navigate to the folder where the course material has been unzipped (_e.g._ using `cd` to change directory
   and `dir` to list files in a folder).
5. Install and activate the `LUcompute` environment described by the file [`environment.yml`](/environment.yml)
   by running the following in the `anaconda prompt`:

   ```bash
   conda env create -f environment.yml
   activate LUcompute
   jupyter nbextension enable rubberband/main
   jupyter nbextension enable exercise2/main
   jupyter nbextension enable --py widgetsnbextension
   ```
[Further Information](https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file)

## Project Work

The project work consists of three steps:

1. Each student will make a Notebook project covering topics from day 1-3 with either
  - research, presenting data analysis and theory behind
    a manuscript or published paper. The Notebook should ideally be written
    such that it can act as supporting information (SI) for a journal.
    Here's some [inspiration.](http://nbviewer.jupyter.org/github/jansoe/FUImaging/blob/master/examples/IOSsegmentation/regNMF.ipynb)
  - _or_ a Notebook presenting a text-book topic of choice and aimed at students.
    Here's some [inspiration](http://nbviewer.jupyter.org/github/demotu/BMC/blob/master/notebooks/Transformation2D.ipynb).
  - **Deadline for project: 27/12**

2. A peer-review process where each student reviews and, in writing, comments on _two_ other notebooks.
   The review should be based on the criteria listed below and for each point, include specific
   suggestions for improvements. **Deadline for review: 3/1**
 
3. Notebook presentation to the class (day 4). Maximum 10 minutes per participant and do include your
   answer to the referee reports.

### Notebook Requirements

The notebook must

- [ ] include rich documentation using Markdown, equations, tables, links, etc.
- [ ] import or generate data. If generating, data should be exported to disk.
- [ ] perform data operations using `numpy`, `scipy`, `pandas` or equivalent.
- [ ] create plots of _publication ready_ quality. For an editorial guide on _Graphical Excellence_,
      see [here.](http://dx.doi.org/10/cg2g)
- [ ] include instructions on how to run the notebook, include the required packages.
      This could be an `environment.yml` file.
- [ ] be reproducible, i.e. someone elso should be able to redo the steps

Further, the notebook could

- [ ] act as supporting information for an article
- [ ] have an digital object identifier (DOI)
