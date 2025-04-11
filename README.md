# Assignment
# Project: Wheelchair-Accessible Navigation System
Unit: SIT215 Computational Intelligence

Assignment: Assignment 1 – Problem Solving

Student ID: S224045922

# Overview
This project aims to develop a navigation system tailored for wheelchair users by addressing the limitations of conventional routing systems. The solution integrates computational intelligence (A* algorithm) to compute optimal and accessible routes based on real-world environmental constraints such as kerb ramps, accessible sidewalks, slopes, and obstacles. The project is implemented in Python and is designed to run in a Jupyter Notebook, allowing for an interactive and iterative workflow complete with visualizations.

It comprises three main tasks:

- Task 1: Environment creation and problem formation, where the physical environment is mapped using “Parsed Lines” (representing accessible pathways) and “Parsed Points” (key facilities).

- Task 2: Basic navigation implementation using the A* algorithm with the standard Haversine distance as a heuristic.

- Task 3: Enhanced environment and heuristics comparison, where additional path segments are added and a new heuristic is developed that includes slope penalties.

# Requirements and Dependencies
- Python: Version 3.7 or later is recommended.

- Jupyter Notebook: Ensure that Jupyter is installed (you can install via pip install notebook if needed).

### Libraries:

- math (Standard library)

- heapq (Standard library)

- matplotlib (Install via pip install matplotlib)

- matplotlib.patches (comes with matplotlib)

#  Detailed Usage Instructions
### 1. Launching the Notebook:

- Open your terminal or command prompt.

- Run the command:

`jupyter notebook`

- The Notebook Dashboard will open in your default web browser.

### 2. Opening the Notebook:

- Locate and click on the file AS.ipynb in the dashboard.

### 3. Running the Code:

Execute the notebook cells sequentially. You can run all cells by going to the "Cell" menu and selecting "Run All."

Ensure that each cell executes without errors. The code is modularized, and key functions include:

+ The haversine function (lines 1–10) calculates the great-circle distance.

+ The build_graph function (lines 12–26) constructs the environment’s graph from parsed lines.

+ The a_star function (lines 28–48) implements the search algorithm.

+ The enhanced_heuristic (lines 56–63) incorporates slope penalties.

+ The plot_comparison function (lines 72–94) creates side-by-side visual comparisons.

+ The main function (lines 96–142) integrates all components.

## 4. Viewing Results:

- Textual outputs in the console will display the computed full path along with a compressed path showing only key facilities.

- The Notebook will also display visual comparisons of routes computed with the original and enhanced heuristics.

- Look for embedded figures (e.g., “Figure 1: Original vs. Enhanced Route”) that illustrate the route overlays on the accessible network.
<img src="https://github.com/bella06-09/Assignment/blob/main/Screenshot%202025-04-12%20at%2003.12.50.png?raw=true">

## 5. Modifying the Data:

- If you need to update the environment, you can modify the parsed_points and parsed_lines variables directly in the Notebook.

- Adjust the slope penalty and threshold in the enhanced_heuristic function (default penalty is 0.2 km, threshold 0.05 km) to refine your model.

# Additional Information

## Heuristic Comparison:
Task 3 includes a detailed comparison of route outputs using the original Haversine heuristic and an enhanced heuristic that includes slope penalties to avoid hazardous segments.

## Visual Aids:
The Notebook contains side-by-side graphs that illustrate the differences between the two approaches, providing a clear understanding of how the environmental data influences the route computation.

## Future Enhancements:
Future versions may incorporate real-time updates or a more interactive GUI interface to allow dynamic user inputs for start/goal points and adjustment of environmental parameters.
