# Offsets (dr, dc) from the middle cell

dr = change in row (negative is up, positive is down)
dc = change in column (negative is left, positive is right)

```
+---------+---------+---------+
| (-1,-1) | (-1, 0) | (-1,+1) |
+---------+---------+---------+
| ( 0,-1) |  XXXXX  | ( 0,+1) |
+---------+---------+---------+
| (+1,-1) | (+1, 0) | (+1,+1) |
+---------+---------+---------+
```

The middle square is the cell itself, offset (0, 0). It is crossed out
because a cell is not its own neighbor.

That leaves 8 neighbors. In Task 7, count_neighbors loops dr and dc
over -1, 0, 1, skips (0, 0), and adds each offset to (row, col).
