# User guide — Common tasks

## 1. Create a new service
1. Dashboard > Services > Add service.
2. Enter service name, duration, price, and select required skills.
3. Click **Save**.

**Tip:** Set duration to actual service time + cleanup buffer if needed.

## 2. Add or update staff schedule
1. Dashboard > Staff > Select staff.
2. Click **Working hours** > Add day/time ranges (e.g., Mon 09:00–17:00).
3. Save. Repeat for each staff.

## 3. Manage bookings
- **View bookings:** Dashboard > Bookings. Filters: date, staff, status.
- **Cancel booking:** Select booking > Cancel > Enter reason (optional). Customer receives cancellation message.
- **Reschedule booking:** Edit booking date/time and notify customer.

## 4. Configure notifications
1. Dashboard > Settings > Notifications.
2. Enable email or SMS reminders. Edit message templates.
3. Use variables: `{{customer_name}}`, `{{booking_time}}`, `{{service_name}}`.

## 5. Common maintenance tasks
- Export bookings: Bookings > Export CSV.
- Bulk update staff skills: Staff > Bulk edit (CSV upload).

## Example flow — New customer books online
1. Customer selects service on booking page.
2. Customer picks available staff/time slot.
3. Customer provides contact details and pays (if required).
4. System sends confirmation email and reminder 24 hours before appointment.
