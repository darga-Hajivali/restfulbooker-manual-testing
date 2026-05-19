# Get Booking API Analysis

## Endpoint
GET /booking/{id}

## Purpose
Retrieves booking details using booking ID.

## Tools Used
- Postman
- Swagger/OpenAPI
- GitHub

---

# Positive Scenario - Valid Booking ID

## Request
Valid booking ID passed in path parameter.

## Expected Behavior
API should return correct booking details.

## Actual Behavior
Booking details returned successfully.

## Validations
- Status code validation
- Firstname validation
- Lastname validation
- Response structure validation

---

# Negative Scenario - Invalid Booking ID

## Request
Invalid string booking ID passed in path parameter.

## Expected Behavior
API should reject invalid booking ID.

## Actual Behavior
API returned 404 Not Found.

## Observation
API properly rejected invalid booking ID input.

---

# Negative Scenario - Non Existing Booking ID

## Request
Non-existing booking ID passed in path parameter.

## Expected Behavior
API should return 404 Not Found.

## Actual Behavior
API returned 404 Not Found.

## Observation
API properly handled non-existing booking resource request.

# Positive Scenario - Updated Booking Validation

## Request
GET API executed using updated booking ID.

## Expected Behavior
API should return updated booking details.

## Actual Behavior
Updated booking details returned successfully with status code 200 OK.

## Observation
GET API successfully retrieved updated booking information after PUT update operation.