[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mlund/jupyter-course/master)

# Reproducible and Interactive Data Science

- [Syllabus](#Syllabus)
- [Credits](#Credits)
- [Program](#Program)
- [Prerequisites](#Prerequisites)
- [Preparation Before the First Session](#Preparation)
- [Project Work](#Project)
- [Notebook Requirements](#Requirements)
- [Getting a DOI Via Zenodo](#Zenodo)
- [Create and Export Conda Environments](#Environments)
- [Troubleshooting](#Troubleshooting)
- [External Resources](#External)

<a name="Syllabus"></a>
## Syllabus 

The aim of this course is to introduce students to the [Jupyter Notebook](http://jupyter.org) which
is an open-source software that allows you to create and share documents that contain live code, equations, visualizations, and explanatory text. Uses include: data cleansing and manipulation, numerical simulations, statistical modeling, machine learning, and much more. Through the notebooks, research results and the underlying analyses can be transparently reproduced as well as shared.
As an example, see [this Notebook](http://nbviewer.jupyter.org/github/minrk/ligo-binder/blob/master/index.ipynb) on gravitational waves published in _Physical Review Letters_.

During three days with alternating video lectures ([Intro & Widgets](https://lu.instructuremedia.com/embed/f7dbab71-5fad-4308-a4d2-1dd0e7d7a3b7), 
[Libraries](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d), 
[ATLAS Dijet](see below) and hands-on exercises, the participants will learn to construct well-documented, electronic notebooks that perform advanced data analyses and produce publication ready plots.
While the course is based on Python, this is not a prerequisite since the Jupyter Notebook supports [many programming languages](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels). The name Jupyter itself stands for Julia, Python, and R, the main languages of data science.

<a name="Credits"></a>
## Credits 

4 ECTS.

Workload equivalent to one working week (5 full-time days) for going through the course and seminars (1.5 hp), one working week to complete the individual project and implementation of corrections (1.5 hp), and 2.5 working days for the peer-review of other students project (0.5 hp).  

<a name="Logistics"></a>
## Logistics 

The course is held in "flipped classroom" mode: after the first introductory and get-to-know-each-other session, the students are supposed go through the videos themselves, and have Q&A sessions with teachers and helpers. 
All students and some of the teachers will be in LINXS, near Ideon, and other teachers will be on Zoom, with the room coordinates to be given to the participants.
There is also a [Discord server](https://discord.gg/3w7R7vYA). 

_Introductory sessions with teachers_ on **December 6, 2022** from 10:15 to 17:00 (with breaks for fika and lunch)

_Q&A Sessions with teachers_ on **December 8 and 9, 2022** from 10:15 to 17:00. 

<a name="Program"></a>
## Program 

The course consists of a taught component with alternating video lectures ([Intro & Widgets](https://lu.instructuremedia.com/embed/f7dbab71-5fad-4308-a4d2-1dd0e7d7a3b7), [Libraries](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d), 
ATLAS Dijet (see below) and hands-on exercises. All notebooks shown in the video lectures are available on this site in the [lectures](lectures) folder.

- Day 1. Introduction
    - [Introduction](https://lu.instructuremedia.com/embed/b76e3161-adcc-4c81-93df-3ba17e7c3a1e) and overview of the Jupyter Notebook (10')
    - Introduction to project work and peer discussion (15')
    - Installation and package management (Miniconda)
    - [Binder](https://youtu.be/BqJyaejvVjQ?t=1315) and [conda environments](https://conda.io/docs/user-guide/tasks/manage-environments.html)
    - Navigating cells, [online resources](#External), and getting help 
    - Documenting using Markdown: rich text, equations, images, tables, videos
    - IPython Magic commands 
    - Cross-language interaction (`bash`)
    - Python [built-in functions](https://youtu.be/YpBUiEsTiEA)
    - Storage and manipulation of [numerical arrays](https://youtu.be/2xJsNi3wk-s) (`numpy`) 
    
- Day 2. Python and Data Science, Plotting
    - (Live demo) Explore a Notebook in action: machine learning for image morphing
    - Repeated operations and [universal functions](https://youtu.be/469ukhzwEPg) (`numpy`, `Cython`, and `fortranmagic`)
    - [Data structures](https://youtu.be/26ZioEwRw00) and [data wrangling](https://youtu.be/pHa3uuSZh6Y) (`pandas`)
    - [Pivot tables](https://youtu.be/ODFpGo7UomA), [grouping and aggregating](https://youtu.be/oh8UijClQoE) (`pandas`)    
    - Creating [publication ready plots](https://youtu.be/B0iTbVySNtc) (`matplotlib`)
    - Plotting [images, errorbars, histograms, and composite plots](https://youtu.be/Xyobv9kGQxU) (`matplotlib`)
    - Exporting figures to raster and vector formats (`matplotlib`)
    - Plotting [categorical data](https://youtu.be/c0Bd8iWmHGw) (`matplotlib`,`pandas`,`seaborn`)
    - 
- Day 3. Visualization and Interactivity
    - Nonlinear least-squares (`scipy`, `R`, and `rpy2`)
    - [IPython widgets](https://luplay.education.lu.se/media/MinRK-Jupyter-COMPUTE2018-widgets/0_18ipnucr)
    - [Interactive plots](https://youtu.be/oLU5eIO7b84) (`bokeh`)
    - Version control, sharing, and archiving (Github and [Zenodo](https://youtu.be/IdLSGZAdhlQ?t=266))
    - [full videos] Explore a Notebook in action in [_the search for new particles_](https://github.com/urania277/jupyter-dijets/tree/jupyter-course-compute-2018) ([ATLAS Dijet 1](https://lu.instructuremedia.com/embed/1041f33b-af73-4ded-91d2-fc570d99d87f) ([ATLAS Dijet 2](https://lu.instructuremedia.com/embed/35624ec2-4073-4f05-9d2b-3a85c0cd8f24) ([ATLAS Dijet 3](https://lu.instructuremedia.com/embed/0d0ab8ab-6c84-4a57-b5f8-e80ed76c3a3e) ([ATLAS Dijet 4](https://lu.instructuremedia.com/embed/205f2870-3d0f-48f4-94fc-a7da72f3f7c6))
    
<a name="Prerequisites"></a>
## Prerequisites

- No prior knowledge in Python is required, but familiarity with programming concepts is helpful.
- A laptop connected to the internet (eduroam, for example) and running Linux, MacOS, or Windows and with Anaconda installed, see below.
- Earphones for watching lectures in your own time / re-watching them during the sessions (we will also provide breakout rooms).

If you have little experience with Python or shell programming, the following two tutorials may be helpful:

- https://swcarpentry.github.io/shell-novice
- https://swcarpentry.github.io/python-novice-inflammation

<a name="Preparation"></a>

## Preparation Before the First Session

1. Watch the video lectures ([Intro & Widgets](https://lu.instructuremedia.com/embed/f7dbab71-5fad-4308-a4d2-1dd0e7d7a3b7), 
[Libraries](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d), 
ATLAS dijets (see above, Day 3))
2. Install [miniconda3](https://conda.io/miniconda.html) alternatively the full
   [anaconda3](https://www.anaconda.com/download) enviroment on your laptop (the latter is **much** larger).
3. [Download](https://github.com/mlund/jupyter-course/archive/master.zip) the course material
   (this github repository) and unzip.
4. Uncomment the line with "# - gcc # [osx]" in the file [`environment.yml`](/environment.yml).
5. Install and activate the `LUcompute` environment described by the file [`environment.yml`](/environment.yml)
   by running the following in a terminal:

   ```bash
   conda env create -f environment.yml
   conda activate LUcompute
   ```

Instructions for Windows:

1. Watch the video lectures ([Intro & Widgets](https://lu.instructuremedia.com/embed/f7dbab71-5fad-4308-a4d2-1dd0e7d7a3b7), [Libraries](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d), ATLAS dijets (see above, Day 3))
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
[Documentation on conda environments](https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file) 

<a name="Project"></a>
## Project Work

The project work consists of three steps:

1. Each student will make a Notebook project covering topics from day 1–4 with either:
  - research, presenting data analysis and theory behind
    a manuscript or published paper. The Notebook should ideally be written
    such that it can act as supporting information (SI) for a journal.
    Here's some [inspiration.](http://nbviewer.jupyter.org/github/jansoe/FUImaging/blob/master/examples/IOSsegmentation/regNMF.ipynb)
  - _or_ a Notebook presenting a text-book topic of choice and aimed at students.
    Here's some [inspiration](http://nbviewer.jupyter.org/github/demotu/BMC/blob/master/notebooks/Transformation2D.ipynb).
  - **Deadline for project: January 30th**
  
2. Each student will upload their project on a public GitHub repository created through [GitHub Classroom](https://classroom.github.com/a/b7DO7_Ok) 
For a brief introduction to git repositories, see [here](https://guides.github.com/activities/hello-world/#commit). Details and repositories will be made available at the end of the course. 

3. A peer-review process where each student reviews and writes comments on _two_ other notebooks by creating issues on the respective GitHub repositories.
   The review should be based on the criteria listed below. For each point, include specific suggestions for improvements. The teachers can also add feedback on how to improve the notebook. **Deadline for review: February 15th.** <br> 
   
4. The deadline for implementing the reviewer comments on your notebook and __answering the GitHub issues__ is **March 15th**. At this point you should also have a Zenodo DOI for your project - add this as a badge to your repository, or as a link to your README. You will have to also add (to your Github repository) a text file that explains what changes you've made, and why. This process simulates a peer-review for scientific papers, so you're ready 
   
5. Save your project to your own GitHub repository when the course has finished as we may delete it before the next course event.

<a name="Requirements"></a>
## Notebook Requirements

This check list summarizes the minimum requirements for the Notebook project to be approved. It should be used as a reference for both the development of the Notebook and the peer-review process.

- [ ] Documentation:
  - [ ] title and abstract of the project (max 300 words)
  - [ ] includes instructions on how to run the notebook 
  - [ ] includes the required packages in an `environment.yml` file
  - [ ] includes a brief explanation of the reason each package/library was used 
  - [ ] includes rich documentation using Markdown (equations, tables, links, images or videos)
  - [ ] is reproducible, _i.e._, someone else should be able to redo the steps
- [ ] Input/Output:
  - [ ] uses `pandas` to read large data sets or `numpy` to load data from text files
  - [ ] uses `pandas` to save to disk the processed or generated data
- [ ] Scientific computing/data processing:
  - [ ] performs numerical operations (`numpy`, `scipy`, `pandas`) or manipulates, groups, and aggregates a data set (`pandas`) 
- [ ] Data visualization:
  - [ ] includes at least one composite plot (inset or multiple panels)
  - [ ] produces _publication ready_ quality figures (see [here](http://dx.doi.org/10/cg2g) for an editorial guide on _Graphical Excellence_):
    - [ ] the figures are 89 mm wide (single column) or 183 mm wide (double column)
    - [ ] the axes are labeled
    - [ ] the font sizes are sufficiently large
    - [ ] the figures are saved as rasterized images (300 dpi) or vector art
- [ ] Version control, sharing, and archiving:
  - [ ] is archived in a repository with a digital object identifier (DOI)
  
<a name="Zenodo"></a>
## Getting a DOI via Zenodo

Part of your project work will consist of adding a Digital Object Identifier [DOI](https://en.wikipedia.org/wiki/Digital_object_identifier) to your work, through Zenodo. 
In order to do that, you should watch the videos mentioned in "day 3": 
    - Version control, sharing, and archiving (Github and [Zenodo](https://youtu.be/IdLSGZAdhlQ?t=266))
The easiest and preferred way to do it is by connecting your Github account to Zenodo first, enabling the repository to be seen by Zenodo, then making a tag in GitHub, following the instructions [here](https://guides.github.com/activities/citable-code/).

<a name="Environments"></a>
## Create and Export Conda Environments

The command to [create a new environemnt](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands) with Python x.y is 
```bash
conda create --name myenv python=x.y
```
where `myenv` is a name of your choice for the new environment and x.y is a specific Python version (e.g. 2.7 or 3.6).
After activating the environemnt (`conda activate myenv`), you can install all the other packages within the environment.
`conda list` shows the list of packages installed in the environment.
The command to [export the active environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#sharing-an-environment) `myenv` to an environment yml file (e.g. `myenv.yml`) is
```bash
conda env export > myenv.yml
```

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

- Cross-language interaction is a striking feature of Jupyter notebooks: The possibility to integrate multiple languages in the same notebook makes it feasible to exploit the best tools of the various languages in the different steps of data analysis. You can read more about it in [this post](https://blog.jupyter.org/i-python-you-r-we-julia-baf064ca1fb6).
- The Jupyter notebook is a very popular tool for working with data in academia as well as in the private sector.
  - These [tutorials](https://www.gw-openscience.org/tutorials/) show how the [LIGO/VIRGO collaboration](https://www.nobelprize.org/prizes/physics/2017/press-release/) extensively uses Jupyter notebooks to communicate its   research.
  - The streaming service Netflix currently uses Jupyter notebooks as the main tool for data analysis. For example, recommendation algorithms which suggest which movies or TV series to watch next are currently run on Jupyter notebooks. You can read more about it in [this post](https://medium.com/netflix-techblog/notebook-innovation-591ee3221233).
  - In 2017 Jupyter received the [ACM Software System Award](https://blog.jupyter.org/jupyter-receives-the-acm-software-system-award-d433b0dfe3a2), a prestigious award that it shares with projects such as Unix and the Web.
- There are many freely available online resources to learn data science. 
  - The best resource to find help with programming and scripting is
[Stack Overflow](https://stackoverflow.com), which is a question and answer website curated by software developer communities. 
  - An excellent book is "Python Data Science Handbook" by Jake VanderPlas which is freely available as Jupyter notebooks at [this GitHub page](https://github.com/jakevdp/PythonDataScienceHandbook). On the author's webpage, you can also find a list of excellent [talks, lectures, and tutorials](http://vanderplas.com/speaking.html) and a [blog](http://jakevdp.github.io/).
  - Yet another useful resource is the podcast [Data Skeptic](https://dataskeptic.com) which features a collection of entertaining and educational mini-lectures on data science as well as interviews with experts.
