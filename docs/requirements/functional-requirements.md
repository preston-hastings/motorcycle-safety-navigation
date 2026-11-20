# Functional Requirements

## Motorcycle Safety Navigation Android Application

### 1. Purpose

This document defines the functional requirements for the Motorcycle Safety Navigation Android application.

The application aims to help motorcycle riders identify areas with historical collision concentrations and make more informed route choices through interactive mapping, GPS navigation and safety-aware route planning.

### 2. Scope

The application will be developed as a native Android prototype using Kotlin and Jetpack Compose.

The proposed functionality includes:

- Interactive mapping
- GPS-based location tracking
- Destination search
- Route generation and visualisation
- Historical motorcycle collision hotspot identification
- Safety-aware route comparison
- Location-based safety warnings

The prototype will use historical collision data as an indication of potential risk, rather than as a prediction of future accidents.

### 3. Functional Requirements

#### FR1 — Interactive Map

**Priority:** Must Have

The application shall display an interactive map that allows users to view and explore geographical locations.

**Acceptance Criteria:**
- The map loads successfully when the application is opened.
- Users can zoom and pan around the map.
- Map loading failures are handled appropriately.

#### FR2 — GPS Location Tracking

**Priority:** Must Have

The application shall obtain the device's geographical location, subject to the user's permission, and display it on the map.

**Acceptance Criteria:**
- The application requests location permission before accessing GPS data.
- The user's current location is displayed on the map.
- Location updates are reflected as the device moves.
- The application handles denied permissions appropriately.

#### FR3 — Destination Search

**Priority:** Must Have

The application shall allow users to search for and select a destination.

**Acceptance Criteria:**
- Users can enter a destination into a search interface.
- Relevant destination results are displayed.
- Users can select a destination.
- Invalid or unsuccessful searches produce appropriate feedback.

#### FR4 — Route Generation

**Priority:** Must Have

The application shall generate and display a route between the user's starting location and selected destination.

**Acceptance Criteria:**
- A route can be requested between two valid locations.
- The calculated route is displayed on the map.
- Route distance and estimated travel time are presented when available.
- Route generation failures are handled appropriately.

#### FR5 — Motorcycle Collision Hotspot Visualisation

**Priority:** Must Have

The application shall identify and display areas with concentrations of historical motorcycle collisions using an appropriate collision dataset.

**Acceptance Criteria:**
- Relevant historical collision data can be loaded.
- Collision hotspots are identified using a documented method.
- Hotspots are displayed geographically on the map.
- Users can visually distinguish hotspot areas from ordinary map features.

#### FR6 — Safety-Aware Route Planning

**Priority:** Must Have

The application shall assess generated routes using historical motorcycle collision information and provide a safety-aware route option where technically feasible.

**Acceptance Criteria:**
- Route assessment incorporates collision-related information.
- The application can compare route options using a documented risk-scoring approach.
- Users can identify the route recommended by the safety-aware calculation.
- The application communicates that historical collision data does not guarantee route safety.

#### FR7 — Location-Based Safety Warnings

**Priority:** Should Have

The application shall provide location-based warnings when a rider approaches an identified collision hotspot.

**Acceptance Criteria:**
- The application determines when the user's location is within a defined warning distance of a hotspot.
- An appropriate warning is presented.
- Repeated warnings are controlled to avoid unnecessary distraction.
- Warnings do not prevent the user from continuing navigation.

#### FR8 — Route Information Display

**Priority:** Should Have

The application shall display relevant information about a selected route.

**Acceptance Criteria:**
- Users can view the route's starting point and destination.
- Route distance is displayed when available.
- Estimated travel time is displayed when available.
- Safety-related route information is presented clearly.

### 4. Requirement Prioritisation

Requirements are prioritised using the MoSCoW method:

- **Must Have:** Essential functionality required for the prototype.
- **Should Have:** Important functionality that will be implemented where feasible.
- **Could Have:** Optional enhancements.
- **Won't Have (Current Scope):** Functionality excluded from the current prototype.

Priorities may be revised following technical research and feasibility evaluation.

### 5. Dependencies and Constraints

- Mapping and routing functionality depends on the selected APIs and their capabilities.
- Hotspot detection depends on the availability and quality of historical collision data.
- GPS functionality depends on device location services and user permissions.
- Safety-aware route generation may require additional route-processing logic.
- The prototype must remain achievable within the project's available development time.

### 6. Verification

Each functional requirement will be verified through appropriate testing, including emulator testing, integration testing and evaluation against its acceptance criteria.

Testing evidence and results will be documented during development.


