# NoSQL-Social-Network-API-18
An API for a social network web application where users can share their thoughts, react to friends’ thoughts, and create a friend list. This application uses Express, Node, MongoDB and Mongoose to allow users, thoughts, friend lists and thought reactions to be created, updated and deleted. 

## User Story
As a social media startup, I want an API for my social network that uses a NoSQL database so that my website can handle large amounts of unstructured data

## Criteria
GIVEN a social network API
WHEN I enter the command to invoke the application
THEN my server is started and the Mongoose models are synced to the MongoDB database
WHEN I open API GET routes in Insomnia for users and thoughts
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete users and thoughts in my database
WHEN I test API POST and DELETE routes in Insomnia
THEN I am able to successfully create and delete reactions to thoughts and add and remove friends to a user’s friend list


## Installation 
* Clone GitHub repository
* npm init
* Ensure that MongoDB and Express are installed on your computer. 
* Invoke application using npm start. 

## Endpoints andEndpoints
User:
Get all users: GET /api/users
Create a user: POST /api/users
Get user by ID: GET /api/users/:id
Update a user: PUT /api/users/:id
Delete a user: DELETE /api/users/:id
Add a friend: PUT /api/users/:userId/friends/:friendId
Delete a friend: DELETE /api/users/:userId/friends/:friendId

Thought:
Get all thoughts: GET /api/thoughts
Create a thought: POST /api/thoughts
Get thought by ID: GET /api/thoughts/:id
Update a thought: PUT /api/thoughts/:id
Delete a thought: DELETE /api/thoughts/:id

Reaction:
Add a reaction: PUT /api/thoughts/:id/reactions
Delete a reaction: DELETE /api/thoughts/:id/reactions

## Technologies Used
* JavaScript
* Node.js
* MongoDB
* Mongoose
* Express.js
