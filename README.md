# EchoS
**Team Name** - EchoS

**Team Members** - Suah Cho (suc139@pitt.edu), Edward Cho (edc86@pitt.edu)

# **Overview**
This project analyzes neighborhood safety in Pittsburgh using multiple public datasets. It focuses on three main aspects of safety: crime, traffic accidents, and fire incidents. We combined data from City Facilities, Police Arrest Data, Fire Incidents, and City Traffic Signs to build metrics that provide insights into each neighborhood's overall safety.

# **Project Goals**
Evaluate Crime Safety:
Combine police facility data with arrest records to create a metric called "arrest per police facility." A lower value suggests fewer arrests relative to the number of police stations, which is used as a proxy for safer neighborhoods.

**Assess Traffic Safety:**
Analyze the City Traffic Signs dataset under the assumption that a higher number of traffic signs leads to fewer traffic accidents. The top 20 neighborhoods with the most traffic signs were identified as areas with better traffic safety.

**Determine Fire Safety:**
Process the Fire Incidents dataset to count the frequency of fire incidents per neighborhood. Neighborhoods with fewer fire reports are considered safer from a fire hazard perspective.

**Data Intersection Analysis:**
Determine common neighborhoods that appear in multiple datasets. By comparing intersections between police and traffic data and between police and fire data, we narrowed down the neighborhoods that consistently show strong safety signals.

**Datasets**
City Facilities.csv:
Contains information on city facilities in Pittsburgh. This dataset was used to extract police facilities and build a mapping between neighborhoods and police zones.

Police Arrest Data.csv:
Contains arrest records for various neighborhoods. This data was aggregated and combined with police facilities data to calculate the arrest per police facility metric.

Fire Incidents.csv:
Includes records of fire incidents across neighborhoods. We computed the total number of fire incidents per neighborhood to assess fire safety.

City Traffic Signs.csv:
Consists of traffic sign locations across neighborhoods. The data was used to count the number of traffic signs per neighborhood as an indicator of measures in place for traffic safety.

**Data Cleaning and Standardization:**

The datasets were cleaned by converting key fields to strings, trimming extra spaces, and converting text to lowercase.

A mapping was created between neighborhoods and police zones using the City Facilities data.

Metric Computation:

Crime Metric: Calculated as the number of arrests per police facility in a neighborhood.

Traffic Safety Metric: Derived by counting the number of traffic signs per neighborhood.

Fire Safety Metric: Measured by counting the number of fire incidents.

**Intersection Analysis:**

Neighborhoods from each dataset were compared to identify common areas between police data and traffic sign data as well as between police data and fire incident data.

The common neighborhoods provided a base for further discussion and decision making.

**Visualization:**

Several bar charts were generated to visualize the metrics. Graphs include the bottom 20 neighborhoods for arrest per police facility ratio, the top 20 neighborhoods for traffic signs, and the bottom 20 neighborhoods for fire incident counts.

Custom labels and annotations were used to clearly display key statistics.

**Findings**
After evaluating and combining the metrics, our analysis indicated that neighborhoods with low arrest per police facility ratios, abundant traffic signs, and fewer fire incidents tend to be the safest. By intersecting the key neighborhoods identified in each individual dataset, we focused on common safety signals. Our final conclusion was that Central Northside stands out as the best and safest neighborhood in Pittsburgh based on our combined metrics.

**Running the Code**
The analysis was performed using Python with the following libraries:

pandas

numpy

matplotlib

To run the project:

Clone the repository.

Ensure the required CSV files are in the same directory as the scripts.

Execute the Python scripts in your preferred environment or run them using a command-line interface.

**Conclusion**
This project demonstrates that evaluating neighborhood safety requires a multi-faceted approach. By combining various datasets, we have developed a more comprehensive view of the factors that contribute to a safe living environment in Pittsburgh. The results of our analysis, particularly the insights from the police data, suggest that Central Northside is the safest neighborhood based on our metrics. We hope that this analysis will serve as a valuable tool for residents, policymakers, and future research initiatives.


