# rebel_test
Created an API to fetch data from blockchain

# Endpoint: /get-token-balance

# Purpose:

This endpoint retrieves the current balance of a specific token for a given user.

# Method:

GET

# Response:

Status Code:

200 OK: If the balance is retrieved successfully.
400 Bad Request: If the request is missing or has invalid parameters.
500 Internal Server Error: If an error occurs during the balance retrieval process.
Body:

If successful:
JSON

```
{
    "code": 200,
    "address": "0x8012747221C6726B0A5f2E099d34cc7705A3D09b",
    "contract": "0x7e56c01536d0576b3EeB84128cac1C222759F408",
    "name": "CEX",
    "balance": "0",
    "msg": "Token Details"
}
```
where balance is the current token balance of the user.
Example Usage:

# Bash

curl -X GET "http://localhost:3000/get-token-balance/"
This will send a GET request to the /get-token-balance endpoint with the specified address.

