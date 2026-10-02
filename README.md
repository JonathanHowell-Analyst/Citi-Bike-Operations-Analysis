# Citi Bike Operations Analysis
### Optimising Winter Operations Through Rider Behaviour and Geographic Analysis

## Executive Summary

This project analyses approximately 1.1 million Citi Bike trips from February 2022 to understand winter rider behaviour and identify opportunities to improve operations.

Using Python, K-means clustering and geographic analysis, the project segments trip behaviour into distinct rider patterns and explores how trip duration, distance and location can support better operational decisions.

The analysis highlights opportunities to improve bike availability, station management and the identification of potentially problematic zero-distance trips.

## Business Problem

Citi Bike operates a large bike-sharing network where demand varies by rider behaviour, location and season.

During winter, understanding how customers use the network can help operations teams allocate bikes more effectively, manage stations and identify unusual trip patterns.

This analysis focuses on three business questions:

1. What distinct rider behaviour patterns exist within winter trips?
2. Where are different types of trips concentrated geographically?
3. How can these patterns support better operational decisions?

## Tools & Skills

- **Python** — data cleaning, transformation and exploratory analysis
- **pandas** — processing approximately 1.1 million trip records
- **Scikit-learn** — K-means clustering and rider segmentation
- **Matplotlib / Seaborn** — exploratory data visualisation
- **Tableau** — geographic and spatial analysis
- **Data Analysis** — identifying behavioural and operational patterns
- **Business Analysis** — translating findings into operational recommendations

Key Insights
The Behavioral Split: Identified a clear distinction between "Commuters" (Cluster 0) and "Explorers" (Cluster 2), each requiring a different rebalancing frequency.

Operational Geography: Cluster 0 is heavily anchored in Manhattan’s commercial core, while Cluster 2 dominates waterfront leisure zones.

Maintenance Alerts: Identified "Zero-Distance" trips (Cluster 1) that signal potential equipment or docking station hardware errors.

Technical Skills & Tools
Data Engineering: Performed extensive cleaning, data type management, and coordinate validation on a 1.1M record dataset using Python (Pandas).

Machine Learning: Implemented K-means Clustering and utilized the Elbow Technique to determine optimal segment counts.

Spatial Analysis: Conducted a Spatial Intersect in Tableau by joining trip coordinates with NYC Neighborhood Tabulation Area (NTA) GeoJSON files.

Interactive Visualization: Developed a multi-point Tableau Storyboard to communicate findings to stakeholders.

Final Deliverables
Interactive Storyboard: [https://public.tableau.com/views/Task6_7_17695020482740/Story1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link]

Analysis Notebooks: [Located in the 03 Scripts folder]

Case Study PDF: [Located in the 05 Sent to Client folder]
