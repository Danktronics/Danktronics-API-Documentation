# Danktronics Media

Welcome to API documentation for the Danktronics Media service.

To get started navigate to the resources folder.

# Reference

**Danktronics Administrators reserve the right to restrict or ban API access.**

###### Base URL

```
https://media.danktronics.org/api
```

## Authentication

Authenticating with the Media API can be done using the `Authorization` header.

The `Authorization` header must always be present and contain an API token.

An API token can currently be retrieved by going to settings on the website and revealing the token.

## Versioning
Media can expose multiple versions of the API (often for testing or deprecation purposes). In order to specify the version of the API you would like to use, you must prefix the route with `/api/v{version_number}/`. If you don't include a version in the URL then the API will automatically default to the latest current stable version. The following table documents the current state of API versions.

###### API Versions

| Version | Status       | Stable  |
| ------- | ------------ | ------- |
| 1       | Discontinued |         |
| 2       | Discontinued |         |
| 3       | Available    | ✔️      |

## Nullable and Optional Resource Keys

Below is a table detailing what keys the API may return.

###### Example Nullable and Optional Fields

| Key                          | Type    |
| ---------------------------- | ------- |
| optional_key?                | string  |
| nullable_key                 | ?string |
| optional_and_nullable_key?   | ?string |
