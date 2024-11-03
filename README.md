# CI2024_lab2

### Results

|                       | Vanuatu | Italy   | Russia   | Us       | China    |
| --------------------- | ------- | ------- | -------- | -------- | -------- |
| **InverOver Greedy1** | 1345.54 | 4258.06 | 36277.21 | 43290.64 | 62012.08 |
| **InverOver Greedy2** | 1345.54 | 4173.81 | 33503.47 | 43365.29 | -        |
| **Edge Greedy1**      | 1345.54 | 4274.79 | 35753.38 | 45396.50 | 60593.96 |
| **Edge Greedy2**      | 1345.54 | 4193.88 | 33532.21 | 41850.80 | -        |

To solve the tsp problem, there are 2 greedy algorithms to generate population: first greedy and second greedy.
First greedy is the easiest one, and it choose the nearest city in each step avoiding cycles; it's the best one for more computational expansive problem because it ends in a reasonable amount of time.
Second greedy it's much slower but it has better results. It's based on segments composed by a tuple, where the first element contains two cities and the second is the distances between the two cities. These segments are sorted by distances in an ordered way, then select for the first time the smaller distance and then tries to add a next segment if don't make the graph cyclic, otherwise go to the next and so on.
For both of the population I created 2 crossover and i just compare them.

Team mate: Davide Jannussi s331391
