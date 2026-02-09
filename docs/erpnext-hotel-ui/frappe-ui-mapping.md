# Frappe UI Implementation Mapping

## Layouts
- **Page** for dashboards and list views.
- **Card** for KPI tiles and summary panels.
- **Drawer** for quick actions and inline edits.

## List Views & Filters
- Use Frappe list views with custom filters for rooms, bookings, and invoices.
- Apply Kanban views for bookings and room-service queues.

## Forms
- Standardized forms with auto-save.
- Inline validation for guest ID, payment, and rate plans.

## Charts
- Use Frappe Charts for occupancy, revenue, and service SLAs.

## Implementation Notes
- Extend ERPNext DocTypes for hotel-specific fields.
- Use Frappe UI route guards for role-based navigation.
- Preserve ERPNext metadata and print formats.
