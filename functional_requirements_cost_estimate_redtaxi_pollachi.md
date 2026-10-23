# Functional Requirements Specification (FRS) & Commercial Proposal
**Project Name:** RedTaxi Pollachi – Outstation & City Cabs Booking Platform  
**Document Version:** 1.0  
**Reference Prototype:** `redtaxi-pollachi-outstation-city-cabs.ai.studio`  

---

## 1. Executive Summary
This document outlines the functional specifications and commercial estimate for the development of the **RedTaxi Pollachi Outstation & City Cabs** platform. The objective is to provide a seamless, digital-first cab booking experience for local city commutes, intercity outstation rides, and curated tourist packages across Pollachi and surrounding destinations (Valparai, Topslip, Palani, Athirappilly, Coimbatore, Ooty, etc.), backed by a centralized fleet and tariff management system.

---

## 2. System Actors & User Roles
1. **Customer / Passenger:** End-users browsing tariffs, calculating trip estimates, and booking city cabs, outstation drops, or tour packages.
2. **Driver Partner:** Chauffeurs receiving trip assignments, viewing customer pickup locations, recording odometer readings, and logging trip completion.
3. **Administrator / Fleet Dispatcher:** Operations managers handling booking confirmations, driver allocations, tariff updates, and billing reports.

---

## 3. Detailed Functional Requirements

### 3.1. User Authentication & Profile Management
* **FR-1.1: Mobile OTP Authentication:** Customers can register and log in using their mobile number via SMS/WhatsApp OTP verification.
* **FR-1.2: Guest Booking Flow:** Users can quickly calculate fares and initiate bookings by entering their Name and Phone Number without mandatory account creation.
* **FR-1.3: User Profile & Saved Addresses:** Registered users can store personal details, GST details (for corporate billing), emergency contacts, and favorite pickup/drop locations.
* **FR-1.4: Booking History:** Users can view a complete log of upcoming, ongoing, and past trips along with downloadable invoices.

### 3.2. Service Discovery & Trip Selection
* **FR-2.1: Multi-Mode Service Selector:** Interactive tab interface allowing users to switch between:
  * **City Cabs / Local Rentals:** Point-to-point city transfers and hourly/kilometer rental packages (e.g., 4 Hrs / 40 Km, 8 Hrs / 80 Km).
  * **Outstation Trips:** One-Way Drop and Round-Trip intercity bookings.
  * **Sightseeing & Tour Packages:** Curated regional packages (e.g., Pollachi to Valparai, Topslip Parambikulam, Aliyar Dam, Palani, Athirappilly Falls) with fixed duration and vehicle pricing.
* **FR-2.2: Vehicle Fleet Showcase:** Categorized display of available vehicles with seating capacity, luggage limit, AC status, and per-km tariff:
  * **Hatchback / Mini:** (e.g., WagonR, Indica – 4+1 Seater)
  * **Sedan:** (e.g., Dzire, Etios – 4+1 Seater)
  * **SUV / MUV:** (e.g., Innova, Ertiga, Marazzo – 6+1 / 7+1 Seater)
  * **Tempo Traveller / Coach:** (12+1 to 20+1 Seater for group tours)

### 3.3. Booking & Ride Management Workflow
* **FR-3.1: Location Search & Autocomplete:** Integration with Map APIs to search and select exact pickup and drop-off points, with automatic distance and duration calculation.
* **FR-3.2: Schedule Management:** Support for both immediate dispatch ("Ride Now") and advance reservations ("Ride Later") with date and time pickers.
* **FR-3.3: Multi-Stop Itinerary:** Ability to add intermediate waypoints for outstation trips and custom sightseeing tours.
* **FR-3.4: Instant Booking Confirmation:** Generation of a unique Booking ID upon submission, followed by automated confirmation alerts via WhatsApp, SMS, and Email.

### 3.4. Fare Calculation & Pricing Engine
* **FR-4.1: Dynamic Fare Estimator:** Automatic calculation of estimated trip cost based on:
  * Base fare and minimum billable kilometers per day (e.g., 250 km/day for outstation).
  * Per-kilometer rate according to vehicle class.
  * Driver Allowance (Bata) calculated per day or for night driving hours (10:00 PM – 6:00 AM).
* **FR-4.2: Transparent Cost Breakdown:** Clear display of inclusions and exclusions (e.g., Toll charges, Interstate Permits, Hill Station charges, and Parking fees billed at actuals).
* **FR-4.3: Promo Codes & Discounts:** Support for applying coupon codes for seasonal discounts or frequent-rider rewards.

### 3.5. Live Tracking, Communication & Safety
* **FR-5.1: Driver & Cab Details Assignment:** Sharing assigned Driver Name, Contact Number, Vehicle Model, and Registration Number prior to pickup.
* **FR-5.2: Trip Start/End Verification:** Odometer reading capture or OTP verification at pickup and drop-off to ensure accurate billing for extra kilometers/hours.
* **FR-5.3: Quick WhatsApp/Call Support:** Direct floating action buttons for instant 24/7 customer care call or WhatsApp inquiry.
* **FR-5.4: SOS / Emergency Alert:** In-trip emergency button allowing passengers to share their live trip details with emergency contacts and the admin control room.

### 3.6. Driver & Vendor Portal
* **FR-6.1: Driver Onboarding & KYC:** Record management for Driver License, Aadhaar, Vehicle RC, Fitness Certificate, and Insurance validity alerts.
* **FR-6.2: Duty & Trip Assignment:** Drivers receive trip details (Customer Name, Pickup Time, Route, Collect Cash amount) via the driver web portal or WhatsApp bot.
* **FR-6.3: Trip Expense Logging:** Ability for drivers to upload toll/parking receipts and closing kilometer readings at the end of an outstation trip.

### 3.7. Admin Dashboard & Operations Control
* **FR-7.1: Centralized Booking Management:** Real-time dashboard to view new inquiries, confirm bookings, modify itineraries, or handle cancellations.
* **FR-7.2: Manual & Automated Dispatch:** Assign available vehicles and drivers to confirmed bookings and trigger automated customer notifications.
* **FR-7.3: Tariff & Package CMS:** Dynamic master settings allowing the admin to update per-km rates, base fares, driver bata, and tour package prices without developer intervention.
* **FR-7.4: Invoicing & Financial Reports:** Automated generation of downloadable PDF trip bills (GST / Non-GST) and analytics on daily/monthly bookings, revenue, and driver payouts.

---

## 4. Non-Functional Requirements (NFR)
* **NFR-1: Mobile-First Responsiveness:** Seamless performance across all smartphones, tablets, and desktop browsers (Progressive Web App ready).
* **NFR-2: Fast Load Times & Local SEO:** Optimized page speed and structured metadata targeting regional search keywords (e.g., *"Pollachi Call Taxi"*, *"Pollachi to Valparai Cab Booking"*).
* **NFR-3: Security & Data Privacy:** SSL encryption (HTTPS), secure API handling, and protected administrative routes.

---

## 5. Commercial Bill Estimate (Quotation)

### Option A: Web-First Booking & Admin Dispatch Portal (Standard Scope)
*Best suited for launching an interactive booking portal with automated fare calculation, WhatsApp/SMS notifications, and full Admin control.*

| S.No | Module / Deliverable | Timeline | Cost (INR) |
| :--- | :--- | :--- | :--- |
| 1 | **Responsive UI/UX & Customer Frontend** (City, Outstation, Tour Packages) | 1 Week | ₹10,000 |
| 2 | **Fare Calculation Engine & Map Distance Integration** | 1.5 Weeks | ₹12,000 |
| 3 | **Customer Booking Flow & WhatsApp/SMS Notification Integration** | 1.5 Weeks | ₹10,000 |
| 4 | **Admin Dashboard** (Bookings, Driver Allocation, Dynamic Rate Card CMS) | 2 Weeks | ₹15,000 |
| 5 | **Payment Gateway Integration & Automated PDF Invoice Generator** | 1 Week | ₹6,000 |
| 6 | **Quality Assurance, Cloud Deployment, SSL & Handover Training** | 1 Week | ₹5,000 |
| **Total** | **Total One-Time Development Cost** | **~5 to 6 Weeks** | **₹58,000** |

---

### Option B: Full-Scale Aggregator Suite (Web + Android/iOS Apps)
*Best suited for large-scale fleet automation with dedicated Customer & Driver mobile applications and live GPS tracking.*

| S.No | Module / Deliverable | Timeline | Cost (INR) |
| :--- | :--- | :--- | :--- |
| 1 | **Customer Web Portal + Native/Cross-Platform Mobile App (Android & iOS)** | 4 Weeks | ₹60,000 |
| 2 | **Driver Partner Mobile App** (Duty Toggle, Live Navigation, Odometer Log) | 3 Weeks | ₹45,000 |
| 3 | **Real-Time Socket Backend & Automated Nearest-Cab Dispatch Engine** | 3 Weeks | ₹50,000 |
| 4 | **Master Admin & Vendor Management ERP Panel** | 2 Weeks | ₹30,000 |
| 5 | **Testing, Cloud Architecture Setup & App Store/Play Store Publishing** | 2 Weeks | ₹15,000 |
| **Total** | **Total One-Time Development Cost** | **~12 Weeks** | **₹2,00,000** |

---

## 6. Third-Party & Recurring Infrastructure Costs (Borne by Client)
* **Domain Name (`.com` / `.in`):** ₹800 – ₹1,200 / year
* **Cloud Server & Database Hosting:** ₹1,000 – ₹3,000 / month (depending on traffic)
* **Google Maps API (Places & Distance Matrix):** Covered under Google's free monthly tier for low-to-medium traffic; billed on actual usage thereafter.
* **WhatsApp Business API / SMS Gateway:** ~₹0.15 to ₹0.80 per notification sent.