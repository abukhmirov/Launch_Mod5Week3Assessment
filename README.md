# JeffersonCountyLibrary

## Setup
* Fork and Clone this repository
* Run `update-database`

## Exercise (12 points)

Check out a new branch and complete the following tasks **in order**:
* 2 points - There is a bug in our authentication!  Identity looks like it is set up, but we can't register users.  Find and fix this bug! (Hint: this should only take one line of code)
* 2 points - Right now, anyone can 'check out' a book.  Update the application so that only a logged in user can check out a book.
* 4 points - In this application, we have the ability to create new books.  Improve this functionality by:
  * Add a link from the nav-bar to add a book
  * Make sure only Librarians can add a book
* 2 points - Create a descriptive pull request and merge this branch into main
* 2 points - Take a screenshot of a database query result from pgAdmin that clearly shows which users in your database are librarians.  Update this README to include your screenshot below:

   ![image](https://github.com/abukhmirov/Launch_Mod5Week3Assessment/assets/130601068/73d35b3d-e6ac-444e-908d-32f8e7d5c086)


  

## Questions (6 points)

Answer the questions below in this README.  Answer these questions as if you are in an interview!

1. What are roles and claims as they relate to Authentication and Authorization?
Roles and Claims are used for permissing different functionalities of the app. Roles allowing to have a grouping of permissions to be assigned to a user. The user might need to Authenticate themselves to gain access to a role. Claims are more granular permission that can be given to a user. An example of the difference between a role and a claim is if you have a user with the Librarian role and they can Read() and Write() with the role's permission. You could also leave them as a regular, non-librarian user, but add claims to them which separately allow  the user to read and write.
2. How do cookies play a role in authentication and authorization?
Cookies allow for regular updates on the user like how many times the user does an action or logs in. This would be too regular of a change for Roles or Claims. The cookies can then be used to change permissions based on whatever they are updating.
3. If asked to implement Auth in a new .NET application, would you use the Identity framework?
Yes, it provides a premade set of tools that automatically get set in your app. This gives me more time to work on the project and the razor pages can be updated to fit my styling choices. It seems counter productive to not use Identity.

## Rubric

This assessment has a total of 18 points.  Earning 12 or higher is a pass!
