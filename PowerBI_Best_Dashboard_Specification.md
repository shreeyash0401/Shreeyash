# BEST POWER BI DESIGN — IT HELPDESK & TICKET RESOLUTION

## Page 1 — EXECUTIVE OVERVIEW
Purpose: Management-level snapshot.

HEADER:
IT HELPDESK & TICKET RESOLUTION ANALYTICS
Subheader: Service Desk Performance | SLA | Workload | Resolution

SLICERS:
Date | Department | Priority | Category | Technician

KPI CARDS:
1. Total Tickets
2. Resolved Tickets
3. Open Tickets
4. SLA Compliance %
5. Avg Resolution Time
6. Avg CSAT

VISUAL GRID:
Left large: Created vs Resolved Tickets by Month (line/column combo)
Right: SLA Met vs Breached (donut)
Bottom-left: Tickets by Category (horizontal bar)
Bottom-middle: Tickets by Priority (stacked bar)
Bottom-right: Tickets by Department (bar)
Footer: Open ticket backlog + critical ticket indicator

## Page 2 — RESOLUTION & SLA
Purpose: Find delays and SLA problems.

KPIs:
Avg Response Time | Avg Resolution Time | SLA Met % | SLA Breached % | Reopened | Escalated

Visuals:
- Resolution Time by Category
- Resolution Time by Priority
- SLA Compliance by Month
- SLA Compliance by Technician
- SLA Met vs Breached by Priority
- Backlog Aging (0–1, 2–3, 4–7, 8–14, 15+ days)

## Page 3 — TECHNICIAN PERFORMANCE
Purpose: Workload balancing and performance.

KPIs:
Total Technicians | Tickets/Technician | Avg Resolution | SLA %

Visuals:
- Technician Workload
- Technician SLA Compliance
- Technician Avg Resolution Time
- Technician CSAT
- Top 5 / Bottom 5 performers
- Workload vs SLA scatter chart

Table:
Rank | Technician | Tickets | Resolved | SLA % | Avg Resolution | CSAT

## Page 4 — TICKET INTELLIGENCE
Purpose: Drill into operational patterns.

Visuals:
- Category × Priority matrix
- Monthly ticket trend
- Ticket Status distribution
- Issue Category trend
- Reopened tickets by category
- Detailed ticket table

Ticket table:
Ticket ID | Date | Department | Category | Priority | Technician | Status |
Response Time | Resolution Time | SLA Status | CSAT

## NAVIGATION
Bottom navigation:
Overview | Resolution & SLA | Technician Performance | Ticket Intelligence

## DESIGN
Use a professional dark IT-operations theme inspired by the reference dashboard, but use original labels/layout.
Recommended accent meaning:
Green = healthy/met SLA
Red = breach/critical
Orange = warning/high
Blue = informational

Keep visual count controlled. Prioritize readable KPI cards, trend charts, SLA visuals, and operational tables.

## DATA MODEL
Recommended star schema:
Calendar → Helpdesk Tickets ← Technicians
                       ← Departments
                       ← Categories
                       ← Priority

For a college project, a single cleaned ticket table plus Calendar table is sufficient.
