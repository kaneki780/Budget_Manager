# Budget Manager

This project is a Java application designed to help users manage their personal budget effectively. The application includes features for adding income, recording purchases across various categories, viewing purchase lists, checking the balance, saving and loading purchase data, and analyzing purchase patterns.

###Key Components:
##Categories Enumeration:

The Categories enum class defines various categories of purchases: FOOD, ENTERTAINMENT, CLOTHES, and OTHER. Each category has a description and an ID for easy identification and management.

findById(int id): Returns the category corresponding to the given ID.

showAll(): Returns a string listing all categories with their IDs and descriptions.

##Main Application Logic:

The Main class is the core of the application, managing user interactions and the overall workflow.

###main(String[] args): 
The entry point of the application, displaying a menu and handling user inputs for various operations such as adding income, making purchases, viewing the balance, saving, loading, and analyzing data.
###income():
Allows the user to add income to the current balance.
###purchase():
Facilitates the addition of new purchases, categorized by type.
###list():
Displays all purchases, optionally filtered by category.
balance(): Shows the current balance.
save(): Saves the current state (balance and purchases) to a file.
load(): Loads the state from a file.
analyze(): Provides options to analyze purchases by sorting them in different ways.
Purchase Class:
The Purchase class represents an individual purchase with attributes for the name, price, and category of the purchase. It implements the Comparable interface to allow sorting based on the price.

getCategory(), getPrice(), getName(): Getter methods for purchase attributes.
compareTo(Purchase o): Compares purchases by price, enabling sorting.
toString(): Provides a formatted string representation of a purchase.
PurchaseManager Class:
The PurchaseManager class manages a collection of purchases and provides methods to manipulate and query the list.

add(Purchase p): Adds a purchase to the list.
isEmpty(): Checks if the purchase list is empty.
getCurrentSum(): Returns the total sum of all purchase prices.
clear(): Clears the list of purchases.
getPurchases(): Returns the list of purchases.
getList(Categories category): Returns a formatted string of purchases, optionally filtered by category.
getSortedList(Categories category): Returns a sorted string of purchases, optionally filtered by category.
How It Works:
The application starts by displaying a menu with options for the user. Based on the user's input, the application performs the corresponding action—such as adding income, recording a purchase, or saving the data. The user can also choose to analyze their spending habits through various sorting and categorization options. The application ensures that all data can be saved to a file and reloaded, providing persistent storage for the user's budget information.

Overall, this budget management application offers a straightforward and efficient way to track personal finances, categorize expenses, and maintain an up-to-date balance.

#Implementation

Choose your action:
1) Add income
2) Add purchase
3) Show list of purchases
4) Balance
5) Save
6) Load
7) Analyze (Sort)
0) Exit
> 6

Purchases were loaded!

Choose your action:
1) Add income
2) Add purchase
3) Show list of purchases
4) Balance
5) Save
6) Load
7) Analyze (Sort)
0) Exit
> 3

Choose the type of purchase
1) Food
2) Entertainment
3) Clothes
4) Other
5) All
6) Back
> 5

All:
Cinema $8.73
Gildan LT $8.61
Hershey's milk chocolate bars $8.54
Keystone Ground Beef $6.28
Red Fuji Apple $5.99
Eggs $3.99
Almond 250g $35.43
Almond 250g $35.43
Skate rental $30.00
FIJI Natural Artesian Water $25.98
Wrangler Men's Stretch Cargo Pant $19.97
Sensodyne Pronamel Toothpaste $19.74
Men's Dual Defense Crew Socks 12 Pairs $13.00
LEGO DUPLO Town Farm Animals $10.10
Chick-fil-A $10 Gift Card $10.00
Milk $3.50
Debt $3.50
Great Value Broccoli Florets $1.00
Total sum: $249.79

Choose the type of purchase
1) Food
2) Entertainment
3) Clothes
4) Other
5) All
6) Back
> 6

Choose your action:
1) Add income
2) Add purchase
3) Show list of purchases
4) Balance
5) Save
6) Load
7) Analyze (Sort)
0) Exit
> 4

Balance: $964.57

Choose your action:
1) Add income
2) Add purchase
3) Show list of purchases
4) Balance
5) Save
6) Load
7) Analyze (Sort)
0) Exit
> 7

How do you want to sort?
1) Sort all purchases
2) Sort by type
3) Sort certain type
4) Back
> 1

All:
Almond 250g $35.43
Almond 250g $35.43
Skate rental $30.00
FIJI Natural Artesian Water $25.98
Wrangler Men's Stretch Cargo Pant $19.97
Sensodyne Pronamel Toothpaste $19.74
Men's Dual Defense Crew Socks 12 Pairs $13.00
LEGO DUPLO Town Farm Animals $10.10
Chick-fil-A $10 Gift Card $10.00
Cinema $8.73
Gildan LT $8.61
Hershey's milk chocolate bars $8.54
Keystone Ground Beef $6.28
Red Fuji Apple $5.99
Eggs $3.99
Milk $3.50
Debt $3.50
Great Value Broccoli Florets $1.00

Total: $249.79




