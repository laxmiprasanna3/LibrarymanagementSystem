# LibrarymanagementSystem

# Book Record Management System
>>server
  >Storing Book Data
  >User Registration
  >Subscription

# Routes and Endpoints

## /users
  >GET:get all list of users
  >POST:Create a new user

## /users/{id}
 >GET:get a specific userby their ID
 >PUT:Update the user by their ID
 DELETE:Delete a user by ID(check if he/she still have an issued  book)&&(is there any fine to be collected from him/her)

 Subscription:
  >3months(Basic Subscription)
  >6months(Standard Subscription)
  >12months(Premium Subscription)

# /users/subscription-details/{id}
GET:get user subscription details
  >>date of subscription
  >>valid till
  >>fine if any

# /Books
 GET:get all book
 POST:create/add a new book

 # /books/{id}
 GET:get a book by ID
 PUT:update a book by ID

 # /books/issued
 GET:get all issued books

 # /books/issued/withFine
 GET:get all issued books with fine

 # Fine Calculation
 >> if the user has a issued book and the issued book is to be returned at 01/08/2024
 if he missed the date of reneval/return, then he needs to pay a penalty of Rs.100/-

>> if the user has a issued book and the issued book is to be returned at 01/08/2024
 if he missed the date of reneval/return, and his subscription also expires, then he needs to pay a penalty of Rs.100/-


 >>npm init
>>npm i express
>>npm i nodemon --save-dev (developers dependence)

>> in package.json -script{
    "start":"node index.js",
    "dev":"nodemon index.js"
}


for Running
>npm run dev

>Install thunder client and json

> url:: http://localhost:8081/