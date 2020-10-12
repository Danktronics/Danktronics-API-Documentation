# Image Resources

This documents all functionality related to images.

### Uploaded Image Object

###### Uploaded Image Structure

| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| id                            | snowflake                                                                           | image identifier                                                                                                                 |
| hash                          | string                                                                              | image hash (specifically for viewing)                                                                                            |
| extension                     | string                                                                              | image extension                                                                                                                  |
| url                           | string                                                                              | ease of use url for accessing the image                                                                                          |
| owner_id                      | snowflake                                                                           | id of the uploader/owner                                                                                                         |

## Get Images - GET /images

Returns an array of uploaded image objects that the current user uploaded.

Query String Parameters
| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| before                        | snowflake                                                                           | get images before this ID                                                                                                        |
| after                         | snowflake                                                                           | get images after this ID                                                                                                         |
| limit                         | integer                                                                             | amount of images to return (default of 10)                                                                                       |

Response
| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| total_count                   | integer                                                                             | amount of owned images                                                                                                           |
| images                        | array of Image objects                                                              | array of owned images                                                                                                            |

## Upload Image - POST /images

Upload an image.

This endpoint only supports requests with a `Content-Type` of `multipart/form-data`. You must send a PNG/JPG/GIF with the correct type
and the file form name must be `file`.