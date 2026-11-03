# FoodLoop – Community Food Redistribution Platform

## Project Summary
FoodLoop is a responsive, demo web application designed to reduce food waste by connecting donors with people or organizations who can use surplus food. The platform allows users to list available food, browse listings, request donations, and track the overall impact of food sharing in a community.

This project was created as a frontend mini-project to demonstrate how a community food-sharing system could work in a simple, user-friendly interface. It focuses on usability, clean design, and a realistic donation workflow without requiring a backend or database setup.

## Why This Project Exists
Food waste is a major issue in many communities. Meanwhile, many households, shelters, schools, or community groups need access to safe and nutritious food. FoodLoop aims to make this sharing process easier by creating a digital bridge between surplus food and people who need it.

The application is meant to be a concept demo, not a live production system, and it highlights how a community-driven platform could support food redistribution in a responsible and transparent way.

## Core Features
- Home page with community impact statistics
- Food listings with donor details, quantity, pickup location, and deadline
- Search and filter options for food listings
- Donation form to publish surplus food safely
- Request workflow for community members
- Request status tracking: pending, approved, rejected, and collected
- Impact dashboard with current statistics and recent community activity
- Responsive design for desktop, tablet, and mobile screens
- Local browser persistence using `localStorage`
- Reset demo data button for quick testing

## User Flow
1. A donor adds surplus food details such as category, quantity, location, and food safety notes.
2. Community members browse active listings and request available food.
3. The request is marked as pending or approved in the demo workflow.
4. A request can later be marked as collected to reflect pickup completion.
5. The dashboard updates to show community impact and food redistribution progress.

## Tech Stack
- HTML5 for structure
- CSS3 for styling and responsiveness
- Vanilla JavaScript for interactivity and state management
- LocalStorage for browser-based persistence
- Google Fonts for modern typography

## Project Structure
```text
FoodLoop_Project/
├── index.html       # Main UI structure of the application
├── style.css        # Page styling, colors, layout, and responsiveness
├── script.js        # Application logic, demo data, filtering, requests, and rendering
├── README.md        # Project documentation
└── .gitignore       # Optional project hygiene file (if present in your environment)
```

## Files Overview
### `index.html`
Contains the complete application layout, including:
- sidebar navigation
- home overview section
- browse listings page
- donation form page
- requests page
- impact dashboard
- modal and toast UI components

### `style.css`
Defines the visual identity of the project, including:
- soft eco-friendly color palette
- modern card layouts
- buttons and forms
- responsive breakpoints for mobile devices
- accessible spacing and typography

### `script.js`
Handles the interactive logic, including:
- initialization of demo data
- saving and loading data from `localStorage`
- rendering food cards and dashboard stats
- search and filtering behavior
- donation request handling
- updating request status
- showing toast notifications and modals

## How to Run
### Option 1: Open directly in browser
1. Download or extract the project folder.
2. Open the folder containing `index.html`.
3. Double-click `index.html`.
4. The application will open in your default browser.

### Option 2: Run a local web server
If you prefer a local server, you can run:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Demo Data Behavior
The project uses sample food donation entries and example request records. These are stored in the browser through `localStorage`, which means:
- the data remains available on the same browser/device
- refreshing the page preserves the current state
- the app behaves like a lightweight prototype without a backend database

## Food Safety Note
This application includes a food safety confirmation checkbox and guidance content for educational purposes. It does not replace real inspection, food handling procedures, or compliance requirements. In real-world use, food redistribution should follow local health regulations and food safety standards such as FSSAI guidelines.

## Current Limitations
This project is intentionally a frontend-only demo. It does not include:
- user authentication
- admin verification
- real-time database
- map-based location matching
- delivery coordination or chat features
- production-grade security
- backend APIs

## Future Enhancements
Possible next steps for a production-ready version include:
- backend with Node.js or PHP
- MySQL or MongoDB storage
- donor, recipient, and admin roles
- secure login and session management
- image uploads for food listings
- map integrations and geolocation
- notification system for requests and approvals
- reporting and analytics dashboard
- NGO verification workflow

## Project Goal
The main goal of FoodLoop is to encourage sustainable living by turning surplus food into a useful resource for the community. It demonstrates how a simple web application can support food sharing, reduce waste, and create a stronger sense of community collaboration.

## License
This project is a student/demo project intended for learning and educational purposes. It is not intended for commercial deployment without proper review, security testing, and legal compliance.

## Conclusion
FoodLoop is a practical and approachable prototype that showcases how technology can support social impact. It combines community-focused design with a realistic donation flow and demonstrates the value of using digital tools to promote food reuse and reduce waste.
