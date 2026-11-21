Problem Statement Develop a Python program for a Multi-Plan Telecommunications Cost Optimization System. The system evaluates multiple mobile recharge plans based on the user's data usage, call minutes, SMS usage, validity period, and budget.
The program should:

Accept customer details and usage requirements.
Accept multiple mobile plans with their prices, data limits, call limits, SMS limits, and validity.
Calculate excess charges when usage exceeds plan limits.
Check whether each plan satisfies the customer's usage and budget requirements.
Identify eligible mobile plans.
Compare the total costs of eligible plans.
Select and display the most economical eligible plan.
Display all plan details and the final recommendation.
Algorithm
Start the program.
Enter customer name.
Enter required data usage in GB.
Enter required call minutes.
Enter required SMS count.
Enter required validity in days.
Enter the customer's maximum budget.
Enter the number of mobile plans.
For each plan, enter:
Plan name.
Plan price.
Data limit.
Call minutes limit.
SMS limit.
Validity days.
Calculate excess data, call, and SMS usage.
Calculate excess charges.
Calculate the total plan cost.
Check budget and validity constraints.
Identify eligible plans.
Compare the total costs of eligible plans.
Select the plan with the lowest total cost.
Display all plan comparisons.
Display the most economical eligible plan.
If no plan is eligible, display a suitable message.
Stop.
flowchart TD

A([Start]) --> B[/Enter Customer Details/]

B --> C[/Enter Data, Calls, SMS, Validity and Budget/]

C --> D{Customer Inputs Valid?}

D -- No --> E[Display Invalid Requirements]
E --> Z([Stop])

D -- Yes --> F[/Enter Number of Mobile Plans/]

F --> G[Initialize Plan List]

G --> H[/Enter Plan Details/]

H --> I{Plan Details Valid?}

I -- No --> H

I -- Yes --> J[Calculate Excess Usage]

J --> K[Calculate Excess Charges]

K --> L[Calculate Total Plan Cost]

L --> M{Usage and Validity Satisfied?}

M -- No --> N[Mark Plan Not Eligible]

M -- Yes --> O{Within Budget?}

O -- No --> N

O -- Yes --> P[Mark Plan Eligible]

N --> Q{More Plans?}
P --> Q

Q -- Yes --> H

Q -- No --> R{Eligible Plans Available?}

R -- No --> S[Display No Eligible Plan]

R -- Yes --> T[Compare Total Costs]

T --> U[Select Lowest Cost Plan]

U --> V[Display Recommended Plan]

S --> W([Stop])
V --> W

