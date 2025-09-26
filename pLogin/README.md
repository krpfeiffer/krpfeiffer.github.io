![project logo](./assets/icon-128x128.png)

# pLogin
WordPress plugin to provide login functions for all the pfeifferNet websites.

## Description
Functionality used by all the pfeifferNet websites to handle user logins.
Uses standard WordPress login functionality.
User interface uses Google Material Design paradigm.

### Features
* User/Member/Subscriber login capabilities.
  - A visitor is someone using the site anonymously. No login handling is required.
  - A user has login credentials and is logged in.
    - Users with editor or author privileges are called "members".
    - Users with subscriber privileges are called "subscribers".
    - There is no special handling of the contributor class.
* Stores user last and previous logins.
* Redirects to member page for users on successful login. Administrator goes to admin dashboard.
* Redirection to login page if a vistor attempts to access private content.
* Provides user password reset request self-service.

## Dependencies
* [pNet plugin](https://github.com/krpfeiffer/pnet)
