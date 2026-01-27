Project: Citi Bike Winter Mobility Strategy (NYC)
Executive Summary
This project analyzes 1.1 million Citi Bike trip records from February 2022 to develop a data-driven winter operations strategy. By moving beyond basic membership categories, I utilized unsupervised machine learning to identify three distinct behavioral clusters. These findings were then localized via a spatial intersect in Tableau to provide a "Logistics Playbook" for Manhattan, Brooklyn, and Queens.

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
