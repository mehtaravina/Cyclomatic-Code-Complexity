This is a project to developed in python to evaluate Cyclomatic Complexity of Code using REST service system.

The REST system focuses on the efficient computation of code complexity for a given repository, utilizing a set of nodes as appropriate to minimize execution time from submission to result return.



Method -

Manager prepares the files cloned from a git repository. Receives code for each commit. Calculating on a commit by commit basis. Places them into a Queue, where the worker can access the files. Waits for the results from the worker and stores them into a Database (File name, Cyclomatic Complexity, Time). Plots the results using Matplotlib.

Worker Uses Cyclomatic Complexity library (Lizard) to calculate the Average Cyclomatic Complexity for each commit present in the Queue. When the worker finishes, they ask for more work until the queue is empty.

Result -

As the number of workers increases, the time taken decreases. It comes to a certain point where increasing the number of workers doesn't increase the efficiency of the system.


Ravina Mehta CS7NS1 (Student ID - 1737906)
