---
title: Programs | SpinOff API
---

# Programs API

## Get available programs

Gets all the available programs to buy
    
    GET /programs

### Response

<%= headers 200 %>
<%= json :programs %>


## Get company programs

Gets all the programs of the user's company. They will appear here after buying
    
    GET /company/programs

### Response

<%= headers 200 %>
<%= json :programs %>


## Buy programs

The user buys the specified program if this is still available.

	PUT /programs/:id/buy

### Response when the purchase is successful

<%= headers 201, false %>


### Response when the purchase is not successful

<%= headers 410, false %>

