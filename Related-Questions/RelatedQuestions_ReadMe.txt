Quora Challenge - Related Questions
Related information: https://www.quora.com/challenges#related_questions

*Description
The related questions challenge represents the development of a program that can find the starting question that most efficiently increases the chance for the user to be led to the right question in the shortest amount of time. In comparison to the upvotes challenge, this could be a variable change versus other similar initial question assessing process for A/B testing that could be measured via the program for the upvotes challenge.

*Personal Opinion
Perhaps the best implementation of this kind of program is for determining the best question to show first without any artificial intelligence learning. In other words, without memorizing and accounting for variables in the word choice and phrasing of questions, this would quickly select the question that would cost the user the least time on average to find the correct question. This is likely the simpler solution than trying to develop a pattern recognition software for user activity as there are many factors that could affect the question asked that would be difficult to account for.

*Method summary
The method applied here is an adapted depth-first search (DFS) program with the inclusion of 'checkpoints'. Because "There exists exactly one path from any question to another, and related questions form undirected pairs between themselves", these checkpoints are necessary to memorize and maintain portions of the path that are used during the search. Once paths are explored and reach a point with no new related questions or 'deadends', if the deadend is not the target then all questions between that deadend and the checkpoint are added to a deadends list that prevents the DFS from returning to that route such that the correct route is void of errors associated with a DFS.

*Improvement ideas
There are probably a few efficiency problems. However, one problem that I would like to address right away is the use of a global variable in order to 'save' the final answer as the DFS searchs through the other alternate paths. A halfway solution was put in place such that when the target has been reached, all questions are added to the deadends list such that the route can not be editted from any remaining strands of the DFS recursive. Perhaps a better solution would be to implement a "stop" function in the event the path to the target has been found in the DFS.
