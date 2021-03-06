[![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-Ready--to--Code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/marksspencer/COVID-Binder) 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/marksspencer/COVID-Binder/master?filepath=index.ipynb)

# COVID-Binder
A repo to host a Binder for JupyterLab work with COVID-19 Data

## Notes:
A couple of things:

1. when it asks for the (optional) path to the Notebook, use *file* and simply type in the filename
2. when looking for data to represent, look to see how the data is stored in the CSV. If I had recognized the way the data was stored, I would have put a *LOT* more effort into creating a bunch of different DataFrames [df()] to be able to ploy X & Y values, rather than the mess I created !
3. I apparently over-complicated things using the bokeh.output_file() instead of the bokeh.output_notebook() parameter
4. there are files in the repo that serve different purposes
   * The **Dockerfile** is to enable GitPod properly
   * The **environment.txt** is to enable the virtual environment, called **JupyterLab** 
   * The **requirements.txt** is to insure the *Binder* container has the correct python modules, like *pandas* & *bokeh* 
5. the use of **Binder** (https://mybinder.org) allows the *Jupyter Notebook* to be shared online with the correct URL 
   * The use of **Binder** appears to be one-way: *BinderHub* loads the container from the GitHub repository, but changes      don't appear to be saved *BACK* 
6. **Binder** works pretty well, once you get it configured properly. 100% MY FAULT - I lurched around without RTFM ! :-) 
