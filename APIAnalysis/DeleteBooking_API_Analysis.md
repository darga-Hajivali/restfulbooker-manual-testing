# Delete Booking API Analysis

## Endpoint
DELETE /booking/{id}

## Purpose
Deletes existing booking resource.

## Headers
- Cookie: token

## Tools Used
- Postman
- Swagger/OpenAPI
- GitHub

---

# Positive Scenario - Delete Existing Booking

## Request
Valid booking ID passed with authentication token.

## Expected Behavior
Booking should be deleted successfully.

## Actual Behavior
Booking deleted successfully.

## Validations
- Delete response validation
- Resource deletion verification using GET API
- 404 validation after deletion

## Observation
DELETE API successfully removed booking resource from the system.