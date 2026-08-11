DAY_4

Algorithm: Rotten Oranges using BFS

In this problem, we are given a grid containing three types of cells: 0 represents an empty orange. 1 represents a fresh orange. 2 represents a rotten orange. Our goal is to find the minimum number of minutes required for all the fresh oranges to become rotten.

I will use the concept of BFS (Breadth-First Search) because, the oranges become rotten level by level and each level represents one minute. First, I will go through the complete grid and count the number of fresh oranges. At the same time, whenever I find a rotten orange (2) I will store its position in a queue. Since, there can be more than one rotten orange at the beginning, all the rotten oranges will be added to the queue before starting the BFS.

After that I will start the BFS process by taking the first rotten orange from the queue. I will check its four neighbouring cells: up, down, left, and right. If any of these neighbouring cells contains a fresh orange (1) that orange will become rotten. I will change its value from 1 to 2 decrease the count of fresh oranges and add its position to the queue. The newly rotten oranges are then processed in the same way.

Once all the currently rotten oranges have been processed the newly rotten oranges will be processed in the next round. This represents one minute passing. I will continue this process until the queue becomes empty. In this way, BFS spreads the rotten oranges through the grid level by level, just like the rot spreading from one orange to its neighbouring oranges.

Finally, I will check whether any fresh oranges are still left. If there are fresh oranges remaining it means they could not be reached by any rotten orange, so the answer will be -1. If there are no fresh oranges left. I will return the total number of minutes taken to make all the fresh oranges rotten.