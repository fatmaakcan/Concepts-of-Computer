# API LOGIC (REST & JSON BASICS)

## What is API?
### API (Application Programming Interface) is like a bridge that allows an application to use another application's features and data. Not everything can be written from scratch. For example, to show the weather in a website, a request is sent to the Meteorology API instead of accessing their private database system.

## REST & HTTP Methods (GET,POST,PUT,DELETE)
### REST is a type of architecture that provides a standart order for API's. In this architecture, processes are divided into request types:
### -GET: Used for retrieving data from the server. (e.g., reading a blog post)
### -POST: Used for sending/saving new data. (e.g., creating a new membership) 
### -PUT: Used for updating existing data. (e.g., changing progile information)
### -DELETE: Used for removing data. (e.g., deleting a message)

## JSON Structure (JavaScript Object Notation)
### The common language of APIs. In the past, XML was used; however, JSON is lighter and easier to read. It is similar to dictionaries in Python or objects in Java.

### A Simple JSON Example:
    {
        "id":101,
        "name":"Olivia",
        "department":"CS",
        "is_active": true
    }

## Endpoint
### An endpoint is the URL of an API and it acts as a gateaway to the outside world. Meaningful names should be used:
### api.site.com/users (brings the user list) -> Good design
### api.site.com/bringTheUsersToMe (out of the standard) -> Bad design
### Process:
### 1. Request: Client sends a GET  request to the /books address.
### 2. Process: Server checks the database.
### 3. Response: Server sends the book list in JSON format with a 200 OK status code. 

