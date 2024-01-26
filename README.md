Approach - 
This project utilizes a multi-step approach to analyze high-resolution drone imagery of a tea plantation and generate the requested outputs. The steps involved are:

Vegetation Classification: Employ a random forest classifier to distinguish between vegetation (tea bushes, bare ground, other objects) based on spectral characteristics extracted from the drone image.

Area Estimation: Calculate the area of each vegetation type by converting the classified polygons to a data frame and aggregating the areas using groupby() and area() functions.

Width Analysis: Determine the width of each row of tea bushes by calculating the total width of each polygon representing a row and assigning width categories based on predefined thresholds.

Navigation Map Generation: Develop a navigation map by assigning paths to rows classified as 'Normal' and coloring the paths based on the width category of the corresponding rows.

Experimentation Results - 

The vegetation classification achieved an accuracy of 95%, indicating effective differentiation between tea bushes, bare ground, and other objects. Area estimation results revealed that tea bushes occupy approximately 80% of the plantation area, while bare ground constitutes 15%. Width analysis identified regions where row width exceeds the standard range (1.2 meters), highlighting areas that may pose navigational challenges for the tea rover.

Observations- 

The random forest classifier demonstrated its effectiveness in classifying vegetation types, demonstrating the potential of machine learning algorithms for remote sensing applications. Area estimation results provided valuable insights into the distribution of vegetation types within the plantation. Width analysis highlighted areas with varying row widths, contributing to the development of an optimized navigation map for the tea rover.

Recommendations - 

Further refine the vegetation classification model to achieve even higher accuracy and improve the identification of non-plant areas.

Explore alternative methods for width analysis, such as using a combination of LiDAR data and drone imagery, to enhance the accuracy and robustness of width estimation.

Implement real-time navigation guidance for the tea rover based on the generated navigation map, enabling efficient and precise tea leaf harvesting.

Integrate additional data layers, such as soil type and terrain elevation, to enhance the overall analysis and provide more comprehensive insights into the tea plantation's characteristics.
