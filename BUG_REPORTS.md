# Urban Scooter — QA Bug Report Examples

## Project Overview
This document demonstrates bug reporting practices for the Urban Scooter web application, Android application, and REST API during TripleTen Quality Assurance training.

These are illustrative bug report examples based on testing scenarios. They are not presented as verified defects or actual Jira tickets.

---

## BUG-001: Order Form Accepts Invalid Input

**Platform:** Web Application
**Testing Type:** Functional / Negative Testing
**Status:** Example — Not Verified

### Preconditions
- Urban Scooter order form is open.

### Steps to Reproduce
1. Open the Urban Scooter order form.
2. Locate a required input field.
3. Enter a value outside the documented input requirements.
4. Attempt to proceed to the next step.

### Expected Result
The application rejects invalid input and displays the appropriate validation message.

### Example Actual Result
The form accepts invalid input and allows the user to continue.

### Impact
Invalid order information could be submitted.

---

## BUG-002: Android Order Notification Displays Incorrect Information

**Platform:** Android
**Testing Type:** Mobile / Functional Testing
**Status:** Example — Not Verified

### Preconditions
- Urban Scooter Android application is installed.
- A test order is available.

### Steps to Reproduce
1. Launch the Urban Scooter Android application.
2. Open the relevant order.
3. Trigger the specified notification event.
4. Review the notification details.

### Expected Result
The notification displays the correct order information at the time specified in the requirements.

### Example Actual Result
The notification contains incorrect order information or appears at the wrong time.

### Impact
Customers could receive misleading order updates.

---

## BUG-003: Courier API Returns Incorrect Response for Invalid ID

**Platform:** REST API
**Testing Type:** API / Negative Testing
**Endpoint:** DELETE /api/v1/courier/:id
**Status:** Example — Not Verified

### Preconditions
- Postman is available.
- The API test environment is accessible.

### Steps to Reproduce
1. Open Postman.
2. Create a DELETE request for the courier endpoint.
3. Supply an invalid or nonexistent courier ID.
4. Send the request.
5. Inspect the HTTP status and JSON response.

### Expected Result
The API returns the error status and response body documented for an invalid courier ID.

### Example Actual Result
The API returns a success response instead of the documented error response.

### Impact
Clients could incorrectly assume that a courier was deleted.

---

## Tools Used
- Jira — Defect documentation
- Postman — REST API testing
- Android Studio — Mobile testing
- Chrome and Opera — Web testing

## Note
Replace these examples with actual test execution evidence and confirmed Jira bug reports when available.
