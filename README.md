# SimpleGoRestAPI
Simple RESTful API to create, read, update and delete books.

# Installation
Mux Router: go get -u github.com/gorilla/mux

# Running the server:
go build
./go_restapi

# Endpoints

## Get All Books
GET api/books

## Get Single Book

GET api/books/{id}

## Delete Book

DELETE /api/delbooks/{id}

Create Book

POST api/books

Request sample
{
  "isbn":"4545454",
  "title":"Harry Potter",
  "author":{"firstname":"JK",  "lastname":"Rowling"}
}

## Update Book

PUT api/updatebooks/{id}

 Request sample
 {
   "isbn":"4545454",
   "title":"Updated Title",
   "author":{"firstname":"Harry",  "lastname":"White"}
 }
