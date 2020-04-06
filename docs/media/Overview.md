# Danktronics Media

Welcome to API documentation for the Danktronics Media service.

To get started navigate to the resources folder.

# Reference

###### Base URL

```
https://media.danktronics.org/api
```

## Authentication

Authenticating with the Media API can be done using the `Authorization` header.

The `Authorization` header must always be present and contain an API token.

An API token can currently be retrieved by going to settings on the website and revealing the token.

## Processing Responses

Currently all responses follow the same data structure

> :warning: **This structure is going to be removed in a future version**

###### Response Structure

| Key                           | Type                                                                                | Description                                                                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| code                          | integer                                                                             | HTTP response code                                                                                                               |
| data                          | object                                                                              | relevant data                                                                                                                    |