# Hand counts

Counts are for the cells in and around each shape (0-indexed, row then col).
Everything not listed is 0.

## Middle: live cells at (4,10), (5,10), (6,10)

Hand-worked counts, rows 3 to 7, columns 9 to 11:

```
row 3: 1 1 1
row 4: 2 1 2
row 5: 3 2 3
row 6: 2 1 2
row 7: 1 1 1
```

Example: (5,10) is alive and its neighbors (4,10) and (6,10) are alive,
so its count is 2. It does not count itself. (5,9) touches all three
live cells, so its count is 3.

Program output (print_neighbor_counts), row 5: `00000000032300000000`

Result: the program agreed with my hand counts.

## Corner: live cells at (0,0), (1,0), (2,0)

Hand-worked counts, rows 0 to 4, columns 0 to 2:

```
row 0: 1 2 0
row 1: 2 3 0
row 2: 1 2 0
row 3: 1 1 0
row 4: 0 0 0
```

Example: (0,0) has only three squares on the grid next to it, and only
(1,0) is alive, so its count is 1. Squares off the edge count as dead.

Program output, row 0: `12000000000000000000`

Result: the program agreed with my hand counts.
