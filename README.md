# Power Grid Analysis
In this project, we attempt to describe the robustness of a power grid to both random and targeted failures via a graph-theoretic model.


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
This repository contains the following notebooks that are best accessed in the order listed:

`00_zip_code_data.ipynb` contains metadata related to zip codes around the united states.
`Power_Grid_Analysis.ipynb` contains the constructors for the graph/network our model is built on.

## Data sources
We downloaded our power datasets from the US Energy Information Agency (EIA) and the Massachusetts Bureau of Geographic Information (MassGIS), though we only used the former as it is more complete.


## To do
- Network construction
- Monte Carlo simulation of network failures. Important questions: What constitutes a network failure? How to handle sources/sinks not near our network geographically?
- Computation of a percolation coefficient for our network
- Simulation of targeted attacks on network
