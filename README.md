# Path-Planning-of-Robot
This project is about developing path planning ability for a robot in an environment of obstacles.

The picture below shows the game world. The black grids are obstacles and the coloured grids are objects. The agent tries to find the optimum path between two identical objects without hitting other objects and obstacles.

![image4](images/test_image4.jpg)

The output of the code is given below. The `Occupied Grids` shows the grids occupied by the obstacles and the objects. `Planned Path` shows the path between two identical objects and the path through which they connect without hitting any other object or obstacle. It also gives number of blocks to move  When the algorithm does not find any match for an object, then it says `NO MATCH`.

Output:

`
Path Planning of Robot!
`

`
Occupied Grids : `
`
[(1, 2), (1, 3), (1, 4), (1, 5), (2, 2), (2, 4), (3, 2), (3, 3), (3, 4), (3, 5), (3, 9), (4, 1), (4, 3), (5, 6), (5, 7), (6, 2), (6, 5), (6, 7), (6, 8), (7, 1), (7, 5), (7, 6), (7, 8), (8, 3), (8, 5), (8, 8), (9, 2), (9, 5), (9, 8), (9, 9), (10, 5)]
`
`
Planned Path :`
`
{(3, 4): ['(8, 3)', [(3, 4), (4, 4), (5, 4), (6, 4), (6, 3), (7, 3), (8, 3)], 7], (3, 9): ['(7, 6)', [(3, 9), (4, 9), (4, 8), (4, 7), (4, 6), (4, 5), (5, 5), (5, 4), (6, 4), (7, 4), (8, 4), (8, 5), (9, 5), (9, 6), (9, 7), (9, 8), (10, 8), (10, 9), (10, 10), (9, 10), (8, 10), (7, 10), (7, 9), (7, 8), (7, 7), (7, 6)], 26], (4, 1): ['(9, 2)', [], 0], (4, 3): ['(7, 1)', [(4, 3), (4, 4), (5, 4), (6, 4), (6, 3), (6, 2), (6, 1), (7, 1)], 8], (6, 2): ['(8, 5)', [(6, 2), (6, 3), (6, 4), (7, 4), (8, 4), (8, 5)], 6], (7, 1): ['(4, 3)', [(7, 1), (7, 2), (7, 3), (6, 3), (6, 4), (5, 4), (4, 4), (4, 3)], 8], (7, 6): ['(3, 9)', [(7, 6), (7, 7), (7, 8), (7, 9), (7, 10), (8, 10), (9, 10), (10, 10), (10, 9), (10, 8), (9, 8), (9, 7), (9, 6), (9, 5), (8, 5), (8, 4), (7, 4), (6, 4), (5, 4), (5, 5), (4, 5), (4, 6), (4, 7), (4, 8), (4, 9), (3, 9)], 26], (8, 3): ['(3, 4)', [(8, 3), (8, 4), (7, 4), (6, 4), (5, 4), (4, 4), (3, 4)], 7], (8, 5): ['(6, 2)', [(8, 5), (8, 4), (7, 4), (6, 4), (6, 3), (6, 2)], 6], (9, 2): ['(4, 1)', [], 0], (2, 4): ['NO MATCH', [], 0], (3, 5): ['NO MATCH', [], 0], (5, 7): ['NO MATCH', [], 0]}
`