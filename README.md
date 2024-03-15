README

Bertrand Paradox Simulation

This Python code simulates Bertrand's paradox, a classic problem in probability theory and geometric probability. The paradox revolves around the question of how to properly define the probability of randomly selecting a chord of a circle that is longer than a side of an inscribed equilateral triangle. The paradox arises because there are different interpretations of what constitutes a "randomly selected" chord.

How to Run the Code:

Prerequisites:

-Python 3 installed on your system.
-Required Python packages: matplotlib, numpy.

Running the Code:

-Save the provided Python code in a file, e.g., bertrand_simulation.py. <br>
-Open your terminal.
-Navigate to the directory where bertrand_simulation.py is saved.
-Run the code using the command: python bertrand_simulation.py.
-A 'plots.png' file is created on the same directory. Open this file to see the plots of different strategies.
Understanding the Code:

The code is organized into a Python class named Bertrand, which encapsulates the simulation methods and plotting functions.
Three methods are implemented to simulate different approaches to selecting random chords:
Method 1: Randomly select one endpoint of the chord on the circle's circumference and test if it forms a chord longer than the triangle's side.
Method 2: On the radius joining centre of the circle and one of the triangle vertices, choose a point and draw a chord perpendicular to the radius passing through this point. Test if this chord is longer than the triangle's side.
Method 3: Randomly select a point within a smaller concentric circle, representing chords that are completely contained within the circle. Test if these chords are longer than the triangle's side.
Each method generates random points or chords and evaluates whether they satisfy the condition of being longer than the side of the inscribed equilateral triangle.
The results are plotted using matplotlib, with each method's simulation results displayed in separate subplots.
Green lines/points represent chords longer than the triangle's side, while red lines/points represent chords that are not.
Output:

After running the code, the program will display the simulation results in three subplots, each illustrating one method's outcomes.
The console will print the ratio of favorable outcomes to the total number of simulations for each method.
Additionally, the plots will be saved as plots.png in the current directory.
Interpreting the Results:

The simulation results demonstrate the different probabilities obtained through each method, highlighting Bertrand's paradox.
Users can observe how the probability of selecting a chord longer than the side of the equilateral triangle varies depending on the method of selection.
Note:

Adjustments to parameters such as the number of iterations (self.n) or the radius of the circle (self.r) can be made within the code to modify the simulation behavior.
