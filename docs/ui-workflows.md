
**Content:**
```markdown
# User Interface Workflows — Online Booking

This document illustrates how UI documentation captures feature workflows from the user's perspective.

---

## 1. Booking Flow (Desktop)

**Step 1:** Customer selects a service from the Booking page.  
**Step 2:** System displays available staff and time slots.  
**Step 3:** User enters details and clicks **Book Appointment**.  
**Step 4:** Confirmation screen shows booking summary and email notification.

**UI Notes:**
- Button text: **Book Appointment**
- Tooltip: “Confirm time and staff before booking”
- Error state: “Selected slot unavailable — please choose another time.”

---

## 2. Booking Flow (Mobile)

Differences from desktop:
- Fewer visible staff cards; scroll enabled.
- Confirmation screen condensed into a modal view.
- Notifications triggered via push + email.

---

## 3. Staff Schedule Update Flow

**Primary persona:** Spa Manager  
**Objective:** Modify staff hours and availability.

Steps:
1. Navigate to **Staff → Profiles**.
2. Select staff → Edit working hours.
3. Save → System recalculates available slots.
4. Confirmation toast: “Staff schedule updated.”

---

**Last Updated:** November 2025  
**Maintainer:** Anwesha Roy
