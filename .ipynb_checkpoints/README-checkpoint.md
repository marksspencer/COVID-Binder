[![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-Ready--to--Code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/marksspencer/COVID-Binder) 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/marksspencer/COVID-Binder/master?filepath=index.ipynb)

# COVID-Binder
A repo to host a Binder for JupyterLab work with COVID-19 Data

## Notes:
A couple of things:
    1. when it asks for the (optional) path to the Notebook, use *file* and simply type in the filename
    2. when looking for data to represent, look to see how the data is stored in the CSV. If I had recognized the way the data was stored, I would have put a *LOT* more effort into creating a bunch of different DataFrames [df()] to be able to ploy X & Y values, rather than the mess I created !
    3. I apparently over-complicated things using the bokeh.output_file() instead of the bokeh.output_notebook() parameter
    4. So the latest data-set is different, in that it is more "simply" formatted. It is updated daily, so now I will need to retrieve it manually, or learn how to handle URLs.

## Ongoing Details:
Since it is all based on the pandas module within Python, tight nlw it is easily contained. I think its time to try to have a web-trigger that builds and launches a Docker Container from the github repo after every successful build. I envision a service similar to **mybinder.org** that allows one to run the notebook *live*.