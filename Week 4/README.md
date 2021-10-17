# Web-based Dashboarding



> Let's take a look at web-based dashboarding tool options available in Python. Dash is a python framework for building web analytic applications. It is written on top of Flask, Plotly.js, and React.js. Dash is well-suited for building data visualization apps with highly custom user interfaces.

> Panel works with visualizations from Bokeh, Matplotlib, HoloViews, and many other Python plotting libraries, making them instantly viewable either individually or when combined with interactive widgets that control them. Panel works equally well in Jupyter Notebooks, for creating quick data-exploration tools. Panel can also be used in standalone deployed apps and dashboards, allowing you to easily switch between those contexts as needed. Voilà turns Jupyter notebooks into standalone web applications. It can be used with separate layout tools like jupyter-flex or templates like voila-vuetify. Streamlit can easily turn data scripts into shareable web apps with 3 main principles: embrace python scripting, treat widgets as variables, and reuse data and computation. There are other tools that can be used for dashboarding:

> Bokeh is a plotting library, a widget and app library. It acts as a server for both plots and dashboards. Panel is one of the web-based dashboarding tools built on Bokeh. ipywidgets provides an array of Jupyter-compatible widgets and an interface supported by many Python libraries, but sharing as a dashboard requires a separate deployable server like Voila. Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. Bowtie allows users to build dashboards in pure Python. Flask is a Python-backed web server that can be used to build arbitrary web sites, including those with Python plots that function as flask dashboards.

> Learn more about the tools from the source link. In this course, we will be focusing on Dash.

> Note (Read): <br/>
> [Python dashboarding tools](https://pyviz.org/dashboarding/) <br/>
> [John Snow's data journalism](https://www.theguardian.com/news/datablog/2013/mar/15/john-snow-cholera-map)

<u>Dashboarding Tools</u>
1. Dash from Plotly
1. Panel
1. Voila
1. Streamlit
1. bokeh
1. ipywidgets
1. matplotlib
1. Bowtie
1. Flask

___

![Dashboarding 1](https://github.com/ThivaV/Data_Visualization_with_Python/blob/master/img/Week%204/Dashboarding_1.png)

![Dashboarding 2](https://github.com/ThivaV/Data_Visualization_with_Python/blob/master/img/Week%204/Dashboarding_2.png)
___

## 1. Introduction to Plotly

To learn more about using Plotly to create dashboards, explore:
* [Plotly python](https://plotly.com/python/getting-started/)
* [Plotly graph objects with example](https://plotly.com/python/graph-objects/)
* [Plotly express](https://plotly.com/python/plotly-express/)
* [API reference](https://plotly.com/python-api-reference/)

Here are additional useful resources:
* [Plotly cheatsheet](https://images.plot.ly/plotly-documentation/images/plotly_js_cheat_sheet.pdf)
* [Plotly community](https://community.plotly.com/c/api/5)
* [Related blogs](https://plotlygraphs.medium.com/)
* [Open-source datasets](https://developer.ibm.com/exchanges/data/)
* [Airline dataset](https://developer.ibm.com/exchanges/data/all/airline/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDV0101ENSkillsNetwork20297740-2021-01-01) from [Data Asset eXchange](https://developer.ibm.com/exchanges/data/)
* Airline Reporting Carrier On-Time Performance Dataset. Preview data, dataset metadata, and data glossary [here.](https://dax-cdn.cdn.appdomain.cloud/dax-airline/1.0.1/data-preview/index.html)

## 2. Introduction to Dash

> Dash is a Open-Source User Interface Python library for creating reactive, web-based applications. It is enterprise-ready and a first-class member of Plotly’s open-source tools. Dash applications are web servers running Flask and communicating JSON packets over HTTP requests. Dash’s frontend renders components using React.js. It is easy to build a Graphical User Interface using dash as it abstracts all technologies required to build the applications. Dash is Declarative and Reactive. Dash output can be rendered in web browser and can be deployed to servers. Dash uses a simple reactive decorator for binding code to the UI. This is inherently mobile and cross-platform ready. Let's say you are planning to create an application to answer a business question. As a first step, you need to determine the layout of the application. Decide which chart to use and where to place for example. This is called `layout` part in dash. The second part is to add interactivity to the application. There are two components of Dash First is `Core components` We can import core components as dcc using this import statement Next is `HTML Components` We can import html components as html using this import statement Let's explore these further.

> The dash_html_components library has a component for every HTML tag. You can compose your layout using Python structures with the dash-html-components library.

> The dash_html_components library provides classes for all of the HTML tags. The keyword arguments describe the HTML attributes like style, className, and id.

> No knowledge of HTML or CSS is required but can help in styling the dashboards. Let's see an example of how to use HTML components.

> We start by creating a dash application. From here we create division in our application layout and then adding components to it. In the outer layout division, we first provide a name for our application using the HTML heading component H1. The style parameter is used to change the font color, size and border of the heading. Next, we add paragraph content to the page using a HTML paragraph component P.

> Division can be created inside the outer division. Here we are providing division content as `This is a new division` and styling it using style parameter components. To put all this together, in the application layout create a HTML division and add components. Multiple divisions can be added to the outer application layout. The dash_core_components describe higher-level components that are interactive and generated with JavaScript, HTML, and CSS through the React.js library. Some example of core components are Creating a slider, input area, check items, and datepicker. You can explore other components using the reference link provided at the end of the slide.

> Let's see how to add a slider and dropdown to the application For the dropdown, we use the dcc.dropdown component. We will create a dropdown list under the options parameter as a dictionary. `Label` will hold the dropdown display label name and `value` will hold the value of the label. We can also provide a default dropdown display label using `value` parameter. For the slider, we use the dcc.slider component and provide min and max value of the slider. The `marks` parameter is used for adding a slide marker and `value` parameter for adding default value.

Additional Resources for Dash. To learn more about Dash, explore:
* [Complete dash user guide](https://dash.plotly.com/)
* [Dash core components](https://dash.plotly.com/dash-core-components)
* [Dash HTML components](https://dash.plotly.com/dash-html-components)
* [Dash community forum](https://community.plotly.com/c/dash/16)
* [Related blogs](https://medium.com/plotly/tagged/dash)

### Make dashboards interactive

References:
* [Dash Basic Callbacks](https://dash.plotly.com/basic-callbacks)
* [Core Components](https://dash.plotly.com/dash-core-components)
* [HTML Components](https://dash.plotly.com/dash-html-components)

Additional Resources for Interactive Dashboards <br/>
To learn more about making interactive dashboards in Dash, visit:
* [Python decorators reference 1](https://realpython.com/primer-on-python-decorators/)
* [Python decorators reference 2](https://www.python.org/dev/peps/pep-0318/#current-syntax)
* [Callbacks with example](https://dash.plotly.com/basic-callbacks)
* [Dash app gallery](https://dash-gallery.plotly.host/Portal/)
* [Dash community components](https://plotly.com/dash-community-components/)