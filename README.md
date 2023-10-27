# Shopping_Cart

## **THEORY**

Introduction
The "Online Grocery Store" application is designed to simulate an online grocery store where customers can view a menu of items, add them to their shopping cart, and view their total bill. This report provides an overview of the code and its functionalities.

Code Structure
The code is organized into several parts, including data structures and functions for displaying the menu, managing the shopping cart, calculating the total bill, and providing a user interface.

Data Structure
Item Structure
	struct Item represents an item available in the store.
	name (string): The name of the item.
	rate (double): The price of the item in rupees.
	quantity (int): The quantity of the item in the shopping cart.
	discount (double): The discount percentage on the item.






Working of the code explained by a case study

The user begins the shopping journey by opening the application and is greeted with a warm welcome to 'CC Grocery Store: where we fulfill your needs.' 

A menu of available items is displayed, showcasing a variety of products, each with a unique item number. The user can easily navigate through the menu, selecting items of interest and specifying the desired quantity. 

For added convenience, the user can also remove items from their cart by entering the name of the item to be removed. 

Once the shopping is complete, the user proceeds to the checkout by entering '0.' 

At this point, the application provides a summary of the items in the shopping cart, displaying their names, rates in rupees, quantities, and the total amount. 

The user's shopping journey concludes with a friendly message, either confirming the contents of the cart or expressing gratitude for visiting the store.






Functions
1. displayMenu
Purpose: Displays the menu of available items.
Output: A table-like display of items including their names, rates in rupees, and discounts.

2. addItemToCart
Purpose: Adds an item to the shopping cart.
Input: Item number and quantity.
Output: Updates the shopping cart with the selected item and its quantity.

3. removeItemFromCart
Purpose: Removes an item from the shopping cart.
Input: Item name.
Output: Removes the specified item from the shopping cart.

4. calculateTotalBill
Purpose: Calculates the total bill based on items in the shopping cart.
Output: Returns the total bill amount in rupees.

5. displayCart
Purpose: Displays the contents of the shopping cart and the total bill.
Output: A table-like display of items in the cart, including their names, rates, quantities, and total amounts.

6. main
Purpose: The main function that manages the user interface
The user can add items to the cart, remove items, and view the total bill. The user exits the application when ready.

User Interface
The user interface is primarily a text-based interaction where the user selects items by entering their corresponding numbers and quantities. 
The options include:
	Adding items to the cart (enter item number and quantity).
	Removing items from the cart (enter the name of the item).
	Checking out (0) to complete the transaction.
Important Points
•	The code is designed to handle prices in rupees (₹) and allows decimal values for precise calculations.
•	Discounts are represented as percentages (e.g., 5% discount).
•	The user is guided through the shopping process using a simple menu-driven interface.
•	The application terminates when the user chooses to check out (enters 0).
•	The code includes sample data for three items; additional items can be added to the menu.

## **Conclusion**
The "Online Grocery Store" application provides a user-friendly interface for customers to shop for groceries, view their cart, and calculate their total bill. The code structure, functions, and user interface make it a convenient simulation of an online grocery store.


![image](https://github.com/RitvikArora22070123094/Shopping_Cart/assets/139522395/ee1b20f1-555f-4c4b-a7bd-c1e510f06991)
![image](https://github.com/RitvikArora22070123094/Shopping_Cart/assets/139522395/2ad7643c-fd75-4d4d-b52d-92d456d12e63)
![image](https://github.com/RitvikArora22070123094/Shopping_Cart/assets/139522395/2a895e73-7eea-47b5-af81-ad9ac7a006e3)
![image](https://github.com/RitvikArora22070123094/Shopping_Cart/assets/139522395/60e91c91-952b-47a2-9367-fc3396f606ea)
![image](https://github.com/RitvikArora22070123094/Shopping_Cart/assets/139522395/11886c93-ef31-4898-90fc-d636558d3084)
![image](https://github.com/RitvikArora22070123094/Shopping_Cart/assets/139522395/bb8ea1b4-38c0-4daa-80ea-8b04e5adcd6e)


![image](https://github.com/RitvikArora22070123094/Shopping_Cart/assets/139522395/8cc57d30-74f7-4546-9d46-b9dda8853638)
![image](https://github.com/RitvikArora22070123094/Shopping_Cart/assets/139522395/f6d71e8b-f533-4bf8-9e3b-3163a2d3e0ba)




