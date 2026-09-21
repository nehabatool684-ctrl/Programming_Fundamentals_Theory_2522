## IPO Chart

| Input | Process | Output |
|---|---|---|
| Number of floor requests `N` | Let `currentFloor = 0` | Motion message for each request |
| Requested floor | Compare requested floor with current floor | `"Moving Up"` |
| | If requested floor > current floor | `"Moving Down"` |
| | If requested floor < current floor | `"Doors Opening"` |
| | If requested floor = current floor | Updated current floor |
| | Update `currentFloor = requestedFloor` after each stop | |
| | Repeat the process for all `N` requests times | |

## PAC Chart

| Item | Description |
|---|---|
| Problem | Process elevator floor requests and determine the elevator's motion |
| Input | Number of floor requests as (N) |
| Input | Requested floor for each request |
| Initial Value | `currentFloor = 0` |
| Loop | Repeat for N floor requests |
| Condition 1 | If `requestedFloor > currentFloor` → Display "Moving Up" |
| Condition 2 | If `requestedFloor < currentFloor` → Display "Moving Down" |
| Condition 3 | If `requestedFloor = currentFloor` → Display "Doors Opening" |
| Update | `currentFloor = requestedFloor` after each stop |
| Output | Movement message for each floor request |
| Final Output | Current floor after processing each request |
