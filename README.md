# Zebrafish_Jaw_Characterisation
This Python script is designed for the analysis and visualization of zebrafish jaw development. It includes
functionality for plotting jaw shapes at various developmental stages and predicting future shapes using linear
regression. These measurements are essential in determining if genes are involved in jaw development and their contribution to bodyplan development.
This code can be modified to identify outliers to the 'typical' wildtype developental trajectory, and if this effect is of statisitical significance

Features
Visualize Jaw Shape: Plot the jaw shape at different developmental stages.
Statistical Analysis: Calculate descriptive statistics for each stage.
Growth Rate Analysis: Analyze and visualize the growth rate of the zebrafish jaw.
Predict Future Development: Use linear regression to predict jaw shapes at future developmental stages.
Installation
Ensure you have Python installed on your system. The script requires the following libraries:

pandas
numpy
matplotlib
scikit-learn
You can install these packages using pip:
pip install pandas numpy matplotlib scikit-learn

Usage
Plotting Jaw Shape:
Use the plot_jaw_shape function to visualize the jaw shape at a specific stage.

Calculating Statistics:
The calculate_statistics function provides descriptive statistics for each stage.

Analyzing Growth Rate:
plot_growth_rate plots the growth rate based on average coordinate changes.

Predicting Future Stages:
predict_future_jaw_shapes uses linear regression to predict jaw shapes at future stages.

Example:

python
Copy code
# Plot jaw shape
plot_jaw_shape(data, stage_number)

# Calculate and display statistics
stats = calculate_statistics(data)

# Plot growth rate
plot_growth_rate(data, number_of_stages)

# Predict future jaw shapes
predicted_shapes = predict_future_jaw_shapes(data, future_stages)


Dataset Format
The script expects a dataset with the following columns:

stage: Developmental stage of the zebrafish.
point: Identifier for each key point in the jaw.
x: X-coordinate of the jaw point.
y: Y-coordinate of the jaw point.
