# Premable

LIP: 0001
Title: Anchor/Client interoperability
Author: SDF
Status: Active
Created: 2019-08-28
Updated: 2019-08-28
Version 0.1.0

# Simple Summary

This LIP defines the standard of Lightnet's interface.

# API Endpoints

- `GET /v1/remittances.kyc-info`
- `POST /v1/remittances.validate`
- `POST /v1/remittances.commit`
- `POST /v1/remittances.callback`

# Authentication

# HTTPS Only

This protocol involves the transfer of value, and so HTTPS is required for all endpoints for security. Wallets and anchors should refuse to interact with any insecure HTTP endpoints.
