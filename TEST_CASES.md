# Urban Scooter — Manual QA Test Cases

## Project Overview
Manual QA testing of the Urban Scooter web application, Android application, and REST API during TripleTen QA training.

The following are representative test case examples. Actual execution results should be recorded separately.

## TC-001: Validate Required Fields on the Order Form
**Platform:** Web
**Test Type:** Negative / Functional

**Preconditions:** Urban Scooter order form is open.

**Steps:**
1. Open the order form.
2. Leave a required field empty.
3. Attempt to proceed to the next step.

**Expected Result:** The form prevents progression and displays appropriate validation feedback.

**Actual Result:** Not recorded in this portfolio example.

## TC-002: Validate Input Boundary Values
**Platform:** Web
**Test Type:** Boundary Value Analysis

**Preconditions:** An input field with defined length limits is available.

**Steps:**
1. Enter a value below the allowed minimum.
2. Enter a value at the minimum.
3. Enter a value at the maximum.
4. Enter a value above the maximum.

**Expected Result:** Valid boundary values are accepted; out-of-range values are rejected according to requirements.

**Actual Result:** Not recorded in this portfolio example.

## TC-003: Verify Order Status Notification
**Platform:** Android
**Test Type:** Functional

**Preconditions:** An order exists and the app is running.

**Steps:**
1. Open the Urban Scooter Android application.
2. Navigate to the relevant order.
3. Trigger or wait for the specified notification event.
4. Check the displayed notification.

**Expected Result:** Notification content and timing match the application requirements.

**Actual Result:** Not recorded in this portfolio example.

## TC-004: Create Courier via REST API
**Platform:** REST API
**Test Type:** API / Functional

**Endpoint:** POST /api/v1/courier

**Steps:**
1. Open Postman.
2. Configure a POST request for the courier endpoint.
3. Supply a valid JSON request body based on the API specification.
4. Send the request.
5. Inspect the response.

**Expected Result:** The API returns the documented success status and response body for a valid courier creation request.

**Actual Result:** Not recorded in this portfolio example.

## TC-005: Delete Courier via REST API
**Platform:** REST API
**Test Type:** API / Functional

**Endpoint:** DELETE /api/v1/courier/:id

**Steps:**
1. Create or identify a test courier.
2. Send a DELETE request using the courier's ID.
3. Inspect the response.

**Expected Result:** The API returns the documented response for a successful deletion.

**Actual Result:** Not recorded in this portfolio example.
