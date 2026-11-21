
Campus Event Financial Planning – Python Program
The program should calculate the costs of:1. Venue charges 2. Equipment charges 3. Catering charges 4. Transportation charges 5. Certificate charges The program should also:
Calculate the total event cost.
Calculate the sponsorship amount received.
Identify the sponsorship shortfall.
Calculate the participant contribution.
Determine the minimum number of registrations required to break even.
Display whether the event makes a profit or incurs a loss.
Algorithm
Start the program.
Enter venue cost.
Enter equipment cost.
Enter catering cost per participant.
Enter transport cost.
Enter certificate cost per participant.
Enter expected number of participants.
Enter sponsorship amount.
Calculate fixed costs (venue + equipment + transport).
Calculate variable costs (catering + certificates).
Calculate total event cost.
Calculate sponsorship shortfall.
Calculate participant contribution per person.
Calculate minimum registrations required to break even.
Display all financial details.
Stop the program.
flowchart TD

A([Start]) --> B[Display Event Financial Planning]

B --> C[/Enter Venue Cost/]

C --> D[/Enter Equipment Cost/]

D --> E[/Enter Transport Cost/]

E --> F[/Enter Catering Cost per Participant/]

F --> G[/Enter Certificate Cost per Participant/]

G --> H[/Enter Expected Participants/]

H --> I[/Enter Sponsorship Amount/]

I --> J[/Enter Registration Fee/]

J --> K{Are Inputs Valid?}

K -- No --> L[Display Invalid Input]

L --> Z([End])

K -- Yes --> M[Calculate Fixed Cost]

M --> N[Calculate Variable Cost]

N --> O[Calculate Total Event Cost]

O --> P[Calculate Sponsorship Shortfall]

P --> Q[Calculate Participant Contribution]

Q --> R[Calculate Minimum Break Even Registrations]

R --> S[Calculate Total Income]

S --> T{Income Greater Than Cost?}

T -- Yes --> U[Display Profit]

T -- No --> V{Income Less Than Cost?}

V -- Yes --> W[Display Loss]

V -- No --> X[Display Break Even]

U --> Y[Display Financial Report]

W --> Y

X --> Y

Y --> Z([End])

