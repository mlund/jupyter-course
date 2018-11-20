[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mlund/jupyter-course/master)

# Reproducible and Interactive Data Science

- [Syllabus](#Syllabus)
- [Credits](#Credits)
- [Program](#Program)
- [Prerequisites](#Prerequisites)
- [Preparation Before the First Session](#Preparation)
- [Project Work](#Project)
- [Troubleshooting](#Troubleshooting)
- [External Resources](#External)

<a name="Syllabus"></a>
## Syllabus 

The aim of this course is to introduce students to the [Jupyter Notebook](http://jupyter.org) which
is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, machine learning and much more. Through the notebooks, research results and the underlying analysis can be transparently reproduced as well as shared.
As an example of a Notebook on gravitational waves published in _Phys. Rev. Lett._, see [here.](http://nbviewer.jupyter.org/github/minrk/ligo-binder/blob/master/index.ipynb)

During three days with alternating [video lectures](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d) and hands-on exercises, the participants will learn to construct well-documented, electronic notebooks that perform advanced data analysis and produce publication ready plots.
While the course is based on Python, this is not a prerequisite, and many [other programming languages](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels) can be used.

<a name="Credits"></a>
## Credits 

4 ECTS.

<a name="Program"></a>
## Program 

_Sessions on **December 3-5, 2018** and project presentations: **January 14-15, 2019**_.
All dates from 10:15 to 15:00.

**Location:** 
- December 3, 2018: lecture hall, Fysicum, Sölvegatan 14
- December 4, 2018: lecture hall _HUB_, Department of Astronomy and Theoretical Physics, Sölvegatan 27
- December 5, 2018: lecture hall _Cassiopeia_, Department of Astronomy and Theoretical Physics, Sölvegatan 27

The course consists of five full days: three with alternating [video lectures](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d) and hands-on exercises, and two
days with project presentations. The notebooks shown in the video lectures are available as Notebooks on this site in the [lectures](lectures) folder.

- Day 1. Introduction
  - Introduction and overview of Jupyter notebooks
  - Installation and package management (Anaconda, managing environments)
  - Navigating cells and iPython "Magic" commands
  - Online resources and getting help
  - Documenting using Markdown: rich text, equations, images, tables, video.
  - Other languages (bash, cython, R, etc.)
  - Online viewing, conversion, sharing, version control (Github, Zenodo, Binder, NBviewer)
  - Python built-in functions
  - Storage and manipulation of numerical arrays (`numpy`)
  - Repeated operations and universal functions (`numpy` and `fortranmagic`)
  
- Day 2. Data Science
  - Data wrangling and data scraping (`pandas`)
  - Pivot tables, aggregation, and grouping (`pandas`)
  - Storage and manipulation of numerical arrays (`numpy`)
  - Creating publication ready plots (`matplotlib`)
  - Exporting to raster and vector formats (`matplotlib`)
  - Plotting images, errorbars, histograms, and composite plots (`matplotlib`)
  - Non-linear least squares (`scipy`)
  
- Day 3. Visualization and Interactivity
  - Plotting categorical data (`matplotlib`,`pandas`,`seaborn`)
  - Interactive plots (`bokeh`)
  - Ipython widgets

- Day 4 and 5. Project presentations

<a name="Prerequisites"></a>
## Prerequisites

- No prior knowledge in Python is required, but familiarity with programming concepts is helpful.
- A laptop connected to the internet (eduroam, for example) and running Unix, MacOS, or Windows and with Anaconda installed, see below.
- Earphones for silently watching lectures during the sessions.

If you have little experience with Python or shell programming, the following two tutorials may be helpful:

- https://swcarpentry.github.io/shell-novice
- https://swcarpentry.github.io/python-novice-inflammation

<a name="Preparation"></a>
## Preparation Before the First Session

1. Watch the [video lectures](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d)
2. Install [miniconda3](https://conda.io/miniconda.html) alternatively the full
   [anaconda3](https://www.anaconda.com/download) enviroment on your laptop (the latter is **much** larger).
3. [Download](https://github.com/mlund/jupyter-course/archive/master.zip) the course material
   (this github repository) and unzip.
4. Install and activate the `LUcompute` environment described by the file [`environment.yml`](/environment.yml)
   by running the following in a terminal:

   ```bash
   conda env create -f environment.yml
   source activate LUcompute
   ```

Instructions for Windows:

1. Watch the [video lectures](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d)
2. Install [miniconda3](https://conda.io/miniconda.html).
3. [Download](https://github.com/mlund/jupyter-course/archive/master.zip) the course material (this github repository)
   and unzip.
4. Open the `anaconda prompt` from the start menu.
5. Navigate to the folder where the course material has been unzipped (_e.g._ using `cd` to change directory
   and `dir` to list files in a folder).
6. Install and activate the `LUcompute` environment described by the file [`environment.yml`](/environment.yml)
   by running the following in the `anaconda prompt`:

   ```bash
   conda env create -f environment.yml
   activate LUcompute
   ```
[Further Information](https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file)

<a name="Project"></a>
## Project Work

The project work consists of three steps:

1. Each student will make a Notebook project covering topics from day 1-3 with either
  - research, presenting data analysis and theory behind
    a manuscript or published paper. The Notebook should ideally be written
    such that it can act as supporting information (SI) for a journal.
    Here's some [inspiration.](http://nbviewer.jupyter.org/github/jansoe/FUImaging/blob/master/examples/IOSsegmentation/regNMF.ipynb)
  - _or_ a Notebook presenting a text-book topic of choice and aimed at students.
    Here's some [inspiration](http://nbviewer.jupyter.org/github/demotu/BMC/blob/master/notebooks/Transformation2D.ipynb).
  - **Deadline for project: January 2, 2019**

2. A peer-review process where each student reviews and, in writing, comments on _two_ other notebooks.
   The review should be based on the criteria listed below and for each point, include specific
   suggestions for improvements. **Deadline for review: January 8, 2019**
 
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

<a name="Troubleshooting"></a>
## Troubleshooting

If your notebook seems to have an issue on connection, similar to the lines below:

   ```
[E 12:18:57.001 NotebookApp] Uncaught exception in /api/kernels/5e16fa4b-3e35-4265-89b0-ab36bb0573f5/channels
    Traceback (most recent call last):
      File "/Library/Python/2.7/site-packages/tornado-5.0a1-py2.7-macosx-10.13-intel.egg/tornado/websocket.py", line 494, in _run_callback
        result = callback(*args, **kwargs)
      File "/Library/Python/2.7/site-packages/notebook-5.2.2-py2.7.egg/notebook/services/kernels/handlers.py", line 258, in open
        super(ZMQChannelsHandler, self).open()
      File "/Library/Python/2.7/site-packages/notebook-5.2.2-py2.7.egg/notebook/base/zmqhandlers.py", line 168, in open
        self.send_ping, self.ping_interval, io_loop=loop,
    TypeError: __init__() got an unexpected keyword argument 'io_loop'
[I 12:18:58.021 NotebookApp] Adapting to protocol v5.1 for kernel 5e16fa4b-3e35-4265
   ```
You should either a) downgrade the package "tornado" b) change L178 of the file 

```
[your conda installation location]/miniconda3/envs/LUcompute/lib/python3.6/site-packages/notebook/base/zmqhandlers.py 
```

from 

   ```
                self.send_ping, self.ping_interval, io_loop=loop,
   ```

into

   ```
                self.send_ping, self.ping_interval,
   ```


https://stackoverflow.com/questions/48090119/jupyter-notebook-typeerror-init-got-an-unexpected-keyword-argument-io-l

<a name="External"></a>
## External Resources

This course will give you an overview on the Jupyter notebook and show you how you can use them to save a record of your workflow, share your research, and make your work repeatable. The Jupyter notebook supports dozens of programming languages. The name Jupyter itself stands for Julia, Python, and R, the main languages of data science. Cross-language interaction is a striking feature of Jupyter notebooks: The possibility to integrate multiple languages in the same notebook makes it feasible to exploit the best tools of the various languages in the different steps of data analysis. You can read more about it in [this post](https://blog.jupyter.org/i-python-you-r-we-julia-baf064ca1fb6).
The Jupyter notebook is a very popular tool for working with data in academia as well as in the private sector.
For example, the [LIGO/VIRGO collaboration](https://www.nobelprize.org/prizes/physics/2017/press-release/) extensively use the Jupyter notebook to communicate and show the reproducibility of their data analyses, as shown in these [tutorials](https://www.gw-openscience.org/tutorials/).
A private company which is currently using Jupyter notebooks as the main tool for data analysis is the streaming service Netflix. For example, recommendation algorithms which suggest which movies or TV series to watch next are currently run on Jupyter notebooks. You can read more about it in [this post](https://medium.com/netflix-techblog/notebook-innovation-591ee3221233).
Moreover, in 2017 Jupyter received the ACM Software System Award, a prestigious award that it shares with projects such as Unix and the Web. 

There are many freely available online resources to learn data science. 
The best resource to find help with programming and scripting is
[Stack Overflow](https://stackoverflow.com), which is a question and answer website curated by software developer communities. 
An excellent book is "Python Data Science Handbook" by Jake VanderPlas which is freely available as Jupyter notebooks at [this GitHub page](https://github.com/jakevdp/PythonDataScienceHandbook). On the author's webpage, you can also find a list of excellent [talks, lectures, and tutorials](http://vanderplas.com/speaking.html) and a [blog](http://jakevdp.github.io/).
Yet another useful resource is the podcast [Data Skeptic](https://dataskeptic.com) which features a collection of entertaining and educational mini-lectures on data science as well as interviews with experts.
