Title
Udacity Bookshelf App!


Description:
---------
explains why your project is interesting
describes your motivation to creating the project and why the user should want to engage with it
provides clear instructions for developers who want to use or contribute to your prject
------

This app is meant to be a virtual Bookshelf app where you can manage your books. This will be the foundation app that will be used by udacity students to learn and demonstrate their abilities towards building APIs. There is a set of TODOs items across the app that the students should work on. 

Getting Started
---
Remember, this should include any prerequisite skills or project dependencies as well as how to run and test the project.
----






API Reference

# API Documentation Practice
In this exercise, your task is to practice writing documentation for the bookstore app we created earlier.

You'll soon be writing documentation for your final project (the Trivia API), after which you'll get feedback from a reviewer. You can think of this as some rudimentary practice to prepare for that.

At each step, you can compare what you've written with our own version. Of course, **there isn't a single correct way to write a piece of documentation**, so your version may look quite different. However, there are principles and practices you should follow in order to produce quality documentation, and we'll point this out so you can check whether you've incorporated them in what you wrote.

## Getting started
Now, add a Getting Started section to your documentation. Remember, this should include at least your base URL and an explanation of authentication. Feel free to provide other information that is relevant for your API

###Introduction

Base URL: at this version, this app is ran locally and is not hosted publicly. The backend is hosted at: http://127.0.0.1:500/

Authentication: at this version, this app does not require authentication.


## Error Handling
Now, add an Error Handling section to your documentation. It should include the format of the error responses the client can expect as well as which status codes you use.
- Response codes
- Messages
- Error types

###Error Handling
Error responses format:
    {
    "success": False, 
    "error": 400,
    "message": "bad request"
    }

Status codes used:
400: bad request
404: resource not found
422: unprocessable


## Endpoint Library
Now, add an Endpoint Library section to your documentation. Make sure that endpoints, methods and returned data are all clear. Consider including sample requests for clarity

- Organized by resource
- Include each endpoint
- Sample request 
- Arguments including data types
- Response object including status codes and data types 

GET /books
- general:
    - is organized as a list of books, returning a list of books objects, total books amount and success value.
    - books are paginated retrieving 8 books per page. Also includes a request argument (page) for a given page, starting in page 1.


    - sample:
        curl http://127.0.0.1:5000/books

    - output:
        {
  "books": [
    {
      "author": "Stephen King", 
      "id": 1, 
      "rating": 5, 
      "title": "The Outsider: A Novel"
    }, 
    {
      "author": "Lisa Halliday", 
      "id": 2, 
      "rating": 4, 
      "title": "Asymmetry: A Novel"
    }, 
    {
      "author": "Kristin Hannah", 
      "id": 3, 
      "rating": 4, 
      "title": "The Great Alone"
    }, 
    {
      "author": "Tara Westover", 
      "id": 4, 
      "rating": 5, 
      "title": "Educated: A Memoir"
    }, 
    {
      "author": "Jojo Moyes", 
      "id": 5, 
      "rating": 5, 
      "title": "Still Me: A Novel"
    }, 
    {
      "author": "Leila Slimani", 
      "id": 6, 
      "rating": 2, 
      "title": "Lullaby"
    }, 
    {
      "author": "Amitava Kumar", 
      "id": 7, 
      "rating": 5, 
      "title": "Immigrant, Montana"
    }, 
    {
      "author": "Madeline Miller", 
      "id": 8, 
      "rating": 5, 
      "title": "CIRCE"
    }
  ], 
  "success": true, 
  "total_books": 16
}


POST /books
.
.
.

















Authors
---
Give credit where credit is due! If you used any open source technologies, cite those here as well.
---







Acknowledgements

---
If anyone helped you on this learning journey or in developing this project specifically, give them a shout here... and let them know in real life.
---