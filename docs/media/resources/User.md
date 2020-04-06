# User Resources

This documents all functionality related to users.

### User Object

###### User Structure

| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| id                            | snowflake                                                                           | user identifier                                                                                                                  |
| username                      | string                                                                              | user's username                                                                                                                    |
| avatar                        | ?string                                                                             | avatar hash and extension                                                                                                        |
| created_at                    | ISO8601 timestamp                                                                   | when the user was created                                                                                                        |
| admin                         | boolean                                                                             | whether this user is an administrator                                                                                            |

## Get User - GET /users/{id}

Returns a user object for the identifier.

## Get Current User - GET /users/@me

Returns a user object of the requester.