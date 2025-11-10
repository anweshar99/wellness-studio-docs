# API Reference — Wellness Studio (Demo)

This section simulates product-facing API documentation used by partners or developers integrating with the Wellness Studio SaaS platform.

---

## 1. Authentication

All API requests require an API key.

**Header Example**
Authorization: Bearer <your_api_key>
Content-Type: application/json

**Response Example**
```json
{
  "status": "success",
  "message": "Authenticated successfully"
}
2. Endpoint — Create a Booking

POST /v1/bookings/create

Creates a new booking for a customer.
| Parameter     | Type   | Required | Description                   |
| ------------- | ------ | -------- | ----------------------------- |
| `customer_id` | string | ✅        | Unique ID for the customer    |
| `service_id`  | string | ✅        | ID of the service booked      |
| `staff_id`    | string | ✅        | Assigned staff member         |
| `start_time`  | string | ✅        | Start time in ISO 8601 format |
Request Example

{
  "customer_id": "CUST102",
  "service_id": "SER567",
  "staff_id": "STF34",
  "start_time": "2025-11-12T10:00:00Z"
}


Response Example

{
  "booking_id": "BKG2301",
  "status": "confirmed"
}

3. Endpoint — Cancel a Booking

POST /v1/bookings/cancel

Cancels an existing booking by ID.
| Parameter    | Type   | Required | Description                  |
| ------------ | ------ | -------- | ---------------------------- |
| `booking_id` | string | ✅        | ID of the booking to cancel  |
| `reason`     | string | ❌        | Optional cancellation reason |
4. Errors
| Code | Message       | Description                         |
| ---- | ------------- | ----------------------------------- |
| 400  | Invalid Input | One or more required fields missing |
| 401  | Unauthorized  | Invalid API key                     |
| 404  | Not Found     | Booking does not exist              |
| 500  | Server Error  | Internal system issue               |
Version: v1.0
Maintainer: Anwesha Roy
Last updated: November 2025


✅ **Value added:** demonstrates you can document APIs, explain parameters, show examples, and format developer content clearly.

---

### **2. Add a “User Interface Workflows” Document**

**Goal:** Show understanding of UX documentation and task flows (how a feature works end-to-end).

📁 Create:
