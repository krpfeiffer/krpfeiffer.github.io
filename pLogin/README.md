![project logo](./assets/icon-128x128.png)

# pLogin
WordPress plugin to handle login functionality.

## Description
This plugin handles user login functionality.

The user interface is based on the Google Material Design (V2) paradigm.
It uses surfaces, elevations and a primary colour to highlight items.

It provides User/Member/Subscriber login capabilities.
- A visitor is someone using the site anonymously. No login handling is required, unless the visitor tries to access private content.
- A user has login credentials and is logged in.
  - Users with editor or author privileges are called "members".
  - Users with subscriber privileges are called "subscribers".
  - There is no special handling of the contributor class.

This plugin leverages standard WordPress functionality.

### Features
* Stores user last and previous logins.
* Redirects to member page for users on successful login. Administrators go to admin dashboard.
* Redirects to login page if a vistor attempts to access private content.
* Provides user password reset request self-service.

## Dependencies
* [pNet plugin](https://github.com/krpfeiffer/pnet)
