
The goal is to create a collection of Python data-visualization demos and documentation for using
[observable-jupyter](https://github.com/thomasballinger/observable-jupyter), a new Python library
that bridges the gap between JavaScript and Python!

## Example: Observable Plot

This Python notebook, [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pbogden/observable-jupyter-demos/blob/master/notebooks/observable_plot.ipynb),
demonstrates exploratory data analysis with
[Observable Plot](https://observablehq.com/@observablehq/plot), 
a JavaScript library built with [D3](https://github.com/d3/d3#d3-data-driven-documents).
The demo shows that the Python API using observable-jupyter is as simple as the popular Seaborn API.

**Yet another new Python plotting package?**

No. What's new is that observable-jupyter integrates
JavaScript data-viz capabilities directly into Python with a super simple API.
This means that the power of HTML5 data visualization is readily accessible from Python.
The demo above shows how it's done with Observable Plot,
a charting library by [Mike Bostock](https://observablehq.com/@mbostock), creator of D3 and co-founder
of [Observable, Inc](http://observablehq.com).
But you can take the same approach to use all sorts of JavaScript data-viz libraries directly from Python.

**Do I need to be front-end developer to customize things on the Python side?**

No. Integrating JavaScript data viz into Python used to be hard, but not anymore -- 
you no longer need to be a front-end web dev to do it.
The demo shows how it's done. 
Once things are set up, it's easy to create custom data visualizations with Python in Jupyter notebooks (or Colab) 
without touching the JavaScript.

**It can't be that easy. What's the catch?**

Someone needs to set up an [Observable notebook](https://www.google.com/search?q=observable+notebook&oq=observable+notebook&aqs=chrome..69i57j69i64j69i60l3j69i65.3681j0j7&sourceid=chrome&ie=UTF-8#kpvalbx=_XSUhYtfsCpiDytMPvsmf4Aw36) to expose the parameters and data variables
needed by the JavaScript library. You do need to know some JavaScript to set it up, but it's not hard.
That's the purpose of this [Observable notebook](https://observablehq.com/@pbogden/observable-plot-jupyter).
It's a very slightly modified fork that I made of 
[Mike Bostock's original](https://observablehq.com/@observablehq/plot).
Parameters and data are specified in Python and then sent as JSON to the JavaScript by a simple
Python function call using the observable-jupyter API. 
This only needs to be done once, then anyone can use it.

**What's next?**

The goal is a collection of demos and documentation for doing data visualization in Python with observable-jupyter.
These demos will showcase a variety of cutting-edge JavaScript libraries for interactive maps, dashboards and 3-D, etc.
We'll include the the kinds of things you can't currently do in Python, such as
this interactive [Mona Lisa Histogram](https://observablehq.com/@d3/mona-lisa-histogram).
For data scientists who know a little JavaScript, we'll also create documentation that shows how to set up 
Observable notebooks so that they're usable with observable-jupyter.
