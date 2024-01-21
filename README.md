## Online Exam Authentication Service #
Project Code: E0001

Authentication Service is part of Online Exam Cloud Infrastructure.

## User Stories ##
### E0001-001: Register ###

* Actor: User without User ID
* Pre Condition:

1. User should have a working email-id which is not already registered with Online Exam Cloud.

* Input:

1. First Name of the User.
2. Last Name of the User
3. Working email id.
4. Phone No.
5. Preferred password with 8 characters (alphanumeric with at least one upper case and one lower case letter).

* Sequence:

1. User opens the webpage.
2. Registration page appears.
3. User supplies the First name,Last name, a working email-id, Phone No and the preferred password.
4. Page displays success message and redirects to login page.

* Post Condition:

1. Page displays success message and the login page appears

* Exceptions:

1. Registration page re-appears with appropriate message if user enters invalid Firstname or Lastname or phone no or invalid email-ID or invalid password.
2. Registration page re-appears with appropriate message if the email-ID is already registered with Online Exam Cloud.
3. Registration page will not show any special message if the email-ID is not reachable.


### E0001-002: Login with Active User ID ###

* Actor: User with Active User ID 

* Pre Condition:

1. User should have activated the User ID

* Input:

1. User ID. 
2. Password.

* Sequence:
 
1. User opens login web page
2. User supplies his/her User ID and Password
3. User click on login button
4. User home page appears

* Post Condition:

1. User home page appears with name of the user displayed.

* Exceptions:

1. Login page re-appears with appropriate message if user enters invalid User ID or password.


### E0001-003 Logout ###

* Actor: User with Active User ID

* Pre Condition:

1. User should have logged in to Online Exam Cloud.

* Input:

1. None

* Sequence:

1. User click on Logout.
2. Page displays a message ‘successfully Logout ‘ and the login page appears.

* Post Condition:

1. Login screen appears
2. Back button or bookmarks fail to open any of the login-protected pages of the web app

* Exceptions:

1. Not Applicable


## Development ##

### Dependencies ###
1. Nodejs 10+
2. Visual Studio Code

### How to run ###
1. Move to the 'app' folder
```
cd app
```
2. Install the dependencies
```
npm install
``` 
3. Run the app
```
npm start
```
4. Verify http://localhost:5001
