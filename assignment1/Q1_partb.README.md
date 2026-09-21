# Hotel Booking System

## IPO Chart

| Input | Process | Output |
|---|---|---|
| Number of guests (N) | Repeat for N guests | Final price for each guest |
| Season (Peak / Off-Peak) | Determine rate based on season | Hotel Total Revenue |
| Room type (Standard / Deluxe / Suite) | Determine rate based on room type | |
| Number of nights | Calculate price = rate × nights | |
| | If nights > 7, apply 15% discount | |
| | Calculate final price | |
| | Add final price to total revenue | |

## PAC Chart


| **Component** | **Description** |
| :--- | :--- |
| **Problem (P)** | To process booking for N guests and calculate final price per guest and total hotel revenue using nested season + room type logic and long-stay discount. |
| **Input (I)** | N = Number of guests <br> For each guest: <br> - season = Peak / Off-Peak <br> - roomType = Standard / Deluxe / Suite <br> - nights = Number of nights stayed |
| **Processing (P)** | 1. Initialize hotelRevenue = 0 <br> 2. FOR i = 1 to N DO: <br> &nbsp;&nbsp;a) Nested IF for Rate: <br> &nbsp;&nbsp;&nbsp;&nbsp; IF season == Peak <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; IF room == Standard => 5000 <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ELSE IF Deluxe => 8000 <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ELSE Suite => 12000 <br> &nbsp;&nbsp;&nbsp;&nbsp; ELSE // Off-Peak <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; IF Standard => 3000 <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ELSE IF Deluxe => 5000 <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ELSE Suite => 8000 <br> &nbsp;&nbsp;b) total = rate * nights <br> &nbsp;&nbsp;c) IF nights > 7 THEN discount = total * 0.15 ELSE discount = 0 <br> &nbsp;&nbsp;d) finalPrice = total - discount <br> &nbsp;&nbsp;e) hotelRevenue += finalPrice <br> 3. End Loop |
| **Output (O)** | - Final Price for each Guest <br> - Hotel Total Revenue after loop |
| **Formulas** | Total = Rate × Nights <br> Final = Total - Discount (if Nights > 7) <br> Hotel Revenue = Sum(Final Prices) |

