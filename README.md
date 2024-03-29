![](./images/dvpy-1.png)

# Why
For people who struggle to start in data visualization with Python

# Description
![](./images/dvpy-2.png)

This hands-on in-person workshop is based on [Data Visualization with Python Course by IBM Cognitive Class](https://cognitiveclass.ai/courses/data-visualization-python)

>Learn how to represent data graphically to convey insights to clients, customers, and stakeholders.


# [Outline](https://github.com/aymanibrahim/dvpy/blob/master/notebooks/00_Outline.ipynb)
The workshop will cover core topics:

## [01 Intro](https://github.com/aymanibrahim/dvpy/blob/master/notebooks/01_Intro.ipynb) [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aymanibrahim/dvpy/blob/master/notebooks/01_Intro.ipynb)

Line Plot            |  Trend | Top 5
:-------------------------:|:-------------------------:|:-------------------------:
![](./figs/01_Intro/immigration_from_haiti.png)  |  ![](./figs/01_Intro/immigration_from_china_india.png)|  ![](figs/01_Intro/immigration_trend_top5_countries.png)

- Introduction to Data Visualization
- Introduction to Matplotlib
- Basic Plotting with Matplotlib
- Dataset on Immigration to Canada
- Line Plots

## [02 Basic Visualization](https://github.com/aymanibrahim/dvpy/blob/master/notebooks/02_Basic.ipynb) [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aymanibrahim/dvpy/blob/master/notebooks/02_Basic.ipynb)

Bar Chart            |  Histogram | Area Plot
:-------------------------:|:-------------------------:|:-------------------------:
![](./figs/02_Basic/top15_immigration_countries_barh.png)  |  ![](./figs/02_Basic/immigration_from_195_countries_histogram.png)|  ![](figs/02_Basic/immigration_trend_top5_countries_modified_alpha.png)

- Area Plots
- Histograms
- Bar Charts

## [03 Specialized Visualization](https://github.com/aymanibrahim/dvpy/blob/master/notebooks/03_Specialized.ipynb) [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aymanibrahim/dvpy/blob/master/notebooks/03_Specialized.ipynb)

Pie Chart            |  Box Plot | Bubble Plot
:-------------------------:|:-------------------------:|:-------------------------:
![](./figs/03_Specialized/immigration_by_continent_2013_pie.png)  |  ![](./figs/03_Specialized/immigration_china_india_boxplot.png)|  ![](figs/03_Specialized/immigration_from_brazil_argentina_bubble.png)

- Pie Charts
- Box Plots
- Scatter Plots
- Bubble Plots

## [04 Advanced Visualization](https://github.com/aymanibrahim/dvpy/blob/master/notebooks/04_Advanced.ipynb) [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aymanibrahim/dvpy/blob/master/notebooks/04_Advanced.ipynb)

Waffle Chart            |  Word Cloud | Regression Plot
:-------------------------:|:-------------------------:|:-------------------------:
![](./figs/04_Advanced/immigration_from_denmark_norway_sweden_waffle_chart.png)  |  ![](./figs/04_Advanced/top_wordcloud.png)|  ![](figs/04_Advanced/immigration_best_fit_white_seaborn.png)

- Waffle Charts
- Word Clouds
- Seaborn and Regression Plots

## [05 Maps and Geospatial Data](https://github.com/aymanibrahim/dvpy/blob/master/notebooks/05_Maps.ipynb) [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aymanibrahim/dvpy/blob/master/notebooks/05_Maps.ipynb)

Choropleth Map             | Clusters Map 
:-------------------------:|:-------------------------:|
![](./figs/05_Maps/immigration_choropleth_map.png)  |  ![](./figs/05_Maps/incidents_sanfran_map_clusters.png)|  

- Introduction to Folium
- Maps with Markers
- Choropleth Maps

# Prerequisites
- [Python for Data Science Workshop](https://github.com/aymanibrahim/pyds)
- [Data Analysis with Python Workshop](https://github.com/aymanibrahim/dapy)

# Pre-workshop 

You will need a laptop that can access the internet 

## 1: Installation
Install miniconda or install the (larger) Anaconda distribution

[Install Python using Miniconda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html)

OR [Install Python using Ananconda](https://www.anaconda.com/distribution/)

## 2: Setup

### 2.1: Download workshop code & materials
Clone the repository
```
git clone git@github.com:aymanibrahim/dvpy.git
```
OR [Download the repository as a .zip file](https://github.com/aymanibrahim/dvpy/archive/master.zip)

### 2.2: Change directory to dvpy
Change current directory to **dvpy** directory
```
cd dvpy
```
### 2.3: Install Python with required packages
Install Python with the required packages into an environment named _dvpy_  as per [environment.yml](https://github.com/aymanibrahim/dvpy/blob/master/environment.yml) YAML file.
```
conda env create -f environment.yml
```
When conda asks if you want to proceed, type "y" and press Enter.

## 3: Activate environment
Change the current default environment (_base_) into _dvpy_ environment.
```
conda activate dvpy
```

## 4: Install & Enable ipywidgets extentions
Install ipywidgets JupyterLab extension
```
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```

Enable  widgetsnbextension
```
jupyter nbextension enable --py widgetsnbextension --sys-prefix
```


## 5: Check installation
Use [check_environment.py](https://github.com/aymanibrahim/dvpy/blob/master/check_environment.py) script to make sure everything was installed correctly, open a terminal, and change its directory (cd) so that your working directory is the workshop directory _dvpy_ you cloned or downloaded. Then enter the following:
```
python check_environment.py
```
If everything is OK, you will get the following message:
> Your workshop environment is set up

## 6: Start JupyterLab
Start JupyterLab using:
```
jupyter lab
```
JupyterLab will open automatically in your browser.

You may access JupyterLab by entering the notebook server’s URL into the browser.

## 7: Stop JupyterLab
Press **CTRL + C** in the terminal to stop JupyterLab.

## 8: Deactivate environment
Change the current environment (_dvpy_) into the previous environment.
```
conda deactivate
```

# Workshop Instructor
## Ayman Ibrahim

- [LinkedIn](https://www.linkedin.com/in/aymanibrahim/)
- [Kaggle](https://www.kaggle.com/aymani)
- [GitHub](https://github.com/aymanibrahim)
- [Twitter](https://twitter.com/AymanIbrahim)
- [Facebook](https://www.facebook.com/ayman.ibrahim.awad)

# References
- [Python: Programming language](https://www.python.org)
- [Conda: Package and environment manager](https://conda.io/en/latest/)
- [Anaconda: Python distribution](https://www.anaconda.com/distribution/)
- [Miniconda: Minimal installer for conda](https://conda.io/en/latest/miniconda.html)
- [NumPy: Fundamental package for scientific computing with Python](https://numpy.org)
- [Matplotlib: Python 2D plotting library](https://matplotlib.org)
- [seaborn: Statistical Data Visualization](https://seaborn.pydata.org)
- [pandas: Python data analysis library](https://pandas.pydata.org)
- [scikit-learn: Machine Learning in Python](https://scikit-learn.org/stable/index.html)
- [Jupyter Notebook: Web application to create documents with code, equations, visualizations and text](https://jupyter.org/)
- [JupyterLab: Web-based development environment for Jupyter Notebooks](https://jupyter.org/)
- [Python for Data Science: Course by IBM Cognitive Class](https://cognitiveclass.ai/courses/python-for-data-science/)
- [Data Analysis with Python: Course by IBM Cognitive Class](https://cognitiveclass.ai/courses/data-analysis-python/)
- [Data Visualization with Python: Course by IBM Cognitive Class](https://cognitiveclass.ai/courses/data-visualization-with-python/)

# Contributing
Thanks for your interest in contributing! There are many ways to contribute to this project. Get started [here](https://github.com/aymanibrahim/dvpy/blob/master/CONTRIBUTING.md).

# License

## Workshop Code
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Workshop Materials

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a>

<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">*Data Visualization with Python Workshop*</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/aymanibrahim" property="cc:attributionName" rel="cc:attributionURL">Ayman Ibrahim</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.  Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://cognitiveclass.ai/courses/data-visualization-with-python/" rel="dct:source">IBM Cognitive Class Data Visualization with Python </a> by <a href="https://www.linkedin.com/in/aklson/"> Alex Aklson, PhD</a>, <a href="https://www.linkedin.com/in/jayrajasekharan/"> Jay Rajasekharan</a></a> and <a href="https://ca.linkedin.com/in/polonglin"> Polong Lin.</a>

