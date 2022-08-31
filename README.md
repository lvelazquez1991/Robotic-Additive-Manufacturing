# Robotic-Additive-Manufacturing
Contains the MATLAB codes and data to train and test a feedforward neural network. The inputs to train this network are the printing parameters that were manually selected from experience and the outputs are measurements of outside diameter, height, and wall width of the 3D printed cylindrical samples. 

Input parameters are:
1. Velocity of the end-effector (mm/s).
2. Instantaneous value of resin viscosity during extrusion (Pa.s).
3. Layer height (mm).
4. Step motor delay (ms).

The values of velocity of the end-effector and layer height value were manually set before each printing session in Slic3r, a virtual environment to pre-process CAD models to generate a gcode for 3D printing. The value of viscosity was calculated using rheology data from material tests performed on the resin used and the step motor delay was manually set in Arduino to control the stepper motor RPM. In this case, the value of stepper motor delay becomes a measure of extrusion rate. 

The output parameters are:
1. Outside diameter of the printed cylinder sample (mm).
2. Wall width of the cylinder (mm).
3. Height of the cylinder (mm).

Output parameter values were measured using a digital caliper accurate to 0.01 mm. 

A total of 187 data points are shown to train and test the neural network. 

