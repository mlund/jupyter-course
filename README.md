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
is an open-source software that allows you to create and share documents that contain live code, equations, visualizations, and explanatory text. Uses include: data cleansing and manipulation, numerical simulations, statistical modeling, machine learning, and much more. Through the notebooks, research results and the underlying analyses can be transparently reproduced as well as shared.
As an example, see [this Notebook](http://nbviewer.jupyter.org/github/minrk/ligo-binder/blob/master/index.ipynb) on gravitational waves published in _Physical Review Letters_.

During three days with alternating video lectures ([Intro & Widgets](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_vujap4by?iframeembed=true&playerId=kaltura_player_5bfdb69292c20&flashvars[playlistAPI.kpl0Id]=0_nc717bpa&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true), [Libraries](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d), [ATLAS Dijet](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_hr5l2zj6?iframeembed=true&playerId=kaltura_player_5bfdb5d709908&flashvars[playlistAPI.kpl0Id]=0_pspvclw2&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true)) and hands-on exercises, the participants will learn to construct well-documented, electronic notebooks that perform advanced data analyses and produce publication ready plots.
While the course is based on Python, this is not a prerequisite since the Jupyter Notebook supports [many programming languages](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels). The name Jupyter itself stands for Julia, Python, and R, the main languages of data science.

<a name="Credits"></a>
## Credits 

4 ECTS.

<a name="Program"></a>
## Program 

_Sessions on **December 3-5, 2018** and project presentations: **January 14-15, 2019**_.
All dates from 10:15 to 15:00.

**Location:** 
- December 3, 2018: _Sal D L315_, Fysicum, Sölvegatan 14
- December 4, 2018: lecture hall _HUB_, Department of Astronomy and Theoretical Physics, Sölvegatan 27
- December 5, 2018: lecture hall _Cassiopeia_, Department of Astronomy and Theoretical Physics, Sölvegatan 27

The course consists of five full days: three with alternating video lectures ([Intro & Widgets](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_vujap4by?iframeembed=true&playerId=kaltura_player_5bfdb69292c20&flashvars[playlistAPI.kpl0Id]=0_nc717bpa&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true), [Libraries](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d), [ATLAS Dijet](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_hr5l2zj6?iframeembed=true&playerId=kaltura_player_5bfdb5d709908&flashvars[playlistAPI.kpl0Id]=0_pspvclw2&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true)) and hands-on exercises, and two
days with project presentations. The notebooks shown in the video lectures are available on this site in the [lectures](lectures) folder.

- Day 1. Introduction
  - morning:
    - [Introduction](https://luplay.education.lu.se/media/MinRK-Jupyter-COMPUTE2018-intro/0_z85if4is) and overview of the Jupyter Notebook (10')
    - Introduction to project work and peer discussion (15')
    - Installation and package management (Miniconda)
    - [Binder](https://youtu.be/BqJyaejvVjQ?t=1315) and [conda environments](https://conda.io/docs/user-guide/tasks/manage-environments.html)
    - Navigating cells, [online resources](#External), and getting help 
    - Documenting using Markdown: rich text, equations, images, tables, videos
    - IPython Magic commands 
    - Cross-language interaction (`bash`)
  - afternoon: 
    - Python [built-in functions](https://youtu.be/YpBUiEsTiEA)
    - Storage and manipulation of [numerical arrays](https://youtu.be/2xJsNi3wk-s) (`numpy`)
    - Repeated operations and [universal functions](https://youtu.be/469ukhzwEPg) (`numpy`, `Cython`, and `fortranmagic`)
  
- Day 2. Data Science
  - morning: 
    - [Data structures](https://youtu.be/26ZioEwRw00) and [data wrangling](https://youtu.be/pHa3uuSZh6Y) (`pandas`)
    - [Pivot tables](https://youtu.be/ODFpGo7UomA), [grouping and aggregating](https://youtu.be/oh8UijClQoE) (`pandas`)
    - Creating [publication ready plots](https://youtu.be/B0iTbVySNtc) (`matplotlib`)
  - afternoon:
    - Plotting [images, errorbars, histograms, and composite plots](https://youtu.be/Xyobv9kGQxU) (`matplotlib`)
    - Exporting figures to raster and vector formats (`matplotlib`)
    - Plotting [categorical data](https://youtu.be/c0Bd8iWmHGw) (`matplotlib`,`pandas`,`seaborn`)
  
- Day 3. Visualization and Interactivity
  - morning:
    - Nonlinear least-squares (`scipy`, `R`, and `rpy2`)
    - Explore a Notebook in action in [_the search for new particles_](https://github.com/urania277/jupyter-dijets/tree/jupyter-course-compute-2018) ([ATLAS Dijet](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_hr5l2zj6?iframeembed=true&playerId=kaltura_player_5bfdb5d709908&flashvars[playlistAPI.kpl0Id]=0_pspvclw2&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true))
  - afternoon:
    - [IPython widgets](https://luplay.education.lu.se/media/MinRK-Jupyter-COMPUTE2018-widgets/0_18ipnucr)
    - [Interactive plots](https://youtu.be/oLU5eIO7b84) (`bokeh`)
    - Version control, sharing, and archiving (Github and [Zenodo](https://youtu.be/IdLSGZAdhlQ?t=266))
    
- Day 4 and 5. Project presentations

<a name="Prerequisites"></a>
## Prerequisites

- No prior knowledge in Python is required, but familiarity with programming concepts is helpful.
- A laptop connected to the internet (eduroam, for example) and running Linux, MacOS, or Windows and with Anaconda installed, see below.
- Earphones for silently watching lectures during the sessions.

If you have little experience with Python or shell programming, the following two tutorials may be helpful:

- https://swcarpentry.github.io/shell-novice
- https://swcarpentry.github.io/python-novice-inflammation

<a name="Preparation"></a>
## Preparation Before the First Session

1. Watch the video lectures ([Intro & Widgets](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_vujap4by?iframeembed=true&playerId=kaltura_player_5bfdb69292c20&flashvars[playlistAPI.kpl0Id]=0_nc717bpa&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true), [Libraries](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d), [ATLAS dijets](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_hr5l2zj6?iframeembed=true&playerId=kaltura_player_5bfdb5d709908&flashvars[playlistAPI.kpl0Id]=0_pspvclw2&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true))
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

1. Watch the video lectures ([Intro & Widgets](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_vujap4by?iframeembed=true&playerId=kaltura_player_5bfdb69292c20&flashvars[playlistAPI.kpl0Id]=0_nc717bpa&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true), [Libraries](https://www.youtube.com/playlist?list=PLto3nNV9nKZlXSWOAqmmn4J7csD4I6a2d), [ATLAS dijets](https://api.kaltura.nordu.net/p/310/sp/31000/embedIframeJs/uiconf_id/23450585/partner_id/310/widget_id/0_hr5l2zj6?iframeembed=true&playerId=kaltura_player_5bfdb5d709908&flashvars[playlistAPI.kpl0Id]=0_pspvclw2&flashvars[playlistAPI.autoContinue]=true&flashvars[playlistAPI.autoInsert]=true&flashvars[ks]=&flashvars[localizationCode]=en&flashvars[imageDefaultDuration]=30&flashvars[leadWithHTML5]=true&flashvars[forceMobileHTML5]=true&flashvars[nextPrevBtn.plugin]=true&flashvars[sideBarContainer.plugin]=true&flashvars[sideBarContainer.position]=left&flashvars[sideBarContainer.clickToClose]=true&flashvars[chapters.plugin]=true&flashvars[chapters.layout]=vertical&flashvars[chapters.thumbnailRotator]=false&flashvars[streamSelector.plugin]=true&flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&flashvars[dualScreen.plugin]=true))
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

1. Each student will make a Notebook project covering topics from day 1–3 with either:
  - research, presenting data analysis and theory behind
    a manuscript or published paper. The Notebook should ideally be written
    such that it can act as supporting information (SI) for a journal.
    Here's some [inspiration.](http://nbviewer.jupyter.org/github/jansoe/FUImaging/blob/master/examples/IOSsegmentation/regNMF.ipynb)
  - _or_ a Notebook presenting a text-book topic of choice and aimed at students.
    Here's some [inspiration](http://nbviewer.jupyter.org/github/demotu/BMC/blob/master/notebooks/Transformation2D.ipynb).
  - **Deadline for project: January 3, 2019**
  
2. Each student will upload her/his project on a public GitHub repository created through [GitHub Classroom](https://classroom.github.com/a/pwsOX3wC) 
For a brief introduction to git repositories, see [here](https://guides.github.com/activities/hello-world/#commit).
You can find your repository [here](https://github.com/teokem), press **cancel** if an error has occured during importing.<br>
Notify your referees via email that your notebook is ready to be checked.

3. A peer-review process where each student reviews and writes comments on _two_ other notebooks by creating issues on the respective GitHub repositories.
   The review should be based on the criteria listed below. For each point, include specific
   suggestions for improvements. **Deadline for review: January 10, 2019**
 
4. Notebook presentation to the class (day 4). Maximum 10 minutes per participant and do **include** your
   answer to the referee reports.
   
5. Save your project when the course finished as we may delete it before the next course event.

### Notebook Requirements

This check list summarizes the minimum requirements for the Notebook project to be approved. It should be used as a reference for both the development of the Notebook and the peer-review process.

- [ ] Documentation:
  - [ ] includes rich documentation using Markdown (equations, tables, links, images or videos)
  - [ ] includes instructions on how to run the notebook 
  - [ ] includes the required packages in an `environment.yml` file
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
