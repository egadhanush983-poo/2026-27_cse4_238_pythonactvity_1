
Retail Billing with Multiple Discount Rules
The program should:
Accept customer details.
Accept multiple product names, categories, prices, and quantities.
Calculate the subtotal for each product.
Apply category-specific taxes.
Apply threshold-based discounts depending on the total purchase amount.
Apply maximum concession limits to prevent excessive discounts.
Calculate the final payable amount.
Generate and display an itemized invoice with product details, taxes, discounts, and total bill.
Algorithm

Start the program.

Enter customer name.

Enter the number of products.

For each product, enter:

Product name.
Product category.
Product price.
Product quantity.
Validate product details and quantities.

Calculate the subtotal for each product. Subtotal = Product Price × Quantity

Calculate category-specific tax:

Electronics: 18%
Clothing: 5%
Groceries: 3%
Furniture: 12%
Calculate total subtotal and total tax.

Apply threshold-based discounts:

Purchase above ₹5,000: 5% discount.
Purchase above ₹10,000: 10% discount.
Purchase above ₹20,000: 15% discount.
Apply a maximum discount limit of ₹2,000.

Calculate the final bill. Final Bill = Subtotal + Tax − Discount

Display the itemized invoice.

Stop flowchart TD

A([Start]) --> B[/Enter Customer Name and Number of Products/]

B --> C{Customer Details Valid?}

C -- No --> D[Display Invalid Details] D --> Z([Stop])

C -- Yes --> E[/Enter Product Name, Category, Price and Quantity/]

E --> F{Product Details Valid?}

F -- No --> G[Display Invalid Product Details]

F -- Yes --> H[Calculate Product Subtotal]

H --> I[Calculate Category-Specific Tax]

I --> J[Add Subtotal and Tax to Totals]

G --> K{More Products?} J --> K

K -- Yes --> E

K -- No --> L{Purchase Subtotal?}

L -- Above 20000 --> M[Apply 15% Discount] L -- Above 10000 --> N[Apply 10% Discount] L -- Above 5000 --> O[Apply 5% Discount] L -- 5000 or Below --> P[No Discount]

M --> Q[Check Maximum Discount Limit] N --> Q O --> Q P --> Q

Q --> R[Apply Maximum Discount of 2000]

R --> S[Calculate Final Bill]

S --> T[Generate Itemized Invoice]

T --> U[/Display Final Bill/]

U --> Z([Stop])


