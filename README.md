# Premable
```
LIP: 0001
Title: Anchor/Client interoperability
Author: SDF
Status: Active
Created: 2019-08-28
Updated: 2019-08-28
Version 0.1.0
```
# Summary

This LIP defines the standard of Lightnet's interface.

# API Endpoints

- `GET /v1/remittances.kyc-info`: optional
- `POST /v1/remittances.validate`: required
- `POST /v1/remittances.commit`: required
- `POST /v1/remittances.callback`: required

# Authentication

  Clients must submit the AccessToken previously obtained via calling `Authentication Endpoint` as below to all API endpoints.
  

# Authentication Endpoint

- `POST /v1/auth`

# HTTPS Only

This protocol involves the transfer of value, and so HTTPS is required for all endpoints for security. Wallets and anchors should refuse to interact with any insecure HTTP endpoints.

# Remittances Validation

  Clients send a request which containing information collected from customer, and Lightnet will returns a response indicating the transaction can continue or an error indicating an issue with the request.
