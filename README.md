Interactive Multivariate Analysis
================

This app was my feeble attempt to re-create the shiny app called in the **FactoShiny** package: <http://factominer.free.fr/graphs/factoshiny.html> which implements multivariate analysis (unsupervised learning / data mining) methods: Principal Component Analysis, Cluster Analysis and Multiple Correspondence Analysis from the **FactoMineR** package in a shiny application.

This app also implements multivariate analysis methods from the FactoMineR package but includes interactive output plots and data objects in addition to reactivity from user inputs typical of a shiny app.

Data objects (underlying data tables uploaded by the user) use the DT package for interactive rendering.

Plots rely on either rbokeh or plotly libraries for interactivity.

Note: All methods require an input data frame with n rows (individuals) and p columns (variables). In order to facilitate efficient performance of the app, separate file uploads exist so that a data pipeline specific for each analyses (requiring homogenous data types (i.e. all numeric or categorical etc.)) is generated and passed to the underlying analytic methods
