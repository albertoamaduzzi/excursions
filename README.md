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

# suggestion minimal daily routine
1) Reading articles:
- sum up in the overleaf as a section what you have read
2) Looking at data:
- Choose some information about what you have learned and write it somewhere.
If it seems bullshit is ok. Reference yourself to what you have already learnt
3) Coding:
- Comment, or try to comment every snippets of code you write. Some snippet are going 
to multiply above all the first period when ideas are not that clear.
At the end of the day always repeat the routine of:
`cd $PROJECT_DIR`, get in the git repository   
`git add .` , this command adds the changes of the local project into an internal state of github, which means, you can now have the possibility to update the repository online    
`git commit -m "description of whatever you have done"`, this snippet marks the added material with a name (implicitely) and a description    
`git push` it updates the project online. It is useful to have synchronized material. 
