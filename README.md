# Capstone Project 3
This is the thrid major project required as part of the Software Engineering Bootcamp by Hyperiondev.com
It is meant to demonstrate the cumulative skills of the student up and until this point.

###### Instructions
Follow these steps:
* Code a Python program that will read from the text file inventory.txt and perform the following on the data, to prepare for presentation to your managers:
    * We’ve provided a template for you in a file named inventory.py.
    * Inside this file, you will find a class named Shoe with the following attributes:
        * country,
        * code,
        * product,
        * cost, and
        * quantity.
    * Inside this class define the following methods:
        * get_cost - Returns the cost of the shoes.
        * get_quantity - Returns the quantity of the shoes.
        * __str__ - This method returns a string representation of a class.
    * Outside this class create a variable with an empty list. This variable will be used to store a list of shoes objects
    * Then you must define the following functions outside the class:
        * read_shoes_data - This function will open the file inventory.txt and read the data from this file, then create a shoes object with this data and append this object into the shoes list. One line in this file represents data to create one object of shoes. You must use the try-except in this function for error handling. Remember to skip the first line using your code.
        * capture_shoes - This function will allow a user to capture data about a shoe and use this data to create a shoe object and append this object inside the shoe list.
        * view_all - This function will iterate over the shoes list and print the details of the shoes returned from the __str__ function. Optional: you can organise your data in a table format by using Python’s tabulate module.
        * re_stock - This function will find the shoe object with the lowest quantity, which are the shoes that need to be re-stocked. Ask the user if they want to add this quantity of shoes and then update it. This quantity should be updated on the file for this shoe.
        * search_shoe - This function will search for a shoe from the list using the shoe code and return this object so that it will be printed.
        * value_per_item - This function will calculate the total value for each item . Please keep the formula for value in mind; value = cost * quantity. Print this information on the console for all the shoes.
        * highest_qty - Write code to determine the product with the highest quantity and print this shoe as being for sale.
    * Now in your main create a menu that executes each function above. This menu should be inside the while loop. Be creative!

## Table of Contents
* Installation guide
* User guide

## Installation guide
This program is based in Python. Ensure that you have the latest version of Python installed on your PC to run the program.
For the latest version visit https://www.python.org/downloads/ 

This program makes use of Pillow, Tkinter and Sqlite3. All packages should be included with the installation of Python.

If you are running this program in an environment, please ensure that you have also install the packages using the installation commands.

## User guide
User is able to make selection by clicking on the appropriate icon.
* View Inventory - Shows all items listed in the inventory
* Search Item - Allows user to search for an item using specified creteria
* Add item - Allows user to add item to inventory
* Stock Value - Shows the stock value for all the items in the inventory
* On Sale - Shows the item with the highest quantity
* Restock Item - Shows the item with the lowest quantity, allows user the increase the amount and refresh 

Exit button - will close/exit the program

###### View Inventory
This window display a list of all the items in the inventory.
The user is can make changes to the data base and use the "Update Inventory" button to capture any changes.

Buttons:
Refresh List: Allows user to refresh the list after making alterations.
Add Item: will open the Add Item window
Update Inventory: Will capture any changes that the user has made to the inventory document

Back: closes current window
Exit: will exit/close the program

###### Search Item
This window allows user to search for specific item in inventory.
User is not able to alter/change any data from this window.

User must enter search criteria into relevant field. (note - only enter data into one field at a time)
Once the user has enter the search criteria, click on "Search"; this will display list of items that matches the search criteria.

Buttons:
Clear: Will clear all fields (not search history)
Search: Will return items that matches the search criteria

Back: closes current window
Exit: will exit/close the program

###### Add Item
This window will allow the user to add an item to the inventory.

User must complete all fields. Click on submit to capture data. This will submit the data to the inventory list and clear all fields.

Buttons:
Clear: Will clear all fields
Submit: Will capture all data to the inventory list

Back: closes current window
Exit: will exit/close the program

###### Stock Value
This window displays the stock value for all the items in the inventory.
User is not able to alter/change any data from this window.

Buttons:
Back: closes current window
Exit: will exit/close the program

###### On Sale
This window displays the item with the highest stock quantity, recommended to be placed on sale.
User is not able to alter/change any data from this window.

Buttons:
Back: closes current window
Exit: will exit/close the program

###### Restock Item
This window displays the item with the lowest stock quantity and allows the user to change/ increase the qty number (only). 
User must change (increase) the number in the Qty-field; click "Restock"
This will update the item's quantity in the inventory list.
To display the next item (with the lowest stock count/qty); click "Refresh"

Buttons:
Restock: will update the current item's Qty-field in the inventory list.
Refresh: will return the item with the lowest stock/qty count.

Back: closes current window
Exit: will exit/close the program
