# Hotel Management UI/UX Design for ERPNext (Frappe v16)

## Goals
- Provide a modern, brandable UI layer that sits on top of ERPNext for hotel operations.
- Deliver clean workflow transitions across Rooms, Bookings, Check-ins/outs, Billing, Restaurant/Bar, Inventory, Waste, Laundry, and Travel Desk.
- Ensure mobile-friendly, quick task completion with role-based navigation.

## Brand System
**Brand tokens**
- Primary: `#1E5EFF` (brand blue)
- Accent: `#F6A609` (warm gold)
- Success: `#22C55E` | Warning: `#F97316` | Danger: `#EF4444`
- Background: `#F8FAFC` | Card: `#FFFFFF`

**Typography**
- Headings: Inter Semibold
- Body: Inter Regular
- Numeric emphasis: Inter Medium

**UI Components** (Frappe UI)
- Page shell with left rail + top bar (global search, notifications, quick create).
- Card-based dashboards (KPI tiles, charts, workflow queues).
- Unified "Task Drawer" for quick actions.
- Status chips for room and booking states.

---

## Information Architecture
### Primary Modules
1. **Front Desk**
   - Rooms
   - Bookings
   - Self Check-in
   - Counter Check-in
   - Counter Check-out
2. **Billing & Invoicing**
3. **Restaurant & Bar**
   - POS / Bar Management
   - Menu Management
   - Room Service
4. **Operations**
   - Inventory Management
   - Waste Management
   - Laundry Service
   - Travel Desk

### Role-Based Navigation
- **Front Desk Agent**: Rooms, Bookings, Check-in/out, Billing
- **Restaurant Manager**: POS/Bar, Menu, Room Service
- **Ops Manager**: Inventory, Waste, Laundry, Travel Desk
- **Finance**: Invoices, Payments, Statements

---

## Core Screens & Workflows

### 1) Rooms Dashboard
**Purpose:** Live room status and readiness.
- Visual grid of room cards with status chips: Available, Occupied, Cleaning, Maintenance, Reserved.
- Filters: floor, room type, housekeeping status, late checkout.
- Quick actions: Assign housekeeping, mark cleaned, open booking.

**Workflow**
1. Select room card → open room detail drawer.
2. Perform quick action (assign housekeeping, add issue, change status).

---

### 2) Bookings & Reservation Flow
**Booking List**
- Timeline or list with arrival/departure, status, payment state.
- Search by guest name, booking ID, phone.

**Create Booking**
- Stepper: Guest → Dates/Rooms → Rate Plan → Extras → Payment → Confirm.
- Real-time availability check and price breakdown.

---

### 3) Self Check-in (Guest-facing Kiosk/Mobile)
- Minimal UI with large buttons and QR/code input.
- Steps: Verify booking → ID capture → Payment → Room key activation.
- Status feedback with progress bar.

---

### 4) Counter Check-in
- Side-by-side split: guest info + room allocation.
- Actions: add upsells, collect payment, assign room/keys.

---

### 5) Counter Check-out
- Display charges summary with editable line items.
- Quick actions: apply discount, add late checkout fee, export invoice.

---

### 6) Billing & Invoicing
- Unified invoice screen with payments, refunds, and taxes.
- Print/email from action bar.
- Ledger view for finance.

---

### 7) Restaurant & Bar Management
**POS Screen**
- Fast item selection with categories, modifiers, and combos.
- Bill split and room-charge option.

**Menu Management**
- Menu builder with drag/drop categories.

**Room Service**
- Orders queue with SLA timer.
- Status: Pending → Preparing → Delivering → Completed.

---

### 8) Inventory Management
- Reorder levels with alert badges.
- Stock movement logs with filters.
- Request to purchase and GRN quick actions.

---

### 9) Waste Management
- Waste log form with category, reason, and photos.
- Analytics card for waste cost and trends.

---

### 10) Laundry Service
- Linen/guest laundry tracking.
- Ticket-based workflow with statuses and turnaround SLA.

---

### 11) Travel Desk
- Booking services (taxi, tours).
- Partner list and commission tracking.

---

## Cross-Module UX Patterns
- **Global Search:** searchable by guest, booking, room, invoice.
- **Quick Create:** booking, room service order, invoice.
- **Notification Center:** guest arrival, late checkout, unpaid invoices.
- **Consistent Status Chips:** reused across modules.

---

## Workflow Transitions
- Booking → Check-in → Room Status update.
- Room Service / Restaurant charges → Billing.
- Check-out → Invoice → Payment.
- Inventory consumption → Waste / Laundry usage.

---

## Frappe UI Implementation Notes
- Use Frappe UI Layouts (Page, Card, Drawer).
- Standardized forms with auto-save.
- Utilize List Views with custom filters and Kanban for bookings.
- Use Frappe Charts for KPIs.

---

## Deliverables
- UI design tokens
- Module dashboards and detailed list views
- Workflow transitions with quick actions and task drawers

