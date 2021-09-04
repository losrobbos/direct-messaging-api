# Chat App API

This project is a sample Socket.io backend server which allows to exchange direct chat messages

It uses:
- ExpressJS
- Socket.io
- MongoDB (for storing the users & messages)

## Prep

Requirement: You have MongoDB setup either on your local PC or in the cloud (e.g. on ATLAS)

Prepare a .env file and put your MongoDB database connection string inside.

You can use the .env.sample file as a template.

E.g. in case you have MongoDB running locally (on default port) you can put something like:

`MONGO_URI=mongodb://localhost/my_chat_db`

Now let's install all needed packages:

`npm install` (or just "npm i")

Now seed in some initial users & message exchanges using the provided seed script

`npm run seed`

## Launching

`npm start`

Once your API launches, you should be able to see your list of users on the route /users.

So if you have started it locally e.g. on localhost Port 5000 you should get it with:

`http://localhost:5000/users`

Now how to connect to this socket io server and exchange messages?

Here you have a sample project that does that:

[https://github.com/losrobbos/direct-messaging-frontend](https://github.com/losrobbos/direct-messaging-frontend)
