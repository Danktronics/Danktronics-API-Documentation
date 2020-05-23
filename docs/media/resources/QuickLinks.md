# QuickLink Resources

This documents all functionality related to quick links.

### QuickLink Object

###### QuickLink Structure

| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| id                            | snowflake                                                                           | quick link identifier                                                                                                            |
| owner_id                      | snowflake                                                                           | quick link owner's id                                                                                                            |
| hash                          | string                                                                              | hash of the quick link                                                                                                           |
| quick_url                     | string                                                                              | ease of use url for redirecting using media                                                                                      |
| redirect_url                  | string                                                                              | url quick link is pointing to                                                                                                    |

## Get QuickLink - GET /quicklinks

Returns an array of the current user's quick links

## Create QuickLink - POST /quicklinks

Provide an object with key url to redirect to. Returns the new quick link object