# User Resources

This documents all functionality related to users.

### User Object

###### User Structure

| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| id                            | snowflake                                                                           | user identifier                                                                                                                  |
| username                      | string                                                                              | user's username                                                                                                                    |
| avatar                        | ?string                                                                             | avatar hash and extension                                                                                                        |
| admin                         | boolean                                                                             | whether this user is an administrator                                                                                            |

## Get User - GET /users/{id}

Returns a user object for the identifier.

## Get Current User - GET /users/@me

Returns a user object of the requester.