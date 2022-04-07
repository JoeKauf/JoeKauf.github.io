[Back to Portfolio](./)

Restaurant Menu
===============

-   **Class: CSCI 325** 
-   **Grade: A** 
-   **Language(s): Java** 
-   **Source Code Repository: https://github.com/JoeKauf/CSCIRestaurantMenu** [features/mastering-markdown](https://guides.github.com/features/mastering-markdown/)  
    (Please [email me](mailto:example@csustudent.net?subject=GitHub%20Access) to request access.)

## Project description

When the program starts, the user is prompted to choose a restaurant they would like to order from. Once the user picks the restaurant, they are asked if they would like to view the previous reviews on that certain restaurant. If the user enters ‘Y’ (for yes) then the reviews are printed from a text file, which has all the previous reviews in it, and the menu is printed for the user to select the items they would like to order. If the user enters ‘N’ (for no) then the program goes straight to printing the menu (all pulled from text files). 

Once the menu is printed, the user can go through and select the menu items that they would like to add to their order. After each selection by the user, they will have the option to add a customization to that item, such as adding cheese, ketchup, etc. When the user is done with the order, they can enter ‘$’ and the program moves on to the checkout screen. The user will then see all the items they selected and the prices of those items including all customizations. On the checkout screen, an options menu will be printed where the user can choose to execute certain tasks (by entering with a char variable) before making their payment, such as adding or removing an item, editing a customization, or proceed to checkout.

When the user chooses to move to the checkout and complete an order, they will be prompted to add a tip by entering either ‘Y’ or ‘N’. If the user chooses ‘N’ then the receipt including the subtotal, tax, and total will be printed. If ‘Y’ the user will be asked how much tip they would like to add. The tip is then added to the total cost. Next, the payment info screen will appear and the user can select their method of payment and enter their payment credentials. When the user is finished entering their payment info, they will have the option to finalize the payment (entering ‘f’), go back (entering ‘b’), or cancel (entering ‘c’) the order. If the user finalized the payment, the user will be notified if the payment was completed or not.

Lastly, after the order is complete for a certain restaurant, the user will be asked if they would like to leave a review on the restaurant. If ‘Y’ is entered, then the user can leave a rating and a text review that will be stored in a text file for other users to view later on if desired. If ‘N’ is entered, the program will move on to the next prompt. The user can either enter ‘e’ to successfully end the program, or enter ‘o’ to make another order. If ‘o’ is entered, the entire program will loop back to the beginning and allow another order to be made.




## How to compile and run the program

How to compile (if applicable) and run the project.

```bash
cd ./project
python setup.py
```

If the programming language does not require compilation, the update the heading to be “How to run the program.” If your application is deployed on a remote service, including instructions on how to deploy it.

## UI Design

This program uses a command line interface. The program outputs a menu and the user will interact with it by entering in responses based upon the screen's prompts.

Lorem ipsum dolor sit amet (see Fig 1), consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat (see Fig 2). Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum (see Fig 3).

![screenshot](images/dummy_thumbnail.jpg)  
Fig 1. The launch screen

![screenshot](images/dummy_thumbnail.jpg)  
Fig 2. Example output after input is processed.

![screenshot](images/dummy_thumbnail.jpg)  
Fig 3. Feedback when an error occurs.

## 3. Additional Considerations

This program does not seek to connect nor can connect with APIs. 

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

[Back to Portfolio](./)
