# Power Grid Analysis
In this project, we attempt to describe the robustness of a power grid to both random and targeted failures via a graph-theoretic model.

![](./plots/cover_plot.svg)
<!-- <img src="./controllers_brief.svg"> -->
## Context
In the event of a disaster FEMA has identified seven different lifelines that require attention in an affected area. Those are as follows:

1. Safety and Security
2. Food, Water, and Sheltering
3. Health and Medical
4. Energy (Power and Fuel)
5. Communication
6. Transportation
7. Hazardous Waste

We here are interested in quantifying risk to energy lifelines, specifically the electrical power grid. We imagine that a similar analysis can be conducted on oil/natural gas resources, but we do not extend our model to those here.

## Notebooks
This repository contains the following notebooks:

[`00_zip_code_data.ipynb`](00_zip_code_data.ipynb) contains metadata related to zip codes around the United States.

[`01_Graph_Building.ipynb`](01_Graph_Building.ipynb) contains the body of the work, including data cleaning, visualization, EDA, and constructors for the graph/network our model is built on.

## Data sources
We downloaded our power datasets from the US Energy Information Agency (EIA) and the Massachusetts Bureau of Geographic Information (MassGIS), though we only used the former as it is more complete.


## Conclusions
We find that our model of the network does not exhibit criticality. That is to say, we find no singular probability $p$, above which our model demonstrates a network failure, and below which the grid happily carries on.
