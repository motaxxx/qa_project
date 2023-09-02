# QA Analyst Project

## Exercice

## Functionality description
- Create a new user by filling in the following fields: Email, First Name, Last Name and clicking the Save button;
- All fields accept alphanumeric characters, length - 6 to 30 characters;
- After user is created, he receives an email with a temporary password that needs to be changed shortly;
- The user will use this credentials to login into the website and have email address, first name and last name displayed on the home page;
- User data is saved into the database, in the following places:
- tblUser.Email - varchar(30);
- tblUser.FirstName - varchar(10);
- tbUser.LastName - varchar(12);
- User creation should not take longer than 3 seconds

## Challenge

### 1. What questions would you ask in order to clarify requirements?

- What if the user has a first name and last name with fewer than 6 characters? (Example: Ana, Mota)
- If the email is not mandatory, and I fill in the first and last name and click "save," where is the email sent for the password change, and how do I log in?
- What happens if I click "cancel"?
- How much time do I have to change the password?
- What happens when the password expires?
- If I have a slow internet connection and can't create the user within 3 seconds?
- Will the password be stored in the database?
- How will the user know if there was an error during user creation?

-----------------

###  2. Specify 5 test cases to test this requirement
### Test Case: User Creation

### Prerequisites:
- None

### Test Data:
- Email: teixeira@gmail.com
- First Name: Christophe
- Last Name: Teixeira

### Test Steps:
1. Open Google Chrome
2. Go to https://broadvoice.coderbyte.com/question/qa-analyst-project-zuvjlgxd1c
3. Click on the "Add New User" button
4. Enter the email
5. Enter the first name
6. Enter the last name
7. Click the "Save" button

### Expected Results:
A new user is successfully created, and a temporary password email is sent to the provided email address in less than 3 seconds.

--------------------

### Test Case: Last Name with 4 Characters

### Prerequisites:
- None

### Test Data:
- Email: mota@gmail.com
- First Name: Christophe
- Last Name: Mota

### Test Steps:
1. Open Google Chrome.
2. Go to https://broadvoice.coderbyte.com/question/qa-analyst-project-zuvjlgxd1c.
3. Click on the "Add New User" button.
4. Enter the email.
5. Enter the first name.
6. Enter the last name.
7. Click the "Save" button.

### Expected Results:
It's not possible to create a new user.

------------------

### Test Case: Empty Field on the First Name

### Prerequisites:
- None

### Test Data:
- Email: mota@gmail.com
- First Name: (leave empty)
- Last Name: Teixeira

### Test Steps:
1. Open Google Chrome.
2. Go to https://broadvoice.coderbyte.com/question/qa-analyst-project-zuvjlgxd1c.
3. Click on the "Add New User" button.
4. Enter the email.
5. Enter the last name.
6. Click the "Save" button.

### Expected Results:
It was not possible to create the user, and I didn´t receive an email with the password.

------------

### Test Case: Logging in with the Temporary Password

### Prerequisites:
- Having a temporary password for the website

### Test Data:
- None

### Test Steps:
1. Open Google Chrome.
2. Go to https://broadvoice.coderbyte.com/question/qa-analyst-project-zuvjlgxd1c.
3. Login with the email and temporary password.

### Expected Results:
Successful login. The home page displays the email address, first name, and last name.

------------

### Test Case: Saving User Email in the Database

### Prerequisites:
- Having a created user

### Test Data:
- Email: teixeira@gmail.com
- First Name: Christophe
- Last Name: Teixeira

### Test Steps:
1. Access the database.
2. Select the tblUser.Email field.


### Expected Results:
The email teixeira@gmail.com is present in the tblUser.Email field.




