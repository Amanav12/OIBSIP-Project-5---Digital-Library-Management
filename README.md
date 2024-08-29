# OIBSIP-Project-5---Digital-Library-Management
Task 5
This project is a Digital Library Management System implemented in Java. The system provides a platform for managing a collection of books, handling user authentication, and performing various library-related tasks such as viewing, issuing, and returning books. Here’s an overview of the project:

1. Core Functionality:
Book Database:

The system has a predefined collection of books categorized by different fields like Electrical Engineering (EE), Electronics and Communication Engineering (ECE), Computer Science Engineering (CSE), Information Technology (IT), Business Administration (BBA), Mathematics (MATHS), Physics (PHYS), Chemistry (CHEM), and language subjects.
The books are stored in a HashMap where the key is the book number (an integer) and the value is the book details (a string).
User Authentication:

The system allows for both admin and user login.
Admins and users are authenticated using a HashMap where the key is the user ID (a string) and the value is the password (an integer).
Different functionality is available depending on whether the user is logged in as an admin or a regular user.
2. Admin Features:
Adding New Books:
Admins can add new books to the collection. They need to provide a unique book number and details of the book.
Updating Existing Books:
Admins can update details of existing books by specifying the book number and the updated details.
Deleting Books:
Admins can delete books from the collection after confirming the action.
3. User Features:
Viewing Books:
Users can view details of a specific book by providing its book number or view all available books.
Issuing Books:
Users can issue a book if they don’t have any other book already issued. The system allows only one book to be issued at a time.
Returning Books:
Users can return a book that they have previously issued.
4. Navigation and Flow:
The application starts with a homepage offering options to login as an admin or a user, or to exit the system.
Once logged in, the user (admin or regular) is directed to their respective mainpage where they can select different actions.
After performing an action, the user is typically returned to their main page to continue with other tasks.
5. User Experience:
The interface is text-based and interactive, prompting the user for input at various stages.
The system checks for invalid input, such as trying to add a book with an existing book number or attempting to issue a book when one is already issued.
6. Structure of the Code:
The system is structured into methods corresponding to different tasks like admin_login(), user_login(), add_new(), upd_old(), views(), etc.
The HashMap data structures are central to the operation, managing user credentials and book details.
The main method initializes the system by calling the homepage() method.
