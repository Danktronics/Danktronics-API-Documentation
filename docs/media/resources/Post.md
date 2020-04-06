# Post Resources

This documents all functionality related to posts.

### Post Object

###### Post Structure

| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| id                            | snowflake                                                                           | post identifier                                                                                                                  |
| title                         | string                                                                              | title of the post                                                                                                                |
| message                       | string                                                                              | post content                                                                                                                     |
| creator                       | snowflake                                                                           | id of the poster                                                                                                                 |
| created_at                    | ISO8601 timestamp                                                                   | when the post was created                                                                                                        |

## Get Posts - GET /posts

Returns an array of post objects that administrators have created.