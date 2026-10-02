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

## Dataset

The analysis uses approximately **1.1 million Citi Bike trips from February 2022**.

The trip data includes information such as:

- Ride duration
- Start and end stations
- Start and end coordinates
- Rider type
- Bike type
- Trip distance

The dataset was cleaned and prepared in Python before behavioural clustering and geographic analysis were performed.

## Data Preparation

Before analysis, the trip data was prepared in Python to make it suitable for behavioural and geographic analysis.

Key preparation steps included:

- Inspecting the dataset for missing and inconsistent values
- Converting date and time fields into appropriate formats
- Calculating trip duration
- Calculating distance between trip start and end locations
- Preparing numerical features for clustering
- Removing or investigating records that could distort the analysis

These steps created a clean analytical dataset for rider segmentation and spatial analysis.

## Rider Segmentation with K-Means

K-means clustering was used to identify distinct trip patterns within the dataset based on characteristics such as trip duration and distance.

The Elbow Method was used to help determine an appropriate number of clusters.

The analysis revealed three broad behavioural patterns:

### 1. Commuter-Style Trips
Shorter, more direct journeys consistent with riders using Citi Bike for practical point-to-point transportation.

### 2. Explorer / Leisure Trips
Longer trips covering greater distances, suggesting more recreational or exploratory use of the network.

### 3. Zero-Distance Trips
Trips where the recorded start and end locations resulted in little or no geographic displacement. These trips may represent round trips, very short journeys, or potential operational and equipment issues requiring further investigation.

## Geographic Analysis

Trip patterns were explored geographically using Tableau to understand where different types of journeys occurred across the Citi Bike network.

Mapping the start and end locations helped reveal how rider behaviour varied across the service area and provided operational context for the clusters identified in Python.

This geographic perspective can help operations teams:

- Identify areas with concentrated rider demand
- Understand where different trip behaviours occur
- Support bike and station allocation decisions
- Investigate locations associated with unusual trip patterns

## Key Findings

### 1. Winter Trips Showed Distinct Behaviour Patterns
Clustering revealed different types of Citi Bike usage rather than one uniform rider pattern, including practical point-to-point journeys and longer exploratory trips.

### 2. Trip Duration and Distance Help Differentiate Rider Behaviour
Combining duration and distance provided a useful way to distinguish between different journey patterns within the network.

### 3. Location Adds Important Operational Context
Geographic analysis showed where different trip behaviours occurred, helping translate the clustering results into information that could support station and bike management.

### 4. Zero-Distance Trips Deserve Further Investigation
Trips with little or no geographic displacement may include legitimate round trips or very short journeys, but they can also provide a useful starting point for investigating potential operational or equipment issues.

## Operational Recommendations

Based on the patterns identified in the analysis, Citi Bike could use the findings to support several operational decisions:

### 1. Align Bike Availability with Demand Patterns
Use trip and location patterns to identify areas where bike availability may need to be adjusted during winter.

### 2. Support Station Rebalancing
Combine geographic demand patterns with station-level activity to help prioritise where bikes should be redistributed.

### 3. Investigate Zero-Distance Trip Hotspots
Identify stations with unusually high concentrations of zero-distance trips and investigate whether these are explained by legitimate rider behaviour or possible bike, docking or data-quality issues.

### 4. Monitor Rider Segments Over Time
Repeat the clustering analysis across different months or seasons to determine whether rider behaviour changes and whether operational strategies should be adjusted accordingly.

## Limitations

This analysis should be interpreted within several limitations:

- The dataset covers **February 2022**, so the findings represent winter behaviour rather than year-round Citi Bike usage.
- Clustering identifies patterns in the data but does not prove why riders behaved in a particular way.
- Zero-distance trips cannot automatically be classified as equipment failures because legitimate round trips or very short journeys may produce similar patterns.
- Operational decisions would benefit from combining trip data with additional information such as station capacity, bike availability and maintenance records.

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
