# excursions
This project contains informations and code collected and written to understand excursions.
Excursions are stochastic processes on S1, that is periodic.
The goal for this project is understanding how to apply measures that come from the literature, 
to periodic trajectories collected amid different sources.

# material
The description of the project is mantained (privately) in:
https://it.overleaf.com/project/67d3f84ca68167c22cd0e595


# suggestions for good practices
The code should be structured in modules (multiple file.py). 
Each file.py should contain code that with a defined goal to accomplish.
Usually each file.py contains either the definition of classes or functions.
The inputs for classes and functions must be clearly stated and 
Each file.py should be 


# description structure
It is very important for readability (by ourselves and others) and mantainability to have a clear distinction between different parts of a project.

`data`: Put all the input data we have for starters
`output`: Put the output. NOTE: the output of some initial step of the analysis may be input of some later steps in the pipeline. The difference between data and output is solely that the output is pre-processed by you. The goal of a project is to define some output (both conceptually and their realization in data structures of the programming language)
`scripts`: contains all the scripts. For each file.py there should be a file.ipynb to test what file.py does with synthetically generated data.   

# suggested data structures
The principal object of the project are set of trajectories. The data structures that give more support in python to work with such objecs are:    
`geopandas`: to handle geometries   
`pandas`/ `polars`: to handle tabular data (the second choice is for parallel code, it may require more experience)   
`numpy` / `jax.numpy`: to handle matrices and vectors  (the second choice is for parallel code, it may require more experience)   
`scikit.mobility`: to handle trajectorie. (This can be done also with pandas polars and geopandas.)

# main difficulties to face
`Conceptual`:   
1) Understanding the problem at hand, essentially understanding what to measure
`Practical`:    
1) Understanding what data structure to use and how to use it


# suggestion for bibliography
https://www.undermind.ai/