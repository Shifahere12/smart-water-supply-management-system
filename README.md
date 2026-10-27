# Smart Water Supply Management System

An IoT-inspired web platform for publishing water supply schedules, tracking complaints, verifying shortages and monitoring tank levels in Karachi, Pakistan.

Built as a university project at the Department of Computer Science, Dawood University of Engineering & Technology (DUET).

**Live demo:** https://shifahere12.github.io/smart-water-supply-management-system/

## Problem

Water supply in many Karachi areas is irregular, and residents have no reliable way to know when water will arrive, report a failure, or see whether other areas face the same problem. Manual valves and meters also lead to leakage, theft and unfair distribution.

## Features

### Public website
- Home page with area search, live supply countdown and latest public notices
- Area explorer, public water status and a shortage and problem map
- Water line map showing working, leaking, damaged and choked lines
- About page, login and registration

### Resident dashboard
- Next scheduled supply with live countdown and schedule change history
- Report whether supply arrived, arrived late or did not arrive
- Tank tracker with live level, manual readings and trend chart
- Complaints with photo or video evidence and ticket follow-up
- Emergency tanker requests
- Notifications and alerts, including low tank warnings

### Staff dashboard
- Assigned complaints with deadlines and resolution notes
- Record supply outcomes and operational updates
- Review community reports and flag discrepancies

### Administrator dashboard
- Overview of areas, schedules, unresolved complaints and household tank levels
- Area management and schedule publishing with a recorded reason for each change
- Complaint assignment and status updates
- Community verification: three or more independent "supply did not arrive" reports flag an area for checking
- Analytics: areas with most shortages, zones with most delays, average delay per area, longest unresolved complaint categories
- Shortage risk forecast for the next 7 days
- Tanker request approvals, CSV report download, user roles and audit log

## Technologies

- HTML5, CSS3 and vanilla JavaScript (no frameworks)
- Browser `localStorage` for demo data
- Responsive layout, scroll animations and SVG charts and maps

## Project structure

```
smart-water-supply-management-system/
├── index.html    page structure
├── style.css     navy and white theme, animations
├── app.js        routing, data, dashboards and features
└── README.md
```

## How to run

1. Download or clone this repository.
2. Open `index.html` in a browser, or run it with the VS Code **Live Server** extension.

No installation or build step is needed.

## Demo accounts

Password for every account: `1234`

| Role | Username |
|------|----------|
| Resident | `ayesha`, `bilal`, `sana`, `hamza`, `nida`, `omar` |
| Staff | `staff1`, `staff2` |
| Administrator | `admin` |

## Limitations

- This is a front-end prototype. All data is demonstration data stored in the browser, not in a server database.
- Tank levels and shortage forecasts are simulated. No real sensors are connected.
- Photos and videos larger than about 350 KB are only visible until the page is reloaded.
- Login is for demonstration only and is not secure.

## Future work

- MySQL backend with a REST API
- Real IoT sensors (ultrasonic level sensor, flow sensor, NodeMCU) sending data to the cloud
- Machine learning for leak and shortage prediction
- GIS-based map of real pipelines
- SMS notifications and consumption-based billing

## Licence

This project was created for educational purposes.
