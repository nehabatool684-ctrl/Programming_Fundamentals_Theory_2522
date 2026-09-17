## IPO Chart

| Input | Process | Output |
|---|---|---|
| Quantity `q` | Validate quantity | Error message if input is invalid |
| Price per item `p` | Validate price | Error message if input is invalid |
| Discount percentage `d` | Validate discount percentage | Error message if input is invalid |
| Tax percentage `t` | Validate tax percentage | Error message if input is invalid |
| | Calculate Subtotal: `s = q × p` | Subtotal |
| | Calculate Discounted Amount: `a = s - (s × d) / 100` | Discounted Amount |
| | Calculate Final Bill: `Final Bill = a + (a × t) / 100` | Final Bill |
| | Store calculation details | Bill document |
| | Generate bill document | Final bill displayed to customer |
| | Display final bill | |

## PAC Chart

| Item | Description |
|---|---|
| Problem | Calculate and display the final shopping bill after discount and tax calculations |
| Input | Quantity `q` |
| Input | Price per item `p` |
| Input | Discount percentage `d` |
| Input | Tax percentage `t` |
| Validation | Check that all entered values are valid |
| Invalid Input | Display an appropriate error message and terminate the calculation |
| Subtotal | `s = q × p` |
| Discounted Amount | `a = s - (s × d) / 100` |
| Final Bill | `Final Bill = a + (a × t) / 100` |
| Storage | Store the calculation details |
| Document | Create a bill document |
| Output | Display the final bill to the customer |
| End | Stop the program after displaying the bill |
