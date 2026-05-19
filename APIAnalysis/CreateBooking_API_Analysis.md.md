# Create Booking API Analysis

## Endpoint
POST /booking

## Purpose
Creates a new booking.

## Headers
Content-Type: application/json

## Tools Used
- Postman
- Swagger/OpenAPI
- GitHub

---

# Positive Scenario - Valid Booking

## Request
Valid booking payload provided.

## Expected Behavior
Booking should be created successfully.

## Actual Behavior
Booking created successfully with generated booking ID.

## Validations
- Status code validation
- Booking ID validation
- Response body validation
- Data validation

---

# Negative Scenario - Missing Firstname

## Request
Firstname field removed from payload.

## Expected Behavior
API should return 400 Bad Request with validation message.

## Actual Behavior
API returned 500 Internal Server Error.

## Observation
Backend validation is not handled properly for missing mandatory fields.

---

# Negative Scenario - Invalid Price

## Request
Invalid price value provided using negative number.

## Expected Behavior
API should reject invalid price with proper validation message.

## Actual Behavior
API became unresponsive / no response observed.

## Observation
Backend validation handling appears unstable for invalid payload values.

---

# Negative Scenario - Empty Body

## Request
Empty JSON payload sent.

## Expected Behavior
API should return 400 Bad Request.

## Actual Behavior
API became unresponsive.

## Observation
API did not properly handle empty payload validation.

---

# Negative Scenario - Invalid Dates

## Request
Invalid date values provided.

## Expected Behavior
API should reject invalid date format.

## Actual Behavior
API became unresponsive.

## Observation
Backend validation handling appears weak for malformed date inputs.