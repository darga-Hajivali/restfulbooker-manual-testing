# Patch Booking API Analysis

## Endpoint
PATCH /booking/{id}

## Purpose
Partially updates booking details.

## Headers
- Content-Type: application/json
- Cookie: token

## Tools Used
- Postman
- Swagger/OpenAPI
- GitHub

---

# Positive Scenario - Partial Booking Update

## Request
Only firstname field updated using PATCH API.

## Expected Behavior
API should update only provided field without affecting other booking details.

## Actual Behavior
Firstname updated successfully with status code 200 OK.

## Validations
- Status code validation
- Firstname validation
- Existing data unchanged validation

## Observation
PATCH API successfully performed partial resource update.