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

## Get Posts - GET /posts

Returns an array of post objects that administrators have created.