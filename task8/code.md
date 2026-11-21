
Manufacturing Cost and Profitability Analysis
The program should:
Accept product name and production quantity.

Accept raw material cost per unit.

Calculate labour charges.

Calculate material wastage costs.

Calculate machine operating costs.

Calculate the total manufacturing cost.

Calculate the selling price and total revenue.

Calculate profit or loss.

Compare the actual profit with a specified profit target.

Display whether the production meets the required profit target.

Algorithm Start the program.
Enter product name.

Enter production quantity.

Enter raw material cost per unit.

Enter labour cost per unit.

Enter wastage percentage.

Enter machine cost per unit.

Enter selling price per unit.

Enter the required profit target percentage.

Validate all input values.

Calculate total material cost.

Material Cost = Material Cost per Unit × Quantity

Calculate total labour cost.
Labour Cost = Labour Cost per Unit × Quantity

Calculate wastage cost.
Wastage Cost = Material Cost × Wastage Percentage / 100

Calculate machine cost.
Machine Cost = Machine Cost per Unit × Quantity

Calculate total manufacturing cost.
Total Cost = Material Cost + Labour Cost + Wastage Cost + Machine Cost

Calculate total sales revenue.
Revenue = Selling Price per Unit × Quantity

Calculate profit or loss.
Profit = Revenue − Total Manufacturing Cost

Calculate profit percentage.
Profit Percentage = (Profit / Total Manufacturing Cost) × 100

Compare actual profit percentage with the target percentage.

Display whether the production meets the profit target.

Display the complete manufacturing report.

Stop. flowchart TD

A([Start]) --> B[/Enter Product Name and Quantity/]

B --> C[/Enter Material, Labour, Wastage and Machine Costs/]

C --> D[/Enter Selling Price and Target Profit Percentage/]

D --> E{All Inputs Valid?}

E -- No --> F[Display Invalid Input]
F --> Z([Stop])

E -- Yes --> G[Calculate Material Cost]

G --> H[Calculate Labour Cost]

H --> I[Calculate Wastage Cost]

I --> J[Calculate Machine Cost]

J --> K[Calculate Total Manufacturing Cost]

K --> L[Calculate Total Sales Revenue]

L --> M[Calculate Profit or Loss]

M --> N[Calculate Profit Percentage]

N --> O{Profit Meets Target?}

O -- Yes --> P[Profit Target Achieved]

O -- No --> Q{Is Profit Positive?}

Q -- Yes --> R[Profit Target Not Achieved]

Q -- No --> S{Profit Equals Zero?}

S -- Yes --> T[No Profit No Loss]

S -- No --> U[Production Resulted in Loss]

P --> V[Generate Manufacturing Report]
R --> V
T --> V
U --> V

V --> W[/Display Cost and Profit Details/]

W --> Z([Stop])

