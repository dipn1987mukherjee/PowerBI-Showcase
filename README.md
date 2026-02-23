# PowerBI-Showcase

Cruise Fleet Executive Intelligence Dashboard
This Power BI dashboard provides a comprehensive analysis of the global cruise industry, focusing on operational efficiency, fleet luxury positioning, and geospatial distribution. It transforms raw data into actionable insights for maritime executives to benchmark performance against industry standards.

Business Key Performance Indicators (KPIs)
The dashboard tracks three critical metrics to determine brand positioning:
Service Ratio (Target < 2.0): Measures guest-to-staff efficiency. A lower ratio (highlighted in Green) indicates a higher luxury tier with more personalized service.
Space Ratio (Goal > 40): Calculated as Gross Tonnage per Passenger. This identifies the "elbow room" and comfort level onboard.
Market Segmentation: A dynamic status indicator that automatically classifies the selected fleet as "Standard" or "Premium" based on live Space Ratio benchmarks.

Key Features & Visualizations
Fleet Tonnage Distribution: A horizontal bar chart ranking cruise lines by their total gross tonnage, identifying market leaders like Royal Caribbean and Carnival.
Geospatial HQ Mapping: A bubble map localized by Latitude and Longitude to visualize the global headquarters and operational hubs of major cruise lines.
Operational Deep-Dive: A detailed matrix providing row-level data on ship length, total cabins, and crew counts for granular fleet management.
Labor Analysis: A 100% stacked bar chart comparing the ratio of Total Crew vs. Total Passengers, used to monitor labor costs and service quality across brands.

Technical Stack
Data Modeling: Implemented a Star Schema by relating a core ship-info dataset to a custom geographic mapping table.
DAX (Data Analysis Expressions):
Dynamic Measures for scaling raw units (100s/1000s) to real-world values.
Conditional Formatting logic to trigger status alerts (Red/Green) based on performance targets.
SWITCH and IF logic for automated market categorization.
Power Query: Performed data cleansing, column renaming, and data type standardization for maritime specific units.

Actionable Insight
By utilizing the Slicer at the top, users can see that lines like Cunard and Crystal consistently exceed the 40+ Space Ratio, justifying their premium price points, while larger lines focus on high-volume efficiency.

How to use: Open the .pbix file in Power BI Desktop to interact with the slicers and drill-through features.
