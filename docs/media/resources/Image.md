# Image Resources

This documents all functionality related to images

### Uploaded Image Object

###### Uploaded Image Structure

| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| id                            | snowflake                                                                           | image identifier                                                                                                                 |
| hash                          | string                                                                              | image hash (specifically for viewing)                                                                                            |
| extension                     | string                                                                              | image extension                                                                                                                  |
| url                           | string                                                                              | ease of use url for accessing the image                                                                                          |
| owner                         | snowflake                                                                           | id of the uploader/owner                                                                                                         |
| created_at                    | ISO8601 timestamp                                                                   | when the image was uploaded                                                                                                      |

## Upload Image - POST /images

Upload an image.

This endpoint only supports requests with a `Content-Type` of `multipart/form-data`. You must send a PNG/JPG/GIF with the correct type
and the file form name must be `file`.

## Get Images - GET /images

Returns an array of uploaded image objects that the current user uploaded.