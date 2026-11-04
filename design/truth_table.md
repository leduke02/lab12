# Truth table for next_state

| # | alive | neighbors | next generation | why |
|---|-------|-----------|-----------------|-----|
| 1 | true  | 0 | false | underpopulation |
| 2 | true  | 1 | false | underpopulation |
| 3 | true  | 2 | true  | survives |
| 4 | true  | 3 | true  | survives |
| 5 | true  | 4 | false | overpopulation |
| 6 | true  | 5 | false | overpopulation |
| 7 | true  | 6 | false | overpopulation |
| 8 | true  | 7 | false | overpopulation |
| 9 | true  | 8 | false | overpopulation |
| 10 | false | 0 | false | stays dead |
| 11 | false | 1 | false | stays dead |
| 12 | false | 2 | false | stays dead |
| 13 | false | 3 | true  | born |
| 14 | false | 4 | false | stays dead |
| 15 | false | 5 | false | stays dead |
| 16 | false | 6 | false | stays dead |
| 17 | false | 7 | false | stays dead |
| 18 | false | 8 | false | stays dead |

18 rows = 2 states x 9 neighbor counts (0 to 8).
Live next generation only for: (alive, 2), (alive, 3), (dead, 3).
