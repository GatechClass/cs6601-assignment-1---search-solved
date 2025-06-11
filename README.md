# cs6601-assignment-1---search-solved
**TO GET THIS SOLUTION VISIT:** [CS6601 Assignment 1 – Search Solved](https://mantutor.com/product/cs-6601-artificial-intelligence-assignment-1-search-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top kksr-disabled" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;112754&quot;,&quot;readonly&quot;:&quot;1&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS6601 Assignment 1 - Search Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Setup

Clone the repository and activate the Conda repository you created in Assignment 0:

git clone https://github.gatech.edu/omscs6601/assignment_1.git conda activate ai_env

Overview

Search is an integral part of AI. It helps in problem solving across a wide variety of domains where a solution isnâ€™t immediately clear. You will implement several graph search algorithms with the goal of solving bi-directional and tri-directional search.

Submission

All code you will edit is in the submission.py file, which will be submitted to Gradescope for grading. You are allowed two submissions every thirty minutes. In your Gradescope submission history, you can mark a certain submission as ‘Active’.

The Files

While you’ll only have to edit and submit submission.py, there are a number of notable files:

| File | Description | | —-:| :———–| |submission.py | Where you will implement your PriorityQueue, Breadth First Search, Uniform Cost Search, _A Search_, Bi-directional Search, Tri-directional Search | |search_submission_tests.py | Simple unit tests to validate your searches validity and number of nodes explored | |search_submission_tests_grid.py | Tests searches on uniform grid and highlights path and explored nodes. | |search_unit_tests.py | More detailed tests that run searches from all possible pairs of nodes in the graph | |romania_graph.pickle | Serialized graph files for Romania. | |atlanta_osm.pickle | Serialized graph files for Atlanta (optional for robust testing for Race!). | |explorable_graph.py | A wrapper around networkx that tracks explored nodes. FOR DEBUGGING ONLY | |visualize_graph.py | Module to visualize search results. See below on how to use it. | |osm2networkx.py* | Module used by visualize graph to read OSM networks. |

Resources

Gradescope: Error Messages

Canvas Course Videos: Search Module

R&amp;N slides on Uninformed Search

Informed Search

Comparing BFS and DFS

A* Search

Links from Canvas, below the videos: * Finding Optimal Solutions to Rubik’s Cube Using Pattern Databases * God’s Number is 26 in the

Quarter-Turn Metric * Reach for Aâˆ—: An Efficient Point-to-Point Shortest Path Algorithm * Computing the Shortest Path: Aâˆ— Search Meets Graph Theory * Reach-based Routing: A New Approach to Shortest Path Algorithms Optimized for Road Networks

Resources for bi-directional searches * A Star meets Graph Theory * Bi Directional A Star – Slides * Bi Directional A Star with Additive Approx Bounds * Bi Directional A Star * Search Algorithms Slide Deck * Bi Directional Stopping Conditions, Piazza ’17 * Bi Directional Search Visualizations * Piazza: Landmark Example

Please refrain from referring code/psuedocode from other resources aside from these.

The Assignment

Your task is to implement several informed search algorithms that will calculate a driving route between two points in Romania with a minimal time and space cost. There is a search_submission_tests.py file to help you along the way. Your searches should be executed with minimal runtime and memory overhead.

We will be using an undirected network representing a map of Romania (and an optional Atlanta graph used for the Race!).

Grading

Points for each section are awarded based on finding the correct path and by evaluating the number of nodes explored. To track the number of times a node is explored during the search, the ExplorableGraph wrapper is used on the networkx Graph class. Every time you process a node, by calling graph[node] or graph.neighbors(node), the count for that node increases by one. You will need to use one of these methods to add a node’s neighbors to the search queue, just be careful not to call it unnecessarily throughout your code. We have created the graph.get_edge_weight(u, v) method to be used to access edge weights between two nodes, u and v. All other normal networkx Graph operations can be performed.

Visualizing the Atlanta graph:

The Atlanta graph is used in some later parts of this assignment. However, it is too big to display within a Python window like Romania. As a result, when you run the bidirectional tests in search_submission_tests.py, it generates a JSON file in the GeoJSON format. To see the graph,

you can upload it to a private GitHub Gist or use this site. If you want to see how visualize_graph.py is used, take a look at the class TestBidirectionalSearch in search_submission_tests.py

Frequently Asked Questions

If start and goal are the same, you should return [].

When nodes in the priority queue have the same priority value, break ties according to FIFO. Hint: A counter can be used to track when nodes enter the priority queue.

Your priority queue implementation should allow for duplicate nodes to enter the queue.

There is a little more to this when you get to tridirectional, so read those Notes especially carefully as well

Do not use graph.explored_nodes for anything that you submit to Gradescope. This can be used for debugging, but you should not be calling this in your code. Please make sure you read the “grading” section above.

Do not create a copy of the graph structure for any of the algorithms or compuations.

If you are stuck, check out the resources! We recognize this is a hard assignment and tri-directional search is a more researchoriented topic than the other search algorithms. Many previous students have found it useful to go through the resources in this README if they are having difficulty understanding the algorithms. Hopefully they are of some use to you all as well! <img draggable="false" role="img" class="emoji" alt="🙂" src="https://s.w.org/images/core/emoji/15.1.0/svg/1f642.svg">

We have included the “Haversine” heuristic in the search_submission_tests.py file. All of the local tests on the Atlanta map use this method. For the race, you can use whatever you choose, but know that the Atlanta map positions are (latitude, longitude). If you would like to learn more about this formula, here is a link: https://en.wikipedia.org/wiki/Haversine_formula Make sure you clean up any changes/modifications/additions you make to the networkx graph structure before you exit the search function. Depending on your changes, the auto grader might face difficulties while testing. The best alternative is to create your own data structure(s).

If you’re having problems (exploring too many nodes) with your Breadth first search implementation, one thing many students have found useful is to re-watch the Canvas videos for an optimization trick mentioned.

Most ‘NoneType object …’ errors are because the path you return is not completely connected (a pair of successive nodes in the path are not connected). Or because the path variable itself is empty.

Unit Tests

We have provided two official unit test files, and one unofficially developed one that students have found useful. They are not complete, and these tests are not guaranteed to ensure full points on the autograder, but they should help in development. To run: python

search_submission_tests.py # Basic tests, visualizes on Romania python search_submission_tests_grid.py # Visualize search on grid python search_unit_tests.py # Unofficial, checks for path correctness

Warmups

We’ll start by implementing some simpler optimization and search algorithms before the real exercises.

Warmup 1: Priority queue

[5 points]

In all searches that involve calculating path cost or heuristic (e.g. uniform-cost), we have to order our search frontier. It turns out the way that we do this can impact our overall search runtime.

To show this, you’ll implement a priority queue which will help you in understanding its performance benefits. For large graphs, sorting all input to a priority queue is impractical. As such, the data structure you implement should have an amortized O(1) insertion and O(lg n) removal time. It should do better than the naive implementation in our tests (InsertionSortQueue), which sorts the entire list after every insertion.

In this implementation of priority queue, if two elements have the same priority, they should be served according to the order in which they were enqueued (see Hint 3).

Warmup 2: BFS

[5 pts]

To get you started with handling graphs, implement and test breadth-first search over the test network.

You’ll complete this by writing the breadth_first_search() method. This returns a path of nodes from a given start node to a given end node, as a list.

For this part, it is optional to use the PriorityQueue as your frontier. You will require it from the next question onwards. You can use it here too if you want to be consistent.

Warmup 3: Uniform-cost search

[10 points]

Implement uniform-cost search, using PriorityQueue as your frontier. From now on, PriorityQueue should be your default frontier. uniform_cost_search() should return the same arguments as breadth-first search: the path to the goal node (as a list of nodes).

Notes: 1. You need to include start and goal in the path. 2. If your start and goal are the same then just return []. 3. The above are just to keep your results consistent with our test cases. 4. You can access all the neighbors of a given node by calling graph[node], or graph.neighbors(node) ONLY. 5. You can access the weight of an edge using:

graph.get_edge_weight(node_1, node_2). Not using this method will result in your explored nodes count being higher than it should be. 6. You are not allowed to maintain a cache of the neighbors for any node. You need to use the above mentioned methods to get the neighbors and corresponding weights. 7. We will provide some margin of error in grading the size of your ‘Explored’ set, but it should be close to the results provided by our reference implementation.

Warmup 4: A* search

[10 points]

Implement A* search using Euclidean distance as your heuristic. You’ll need to implement euclidean_dist_heuristic() then pass that function to a_star() as the heuristic parameter. We provide null_heuristic() as a baseline heuristic to test against when calling a_star tests.

Hint: You can find a node’s position by calling the following to check if the key is available: graph.nodes[n][‘pos’]

Notes: 1. You need to include start and goal in the path. 2. If your start and goal are the same then just return []. 3. The above are just to keep your results consistent with our test cases. 4. You can access all the neighbors of a given node by calling graph[node], or graph.neighbors(node) ONLY. 5. You can access the weight of an edge using:

graph.get_edge_weight(node_1, node_2). Not using this method will result in your explored nodes count being higher than it should be. 6. You are not allowed to maintain a cache of the neighbors for any node. You need to use the above mentioned methods to get the neighbors and corresponding weights. 7. You can access the (x, y) position of a node using: graph.nodes[n][‘pos’]. You will need this for calculating the heuristic distance. 8. We will provide some margin of error in grading the size of your ‘Explored’ set, but it should be close to the results provided by our reference implementation.

Exercises

The following exercises will require you to implement several kinds of bidirectional searches. The benefits of these algorithms over uninformed or unidirectional search are more clearly seen on larger graphs. As such, during grading, we will evaluate your performance on the map of Romania included in this assignment.

For these exercises, we recommend you take a look at the resources mentioned earlier.

Exercise 1: Bidirectional uniform-cost search

[20 points]

Implement bidirectional uniform-cost search. Remember that this requires starting your search at both the start and end states.

bidirectional_ucs() should return the path from the start node to the goal node (as a list of nodes).

Notes: 1. You need to include start and goal in the path. Make sure the path returned is from start to goal and not in the reverse order. 2. If your start and goal are the same then just return []. 3. The above are just to keep your results consistent with our test cases. 4. You can access all the neighbors of a given node by calling graph[node], or graph.neighbors(node) ONLY. 5. You can access the weight of an edge using: graph.get_edge_weight(node_1, node_2). Not using this method will result in your explored nodes count being higher than it should be. 6. You are not allowed to maintain a cache of the neighbors for any node. You need to use the above mentioned methods to get the neighbors and corresponding weights. 7. We will provide some margin of error in grading the size of your ‘Explored’ set, but it should be close to the results provided by our reference implementation. Exercise 2: Bidirectional A* search

[29 points]

Implement bidirectional A* search. Remember that you need to calculate a heuristic for both the start-to-goal search and the goal-to-start search.

To test this function, as well as using the provided tests, you can compare the path computed by bidirectional A* to bidirectional UCS search above. bidirectional_a_star() should return the path from the start node to the goal node, as a list of nodes.

Notes: 1. You need to include start and goal in the path. 2. If your start and goal are the same then just return []. 3. The above are just to keep your results consistent with our test cases. 4. You can access all the neighbors of a given node by calling graph[node], or graph.neighbors(node) ONLY. 5. You can access the weight of an edge using:

graph.get_edge_weight(node_1, node_2). Not using this method will result in your explored nodes count being higher than it should be. 6. You are not allowed to maintain a cache of the neighbors for any node. You need to use the above mentioned methods to get the neighbors and corresponding weights. 7. You can access the (x, y) position of a node using: graph.nodes[n][‘pos’]. You will need this for calculating the heuristic distance. 8. We will provide some margin of error in grading the size of your ‘Explored’ set, but it should be close to the results provided by our reference implementation. Exercise 3: Tridirectional UCS search

[12 points]

Implement tridirectional search in the naive way: starting from each goal node, perform a uniform-cost search and keep expanding until two of the three searches meet. This should be one continuous path that connects all three nodes.

Notes: 1. You need to include start and goal in the path. 2. If all three nodes are the same then just return []. 3. If there are 2 identical goals (i.e. a,b,b) then return the path [a…b] (i.e. just the path from a to b). 4. The above are just to keep your results consistent with our test cases. 5. You can access all the neighbors of a given node by calling graph[node], or graph.neighbors(node) ONLY. 6. You can access the weight of an edge using: graph.get_edge_weight(node_1, node_2). Not using this method will result in your explored nodes count being higher than it should be. 7. You are not allowed to maintain a cache of the neighbors for any node. You need to use the above mentioned methods to get the neighbors and corresponding weights. 8. We will provide some margin of error in grading the size of your ‘Explored’ set, but it should be close to the results provided by our reference implementation.

Exercise 4: Upgraded Tridirectional search

[8 points]

This is the heart of the assignment. Implement tridirectional search in such a way as to consistently improve on the performance of your previous implementation. This means consistently exploring fewer nodes during your search in order to reduce runtime. Keep in mind, we are not performing 3 bidirectional A* searches. We are searching from each of the goals towards the other two goals, in the direction that seems most promising.

The specifics are up to you, but we have a few suggestions: * Tridirectional A* * choosing landmarks and pre-computing reach values * ATL

(A*, landmarks, and triangle-inequality) * shortcuts (skipping nodes with low reach values) tridirectional_upgraded() should return a path between all three nodes.

Notes: 1. You need to include start and goal in the path. 2. If all three nodes are the same then just return []. 3. If there are 2 identical goals (i.e. a,b,b) then return the path [a…b] (i.e. just the path from a to b). 4. The above are just to keep your results consistent with our test cases. 5. You can access all the neighbors of a given node by calling graph[node], or graph.neighbors(node) ONLY. 6. You can access the weight of an edge using: graph.get_edge_weight(node_1, node_2). Not using this method will result in your explored nodes count being higher than it should be. 7. You are not allowed to maintain a cache of the neighbors for any node. You need to use the above mentioned methods to get the neighbors and corresponding weights. 8. You can access the (x, y) position of a node using: graph.nodes[n][‘pos’]. You will need this for calculating the heuristic distance. 9. We will provide some margin of error in grading the size of your ‘Explored’ set, but it should be close to the results provided by our reference implementation.

Final Task: Return your name

[1 point]

A simple task to wind down the assignment. Return your name from the function aptly called return_your_name().

The Race!

Here’s your chance to show us your best stuff. This part is mandatory if you want to compete in the race for extra credit. Implement custom_search() using whatever strategy you like. More details will be posted soon on Piazza.

Bonus points are added to the grade for this assignment, not to your overall grade.

The Race! will be based on Atlanta Pickle data.
