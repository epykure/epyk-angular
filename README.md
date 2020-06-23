
![](https://raw.githubusercontent.com/epykure/epyk-angular/master/static/images/logo.ico)


# Epyk on Angular!

No need to get familiar to TypeScript or even to learn Javascript to start building rich Angular pages !

Presentation
================================

This project is to demonstrate the use of Epyk to push sophisticated views to a Angular framework without having to 
fully change the code.

This can also be an opportunity to share the UI implementation between JavaScript and Python developers by creating rich components.

Lot of components are already available in Epyk but feel free to bring news ideas !

The architecture of this kind of set up the as presented below:

<div align="center" >
    <img width=500 src="https://github.com/epykure/epyk-angular/blob/master/static/images/design.PNG?raw=true">
</div>

It is similar to the set up for other popular web framework like:

- [Vue](https://github.com/epykure/epyk-vue): Available
- [React](https://github.com/epykure/epyk-react): In Progress


Quickstart
================================

> pip install epyk

Install nodeJs from the [official website](https://nodejs.org/en/)

Then install Angular.js CLI from the [Official website](https://cli.vuejs.org/) or use the Python embedded CLI

Then control your environment directly from Epyk by using the mapped CLI.


```py
from epyk.web import angular

node_app = angular.Angular(r"C:\Angular")
angular_name = "angular-apps"

# Install Angular CLI
# node_app.clis.angular()

# Create the Angular App
#node_app.create(angular_name)

# Install the packages but also update the angular.json automatically
#node_app.cli(angular_name).npm(["jquery", "jquery-ui-dist"])

#node_app.router(angular_name)

node_app.serve(angular_name)
```


Then you can create a similar setup to your environment with the reports and views folders.
By running the transpile.py your reports will be automatically transpiled to code compatible with Vue.

It will also mention the missing packages on the app during the conversion to .vue files

<div align="center" >
    <img width=300 src="https://github.com/epykure/epyk-vue/blob/master/static/images/missing_modules.PNG?raw=true">
</div>


Benefits
================================

Code will be always in Python and it can be transpiled to any required output. 
It can obviously be part of a full python stack but without any changes can be also used to a Angular environment.

Routing and file structure will be automatically done from the Epyk Components

<div align="center" >
    <img width=600 src="https://github.com/epykure/epyk-angular/blob/master/static/images/routing.PNG?raw=true">
</div>

This can allow you to map your ML or IA algorithm to reports visible in Jupyter Notebook and in the same way to more 
moderne web platform.

<div align="center" >
    <img width=300 src="https://github.com/epykure/epyk-angular/blob/master/static/images/components.PNG?raw=true">
</div>


Coming Soon
================================

As Epyk is a light wrapper it is possible also to interface with the popular components libraries.
So in the next release of the core framework PrimeNg, Bootstrap, Material Design will be integrated

<div align="center" >
    <img width=600 src="https://github.com/epykure/epyk-angular/blob/master/static/images/extensions.PNG?raw=true">
</div>

Similar concept will be done for React and FluentUI !

Compatibility
================================

This has been tested on Angular9.

You can get more example on the common templates [repository](https://github.com/epykure/epyk-templates/tree/master/web/angular)

More examples of reports are available on Github or in [Jupyter](https://nbviewer.jupyter.org/github/epykure/epyk-templates-notebooks/blob/master/index.ipynb)

Please get in touch if there is any feature you feel Epyk-UI needs