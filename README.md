# Quora Challenges

The files in this repository are those related to challenges found at https://www.quora.com/challenges.
Python was selected as it is the my most likely primary programming language to use in data science.

A more detailed description and analysis of the solutions can be found in the README files in each challenge's folder. However, a summary of the methods employed for each solution is described below:
1) Upvotes - A 'viewing' window for period of days is created and 'slides' across the upvotes array to determine number of nonincreasing and nondecreasing trends.
2) Related Questions - A depth-first search was performed on the relation tree with checkpoints to revert back in case the path does not find the endpoints.
