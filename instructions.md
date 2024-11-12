# Instructions  

Given an m x n 2D binary grid which represents a map of '1's (land) and '0's (water), return the number of **unique** island **shapes**.

An island is surrounded by water and is formed by connecting adjacent lands horizontally or vertically. You may assume all four edges of the grid are all surrounded by water.

An island shape is the shape an island takes, e.g., 3x2 rectangle, 2x2 L-shape, etc. Islands that have the same shape but which are either *rotations* or *mirror images* of each other are considered to have the same **unique** shape. 

### Example 1:

**Input**: 

    grid = [[1,1,0,1,1,0],
            [1,1,0,0,0,0],
            [1,1,0,1,1,1],
            [0,0,0,1,1,1]]
  
**Output**: 2

**Reasoning**: There are 3 islands but 2 of the islands have the same unique island shape because a 2x3 rectangle can be rotated to become a 3x2 rectangle. So there are just 2 unique island shapes in the grid.

### Example 2:

**Input**: 

    grid = [[1,1,0,1,1],
            [1,0,0,0,1],
            [0,0,0,1,0],
            [0,0,0,1,1]]
            
**Output**: 1

**Reason**: All 3 islands are versions of the same island shape, i.e., a 2x2 L-shape. They are either rotations or mirror images of each other. So there is only 1 unique island shape in the grid.

### Constraints:

    m == grid.length
    n == grid[i].length
    1 <= m, n <= 300
    grid[i][j] is '0' or '1'.

