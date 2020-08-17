# Exercise Tracking API

#### A microservice to create users, allowing them to add exercises to their personal log and include information like descriptions, durations and date the entry.

### User Stories


1. I can create a user by posting form data (username) to /api/exercise/new-user. A username and userID will be returned.
2. I can get an array of all users using the api/exercise/users/[username] endpoint and providing a username.
3. I can add an exercise to any user with a POST request to /api/exercise/add (using form data and providing a userID, description, duration, and date[not required]). to If no date is supplied, the current date will be used. The server will return the user object with the added exercises.
4. I can retrieve a full exercise log of any user by sending a GET request to /api/exercise/log/[userID] and providing a userID. The user object will be returned with the log as an array and an exercise count.
5. I can retrieve part of the log of any user by also passing along optional parameters of a date range or an entry number limit.