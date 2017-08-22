# Shopping-List

Tracks the completion of an assignment to make a Shopping List. 

## To Do - Part 1
 - Setup unit testing libraries and ensure minimal tests written.
Note: From here onwards, you’re expected to practise Test-Driven Development.

- Develop features enabling user to Create, Read, Update and Delete non-persistent data
(no database required, data is lost when application stops) using OOP.

- Develop features enabling user to Login to application using OOP.

- Building on the UI templates developed in Challenge 1, create a user interface to access
functionality above implemented with HTML/CSS/Bootstrap or Materialize.

- Integrate TravisCI for Continuous Integration in your repository (with ​ReadMe​ badge).

- Integrate test coverage reporting (e.g. Coveralls) with badge in the ReadMe.

- Obtain CI badges (e.g. from Code Climate and Coveralls) and add to ReadMe.

- Create a pull request and request two of your friends to review it.

- Deploy your Flask application to Heroku.

## To Do - Part 2
Note: To be done after part 1
- Create a new Repo in which you will develop a Flask API.
Note: From here onwards, you’re expected to practise Test-Driven Development.
- Create models for the data which the API will be manipulating using SQLAlchemy.
- Implement data persistence using Postgresql
- Create a RESTful API using Flask with Endpoints that:
a. Enable users to create accounts and login into the application

EndPoint | Public Access
------------ | -------------
POST /auth/register | TRUE
POST /auth/login | TRUE
POST /auth/logout | TRUE
POST /auth/reset-password | TRUE

b. Enable users to create, update, view and delete a shopping list

EndPoint | Public Access
------------ | -------------
POST /shoppinglists/ | FALSE
GET /shoppinglists/ | FALSE
GET /shoppinglists/<id> | FALSE
PUT /shoppinglists/<id> | FALSE
DELETE /shoppinglists/<id> | FALSE

c. Add, update, view or delete items in a shopping list

EndPoint | Public Access
------------ | -------------
POST /shoppinglists/<id>/items/ | FALSE
PUT /shoppinglists/<id>/items/<item_id> | 
DELETE /shoppinglists/<id>/items/<item_id> | FALSE

- Implement Token Based Authentication for the API such that methods besides login and
register are not accessible to unauthenticated users.
- Create scripts for handling migration of data when the data model changes.
- Implement searching based on the name using a GET parameter q.
- Implement pagination on your API so users can specify the number of results they would
like to have via a GET parameter limit.
- Test API with Postman.
- Using a tool like Swagger or Apiary, document your API. The documentation should be
accessible via your application’s URL.
- Integrate TravisCI for Continuous Integration in your repository (with ReadMe badge).
- Integrate test coverage reporting (e.g. Coveralls) with badge in the ReadMe.
- Create a pull request and request two of your friends to review it.
- Merge with master
- Deploy to Heroku.
