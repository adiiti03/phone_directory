The program is a simple implementation of a contact book using a doubly linked list. Here is the design flow of the program:

1.	Node Structure:
-	A  `Node`  structure  is  defined  to  store  contact  information,  including  `name`,
`phone_number`, and pointers to the next and previous nodes in the doubly linked list.

2.	ContactBook Class:
-	A `ContactBook` class is defined to manage the contact book.
-	Private member variables include a pointer to the head of the linked list (`head`), a string (`x`) for temporary storage of names, and a long long integer (`y`) for temporary storage of phone numbers.
-	The constructor initializes the head to `NULL`, and `x` and `y` to default values.
-	Several member functions are defined within the class.

3.	CreateNode Function:
-	Adds a new contact to the contact book.
-	Takes user input for the name and phone number.
-	Creates a new node, assigns values, and adds it to the end of the linked list.

4.	Display Function:
-	Displays all contacts in the contact book.
-	Uses the BubbleSort function to sort contacts alphabetically by name before displaying.
-	Counts the total number of contacts.

5.	Search Function:
-	Allows the user to search for a contact by either name or phone number.
-	Takes user input for the search type (name or number) and the search query.
-	Displays the contact information if found; otherwise, notifies the user that the contact was not found.

6.	DeleteAllContacts Function:
-	Deletes all contacts in the contact book.
-	Frees memory occupied by each node in the linked list.
7.	DeleteContactBySearch Function:
-	Allows the user to search for and delete a specific contact.
-	Takes user input for the search type (name or number) and the search query.
-	Displays the contact information if found and asks for confirmation before deletion.
8.	BubbleSort Function:
-	Sort the contact book alphabetically by name using the Bubble Sort algorithm.

9.	EditContacts Function:
-	Allows the user to search for and edit a specific contact.
-	Takes user input for the search type (name or number) and the search query.
-	Displays the contact information if found and allows the user to input new values.
 
10.	OfflineSave Function:
-	Writes the contact book data to a text file named "contactbook.txt."
11.	ReopenCB Function:
-	Reads the contact book data from the "contactbook.txt" file and reconstructs the linked list.

12.	Structure Function:
-	Displays a menu of options for the user.
-	Takes user input for the desired operation and calls the corresponding function.
-	Handles exceptions for invalid commands.

13.	Main Function:
-	Creates an instance of the `ContactBook` class.
-	Invokes the `reopenCB` function to load existing contacts from the file.
-	Takes user input for their name.
-	Displays a welcome message and enters the main structure loop.

The program uses a menu-driven approach to interact with the user, allowing them to add, edit, delete, search, display, and manage contacts in the contact book. The contact book data is saved to and loaded from a text file for persistence between program executions.
