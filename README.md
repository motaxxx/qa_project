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




###  2. Specify 5 test cases to test this requirement
