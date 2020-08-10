# User Resources

This documents all functionality related to users.

### User Object

###### User Structure

| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| id                            | snowflake                                                                           | user identifier                                                                                                                  |
| username                      | string                                                                              | user's username                                                                                                                  |
| avatar                        | ?string                                                                             | avatar hash and extension                                                                                                        |
| email?                        | string                                                                              | user's email                                                                                                                     |
| verified?                     | boolean                                                                             | if user's email is verified                                                                                                      |
| bot                           | boolean                                                                             | if user is a bot                                                                                                                 |
| flags                         | integer                                                                             | user details                                                                                                                     |

### Third Party Connection Object

###### Third Party Connection Structure

| Field         | Type    | Description                                                                         |
| ------------- | ------- | ----------------------------------------------------------------------------------- |
| type          | string  | connection service                                                                  |
| id            | string  | id of the account                                                                   |
| name          | string  | the username of the account                                                         |
| connected_on? | ISO 8601| time of connection                                                                  |

## Get Current User - GET /users/@me

Returns the user object of the requester.

## Get Current User Connections - GET /users/@me/connections

Returns an array of connection objects connected by the requester.