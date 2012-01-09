---
title: Company | SpinOff API
---

# Company API

## Get company

Gets the information of the user's company.
    
    GET /company

### Response

<%= headers 200 %>
<%= json :company %>


## Create company

Creates the company for the user.
    
    POST /company

### Input

name
: _Required_ **string** - The desired name for the company

### Response with valid parameters

<%= headers 201, false %>

### Response with invalid parameters

<%= headers 412, false %>