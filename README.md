This .pyt tool is designed to help power companies assess pipeline integrity risks by integrating multiple datasets and conducting spatial analysis on environmental, social, and infrastructure factors.

Tool Overview


Tool Name:  Pipeline Risk & Threat Assessment Tool
Tool Type: Python Toolbox (.pyt)
Version: 1.0
Developed By: Aliasghar Bazrafkan
Date: 02/27/2025
ArcGIS Pro Version: 3.x
Python Version: 3.9+
Geodatabase Compatibility: File Geodatabase (.gdb), Shapefiles (.shp)

Purpose
This tool identifies potential risks and threats to power companies’s pipeline infrastructure by overlaying and analyzing geospatial data. It automates the classification of high-risk pipeline segments by considering:

Proximity to Sensitive Areas (Natural reserves, wetlands, water bodies, and protected lands).
Environmental Risks (Soil erosion, flooding zones, landslide susceptibility).
Social & Infrastructure Risks (Proximity to urban centers, schools, hospitals, and critical infrastructure).
Pipeline Condition Data (Corrosion levels, maintenance history, pressure variations).



Functionalities

✅ Pipeline Overlay with Risk Layers

Uses spatial joins to integrate pipeline data with environmental, social, and infrastructure risk layers.
✅ Risk Classification Model

Assigns a risk score based on spatial relationships (e.g., pipelines near high-population areas receive higher risk values).
Uses weighted overlay analysis to calculate risk zones.
✅ Proximity Analysis for Critical Infrastructure

Identifies schools, hospitals, and industrial sites within a user-defined buffer distance.
Flags areas where pipelines intersect with major roads, railways, or sensitive ecosystems.
✅ Oil Spill Impact Analysis

Uses hydrology models and terrain analysis to predict the spread of oil spills.
Estimates potential environmental & social impact zones.
✅ Automated Report Generation

Outputs a pipeline risk classification map.
Generates a summary report in CSV or PDF format with flagged high-risk segments.


Input Parameters

Parameter Name	Data Type	Required?	Description

Pipeline Dataset	Feature Class / Shapefile	✅ Yes	Input layer containing BP’s pipeline network.
Environmental Risk Layers	Feature Class / Raster	✅ Yes	Layers representing wetlands, soil erosion zones, flood-prone areas.
Social & Cultural Layers	Feature Class / Shapefile	✅ Yes	Schools, hospitals, population density zones, protected areas.
Critical Infrastructure	Feature Class / Shapefile	✅ Yes	Roads, power stations, industrial sites near pipelines.
Buffer Distance (miles)	Float	⬜ Optional	Distance to analyze proximity-based risks (default: 1 mile).
Output Risk Map	Feature Class	✅ Yes	Path to save classified pipeline risk dataset.

Output
Pipeline Risk Classification Map (Feature class with color-coded risk zones).
Risk Report (CSV/PDF) (Summary of flagged high-risk areas).
Impact Zone Map (Visualizing potential oil spill spread and affected areas).

![image](https://github.com/user-attachments/assets/18c3d8d9-a6bf-409d-9c65-87dbe4acd459)


Results

![image](https://github.com/user-attachments/assets/d886bc41-43ed-4dc2-a292-6310af4c2f85)

