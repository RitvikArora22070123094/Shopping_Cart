/*22070123094
Shopping_Cart_Mini_Project*/
#include <iostream>
#include <iomanip>
#include <vector>
using namespace std;

// Structure to represent an item
struct Item {
    string name;
    double rate; // Rate in Rupees
    int quantity;
    double discount;
};

// Function to display the menu
void displayMenu(const vector<Item>& items) {
    cout << "****************** Menu ******************" << endl;
    cout << "Item No.  Name             Rate (₹)   Discount" << endl;
    cout << "----------------------------------------" << endl;
    for (int i = 0; i < items.size(); i++) {
        cout << setw(5) << i + 1 << setw(9) << items[i].name << setw(15) << "₹" << items[i].rate << setw(12) << items[i].discount << "%" << endl;
    }
    cout << "----------------------------------------" << endl;
}

// Function to add an item to the cart
void addItemToCart(vector<Item>& cart, const vector<Item>& items, int itemNo, int quantity) {
    itemNo--; // Adjust for 0-based indexing
    if (itemNo >= 0 && itemNo < items.size() && quantity > 0) {
        cart.push_back(items[itemNo]);
        cart.back().quantity = quantity;
        cout << quantity << " " << items[itemNo].name << " added to the cart." << endl;
    } else {
        cout << "Invalid item selection or quantity." << endl;
    }
}

// Function to remove an item from the cart
void removeItemFromCart(vector<Item>& cart, const string& itemName) {
    for (auto it = cart.begin(); it != cart.end(); ++it) {
        if (it->name == itemName) {
            cout << it->name << " removed from the cart." << endl;
            cart.erase(it);
            return;
        }
    }
    cout << "Item not found in the cart." << endl;
}

// Function to calculate the total bill
double calculateTotalBill(const vector<Item>& cart) {
    double total = 0;
    for (const Item& item : cart) {
        double discountedRate = item.rate - (item.rate * item.discount / 100);
        total += discountedRate * item.quantity;
    }
    return total;
}

// Function to display the cart and the total bill
void displayCart(const vector<Item>& cart) {
    cout << "************ Your Shopping Cart ************" << endl;
    cout << "Item       Rate (₹)   Quantity    Amount (₹)" << endl;
    cout << "----------------------------------------" << endl;
    for (const Item& item : cart) {
        double discountedRate = item.rate - (item.rate * item.discount / 100);
        cout << setw(10) << item.name << setw(15) << "₹" << item.rate << setw(11) << item.quantity << setw(12) << fixed << setprecision(2) << "₹" << discountedRate * item.quantity << endl;
    }
    cout << "----------------------------------------" << endl;
    cout << "Total Bill: ₹" << calculateTotalBill(cart) << endl;
    cout<<"thank you for visiting!\nWe hope to serve you in the future!"<<endl;
}

int main() {
    cout << "Welcome to CC Grocery Store: Where We Fulfill Your Needs" << endl;
    
    vector<Item> items = {
        {"Item1", 10.99, 0, 5},
        {"Item2", 7.99, 0, 0},
        {"Item3", 15.99, 0, 10},
        {"Item4", 12.49, 0, 3},
        {"Item5", 8.99, 0, 5},
        {"Item6", 19.99, 0, 7},
        {"Item7", 5.99, 0, 2},
        {"Item8", 6.49, 0, 0},
        {"Item9", 17.99, 0, 8},
        {"Item10", 14.99, 0, 4},
        {"Item11", 9.99, 0, 6},
        {"Item12", 13.99, 0, 5},
        {"Item13", 16.99, 0, 10},
        {"Item14", 18.99, 0, 5},
        {"Item15", 6.99, 0, 0},
        {"Item16", 7.49, 0, 3},
        {"Item17", 11.99, 0, 8},
        {"Item18", 8.49, 0, 2},
        {"Item19", 4.99, 0, 0},
        {"Item20", 20.99, 0, 7}
    };

    vector<Item> cart;

    while (true) {
        displayMenu(items);
        int choice;
        cout << "Enter item number to add to cart (0 to checkout, -1 to remove an item): ";
        cin >> choice;
        if (choice == 0) {
            break;
        } else if (choice == -1) {
            string itemName;
            cout << "Enter the name of the item to remove: ";
            cin >> itemName;
            removeItemFromCart(cart, itemName);
        } else {
            int quantity;
            cout << "Enter quantity: ";
            cin >> quantity;
            addItemToCart(cart, items, choice, quantity);
        }
    }

    if (cart.empty()) {
        cout << "Your cart is empty. Thank you for visiting!" << endl;
    } else {
        displayCart(cart);
    }

    return 0;
}

/*OUTPUT
Welcome to CC Grocery Store: Where We Fulfill Your Needs
****************** Menu ******************
Item No.  Name             Rate (Γé╣)   Discount
----------------------------------------
    1    Item1            Γé╣10.99           5%
    2    Item2            Γé╣7.99           0%
    3    Item3            Γé╣15.99          10%
    4    Item4            Γé╣12.49           3%
    5    Item5            Γé╣8.99           5%
    6    Item6            Γé╣19.99           7%
    7    Item7            Γé╣5.99           2%
    8    Item8            Γé╣6.49           0%
    9    Item9            Γé╣17.99           8%
   10   Item10            Γé╣14.99           4%
   11   Item11            Γé╣9.99           6%
   12   Item12            Γé╣13.99           5%
   13   Item13            Γé╣16.99          10%
   14   Item14            Γé╣18.99           5%
   15   Item15            Γé╣6.99           0%
   16   Item16            Γé╣7.49           3%
   17   Item17            Γé╣11.99           8%
   18   Item18            Γé╣8.49           2%
   19   Item19            Γé╣4.99           0%
   20   Item20            Γé╣20.99           7%
----------------------------------------
Enter item number to add to cart (0 to checkout, -1 to remove an item): 1
Enter quantity: 2
2 Item1 added to the cart.
****************** Menu ******************
Item No.  Name             Rate (Γé╣)   Discount
----------------------------------------
    1    Item1            Γé╣10.99           5%
    2    Item2            Γé╣7.99           0%
    3    Item3            Γé╣15.99          10%
    4    Item4            Γé╣12.49           3%
    5    Item5            Γé╣8.99           5%
    6    Item6            Γé╣19.99           7%
    7    Item7            Γé╣5.99           2%
    8    Item8            Γé╣6.49           0%
    9    Item9            Γé╣17.99           8%
   10   Item10            Γé╣14.99           4%
   11   Item11            Γé╣9.99           6%
   12   Item12            Γé╣13.99           5%
   13   Item13            Γé╣16.99          10%
   14   Item14            Γé╣18.99           5%
   15   Item15            Γé╣6.99           0%
   16   Item16            Γé╣7.49           3%
   17   Item17            Γé╣11.99           8%
   18   Item18            Γé╣8.49           2%
   19   Item19            Γé╣4.99           0%
   20   Item20            Γé╣20.99           7%
----------------------------------------
Enter item number to add to cart (0 to checkout, -1 to remove an item): 3
Enter quantity: 4
4 Item3 added to the cart.
****************** Menu ******************
Item No.  Name             Rate (Γé╣)   Discount
----------------------------------------
    1    Item1            Γé╣10.99           5%
    2    Item2            Γé╣7.99           0%
    3    Item3            Γé╣15.99          10%
    4    Item4            Γé╣12.49           3%
    5    Item5            Γé╣8.99           5%
    6    Item6            Γé╣19.99           7%
    7    Item7            Γé╣5.99           2%
    8    Item8            Γé╣6.49           0%
    9    Item9            Γé╣17.99           8%
   10   Item10            Γé╣14.99           4%
   11   Item11            Γé╣9.99           6%
   12   Item12            Γé╣13.99           5%
   13   Item13            Γé╣16.99          10%
   14   Item14            Γé╣18.99           5%
   15   Item15            Γé╣6.99           0%
   16   Item16            Γé╣7.49           3%
   17   Item17            Γé╣11.99           8%
   18   Item18            Γé╣8.49           2%
   19   Item19            Γé╣4.99           0%
   20   Item20            Γé╣20.99           7%
----------------------------------------
Enter item number to add to cart (0 to checkout, -1 to remove an item): 0
************ Your Shopping Cart ************
Item       Rate (Γé╣)   Quantity    Amount (Γé╣)
----------------------------------------
     Item1            Γé╣10.99          2         Γé╣20.88
     Item3            Γé╣15.99          4         Γé╣57.56
----------------------------------------
Total Bill: Γé╣78.44
thank you for visiting!
We hope to serve you in the future!
*/
