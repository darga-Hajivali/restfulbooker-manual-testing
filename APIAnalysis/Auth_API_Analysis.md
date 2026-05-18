# Auth API Analysis

## Endpoint
POST /auth

## Purpose
Generate authentication token

## Request Headers
Content-Type: application/json

## Request Body

{
   "username": "admin",
   "password": "password123"
}

## Expected Status Code
200

## Expected Response

{
   "token": "generated_token"
}

## Positive Scenarios
- Verify token generated with valid credentials

## Negative Scenarios
- Verify API rejects invalid password
- Verify API rejects blank username