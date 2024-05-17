EMPTRACK:- Built a secure employee profile management system with Python, Flask and MySQL featuring CRUD operations and robustauthentication.
Utilized Flask’s flexibility and MySQL’s efficiency to create a scalable, responsive and secure employee data solution. 

Installaion:- 1) pip intsall flask
              2) pip install flask-mysqldb

Important terms to know:-

App routing is the technique used to map the specific URL with
the associated function intended to perform some task

GET:- 1)It is a method of data retrieval from the server.
      2)It is used for retrieving data like searching, filtering, or paging.

POST:- 1)It is a method which is used to request to a server.
       2)It is used for submitting forms, modifying data, or creating new resources.

Explanation:
1)Flask App Initialization:

-> Initialize Flask application and MySQL configuration.
-> Set a secret key for session management.

2)Login Route:

-> Handles both GET and POST requests.
-> Validates user credentials and manages session variables.

3)Logout Route:

-> Clears the session and redirects to the login page.

4)Registration Route:

-> Validates user input.
-> Checks if the account already exists.
-> Registers a new user if all validations pass.

5)Index Route:

-> Displays the index page if the user is logged in.
-> Redirects to login if not authenticated.

6)Display Route:

-> Retrieves and displays the user's account details if logged in.
-> Redirects to login if not authenticated.

7)Update Route:

-> Allows the user to update their account details.
-> Performs input validation and updates the database.

8)Main Function:

-> Runs the Flask application on localhost at port 5000.


Explanation of basics of Flask terms:-

1. render_template

-> Purpose: Renders an HTML template and returns it to the client.
-> Example: return render_template('index.html', msg=msg)
-> Usage: Displays the index.html page and passes the msg variable to it.

2. request
   
-> Purpose: Accesses data sent by the client (like form submissions).
-> Example: request.method, request.form
-> Usage: Checks if the request method is POST and retrieves form data.

4. redirect

-> Purpose: Redirects the client to a different URL.
-> Example: return redirect(url_for('login'))
-> Usage: Sends the user to the login page.

5. url_for

-> Purpose: Generates a URL for the given endpoint (function).
-> Example: url_for('login')
-> Usage: Creates a URL for the login route.

6. session
-> Purpose: Stores data for a user session across requests.
-> Example: session['loggedin'] = True
-> Usage: Keeps track of whether the user is logged in.
