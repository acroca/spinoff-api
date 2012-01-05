---
title: Global responses | SpinOff API
---

# Global responses

## When the request sends an non-basic authentication

If the request contains any other kind of authentication but simple

### Response

<%= headers 400, false %>


## When the user is not valid

It happens when the user doesn't specify HTTP basic authentication with the e-mail and password. Also when the password is incorrect

### Response

<%= headers 401, false %>

## When the user has to create a company

It happens when the user still have to create the company.
Visit the [Company API](/company/) in order to know how to proceed.

### Response

<%= headers 406, false %>