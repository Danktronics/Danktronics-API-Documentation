# OAuth2

OAuth2 allows your applications to interact with the Danktronics Accounts API as an authorized user.

## Reference

If you are implementing OAuth2 without a library, read [RFC6749](https://tools.ietf.org/html/rfc6749) for how to format requests.

## URLs

###### OAuth2 URLs

| URL                                            | Description               |
| ---------------------------------------------- | --------------------------|
| https://danktronics.org/oauth2/authorize       | Authorization request URL |
| https://danktronics.org/api/oauth2/token       | Access Token URL          |

## Scope

The following are valid scopes to access certain information or perform actions.

###### OAuth2 Scopes

| Name                       | Description                                                                                                                                           |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| identify                   | grants [/users/@me](docs/accounts/resources/User.md)                                                                                                  |
| connections                | grants [/users/@me/connections](docs/accounts/resources/User.md)                                                                                      |