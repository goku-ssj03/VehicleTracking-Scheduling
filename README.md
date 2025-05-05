This project is about automating the route scheduling of transportation vehicles, in this case buses, when the following input variables are given: 
running time, break time, source, destination and hourly frequency on each route for all 24 hours. The input can be a CSV file or a dataframe.

There are 3 major parts to this code:
1. Creating an input dataframe with random values of the above-mentioned variables. This is required to test the program on any random data
   because if the program runs on this random dataset it can be generalized to any data set.
   
2. Writing the main program which keeps track of the hourly demands of each route, converts that hourly demand of each route in an
   equally distributed duration during that hour, runs a loop every 5th minute on each route to check for bus requirements, and allocates a bus
   to every route that requires it at that point in time. This program also does real-time tracking of each bus and can generate the whole journey
   of every bus between different routes that it covers throughout the day. This program simultaneously does real-time tracking of each route,
   captures the id and hence all the information of the buses running, and can generate the dataset for the whole day showing important information for analysis.

3. This part of the code takes the generalized input created in Step 1 and runs it in the program mentioned in Step 2 to create an output file to create
   the schedule of the buses for the whole city. If here the input file is provided of any city, say Pune or Delhi, this part of the code will give a CSV file
   as an output file which will provide the details of the bus scheduling, as well as real-time tracking of all the buses and the supply-demand analysis of each route.
   
Thanks for your patience :)
