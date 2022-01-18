# Introduction
The project uses [typicode/json-server](https://github.com/typicode/json-server) library to create fake REST API. If you want to know more details, read this [article](https://dev.to/myogeshchavan97/how-to-easily-create-and-host-your-own-rest-api-without-writing-a-single-line-of-code-2np4), but it is not necessary. All endpoints that should be used in this application are documented below.

# Documentation
To run the project on the localhost, execute the following command: 
```
npm start
```
Now, the backend application is available under the following link: http://localhost:3000 and it is ready for integration with the UI.

## Endpoints

### Get calendar configuration
```
GET http://localhost:3000/config
```

### Get user's appointments
```
GET http://localhost:3000/users/:id/appointments
```

### Create appointment
```
POST http://localhost:3000/appointments
```
Example body (all properties are required):
```
  {
    "userId": "779cc6e8-b1d7-490a-bb9a-64d5fa1dd87f",
    "start": "2022-01-14T08:00:00.000Z",
    "end": "2022-01-14T09:00:00.000Z"
  }
```