# Homework 2: Work Breakdown Structure 
**Project:** Smart Parking Platform  
**Company:** Software Corp.  
**Date:** September 17, 2026  

---

## 1. Work Breakdown Structure (WBS)

### 1.0 Smart Parking Platform

#### 1.1 User Authentication and Profile Management
* **1.1.1 User Registration Module**
  * 1.1.1.1 Driver account creation interface (Name, Email, Phone, Password)
  * 1.1.1.2 Vehicle information registration (Make, Model, License Plate Number)
  * 1.1.1.3 Two-factor SMS and email verification setup
* **1.1.2 User Login and Session Handling**
  * 1.1.2.1 Secure token generation and OAuth 2.0 integration
  * 1.1.2.2 Password reset workflow and encrypted email recovery dispatch
  * 1.1.2.3 Persistent session state and automatic token timeout rules
* **1.1.3 Profile and Credential Administration**
  * 1.1.3.1 User profile edit screen (Update personal and vehicle records)
  * 1.1.3.2 Saved payment method vaulting (Tokenized card storage via PCI gateway)
  * 1.1.3.3 Account deactivation and data purge processing

#### 1.2 User and Operator Account Administration
* **1.2.1 Role-Based Access Control (RBAC) System**
  * 1.2.1.1 User role definition (Driver, Facility Operator, Support Admin)
  * 1.2.1.2 Role permission matrix implementation across backend endpoints
* **1.2.2 Operator Onboarding Workflow**
  * 1.2.2.1 Commercial garage business verification application form
  * 1.2.2.2 Facility proof documentation upload and administrative review queue
  * 1.2.2.3 Facility operator credentials generation and dispatch
* **1.2.3 User Management Console**
  * 1.2.3.1 Administrative user search, filtering, and detail inspection portal
  * 1.2.3.2 Account suspension, lockout, and password unlock controls
  * 1.2.3.3 Staff role assignment and privilege escalation workflows

#### 1.3 Dashboards and Core Application Portals
* **1.3.1 Operator Facility Management Dashboard (Web Portal)**
  * 1.3.1.1 Add, edit, or remove garage location details and facility metadata
  * 1.3.1.2 Floor plan configuration (Levels, total stalls, EV and ADA stalls)
  * 1.3.1.3 Real-time stall status editor (Mark stalls offline for maintenance)
  * 1.3.1.4 Dynamic pricing and surge rate rule configuration interface
* **1.3.2 Driver Search, Booking, and Payment Portal (Mobile Application)**
  * 1.3.2.1 GPS-enabled interactive map showing nearby garages with live open spots
  * 1.3.2.2 Garage detail cards (Hourly rates, operating hours, clearance heights)
  * 1.3.2.3 Space reservation selection, arrival window, and 5-minute stall hold
  * 1.3.2.4 In-app checkout flow with Apple Pay, Google Pay, and credit card processing
  * 1.3.2.5 Digital pass generation with QR code and active booking countdown
* **1.3.3 Navigation and Access Control Integration**
  * 1.3.3.1 External map routing deep link (Google Maps and Apple Maps to gate)
  * 1.3.3.2 Gate reader API integration (QR scanner and License Plate Recognition)
  * 1.3.3.3 Real-time check-in and check-out entry state transition handlers

#### 1.4 Analytics, Reporting, and Alerts
* **1.4.1 Real-Time System Telemetry and Notifications**
  * 1.4.1.1 Automated push notifications (15-minute expiration alerts)
  * 1.4.1.2 Overstay detection service and dynamic penalty charge calculator
  * 1.4.1.3 High-occupancy threshold alerts (Notifying operators when facility reaches 95%)
* **1.4.2 Occupancy Reporting Subsystem**
  * 1.4.2.1 Live occupancy metrics aggregation per floor and facility
  * 1.4.2.2 Historical space turnover rate graph visualization
  * 1.4.2.3 Peak congestion hours and dwell-time trend charts
* **1.4.3 Financial and Transaction Reporting**
  * 1.4.3.1 Operator gross and net revenue dashboard summaries
  * 1.4.3.2 Transaction audit log search and dispute tracking
  * 1.4.3.3 Automated CSV and PDF export generator for accounting reconciliation

  ---

## 2. Project Timeline & Gantt Schedule (16-Week Semester)

### 2.1 Visual Gantt Chart

```mermaid
gantt
    title Smart Parking Platform - 16-Week Project Timeline
    dateFormat  YYYY-MM-DD
    axisFormat  %b %d

    section Phase 1: Planning & Scope
    Project Kickoff & SRS Formulation       :done,    task1, 2026-09-01, 2026-09-14
    WBS & Project Scheduling                :active,  task2, 2026-09-15, 2026-09-21

    section Phase 2: Architecture & Auth
    Database Architecture & API Scaffolding :         task3, 2026-09-22, 2026-09-28
    Authentication & Session Security       :         task4, 2026-09-29, 2026-10-05
    RBAC & Operator Onboarding Module       :         task5, 2026-10-06, 2026-10-12

    section Phase 3: Portals & Hardware Sync
    Operator Facility Management Portal     :         task6, 2026-10-13, 2026-10-19
    Driver Interactive Map & Search UI      :         task7, 2026-10-20, 2026-10-26
    Reservation Engine & Payment Processing :         task8, 2026-10-27, 2026-11-02
    Gate Control & QR Pass Validation       :         task9, 2026-11-03, 2026-11-09

    section Phase 4: Analytics & Alerts
    Notification Daemon & Overstay Alerts   :         task10, 2026-11-10, 2026-11-16
    Occupancy Reporting & Financial Exports :         task11, 2026-11-17, 2026-11-23

    section Phase 5: Verification & Launch
    End-to-End System Load & Stress Testing :         task12, 2026-11-24, 2026-11-30
    Security Audit & Bug Remediation        :         task13, 2026-12-01, 2026-12-07
    Final System Acceptance & Staging Prep  :         task14, 2026-12-08, 2026-12-14
    Final Deliverable & Live Demonstration  :         task15, 2026-12-15, 2026-12-18