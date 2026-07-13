# RouteNotes – Location Notes for Delivery Drivers
RouteNotes is a lightweight web application that lets delivery drivers (Amazon, UPS, FedEx, USPS, Spark, Roadie, etc.) save gate codes, access tips, walk‑through photos, GPS coordinates, and other location-specific notes. It is designed to run on a simple Linux VPS using PHP and MySQL, with RecurringStack providing authentication.

This project is intentionally minimal so it can be expanded and later wrapped into a mobile app for the Google Play Store.

---

## 🚚 Purpose
Delivery drivers constantly encounter:
- Locked gates with passcodes
- Hidden entrances or walk‑through paths
- Confusing apartment layouts
- Special instructions for buildings
- Dangerous or problematic locations

RouteNotes allows drivers to quickly save and retrieve these details.

---

## 🧱 Tech Stack
**Backend:** PHP 8+  
**Database:** MySQL  
**Auth:** RecurringStack (JWT or session-based)  
**Frontend:** HTML, CSS, JavaScript (mobile-friendly)  
**Hosting:** Any Linux VPS (Apache or Nginx)  
**Mobile App (future):** Capacitor wrapper for Android

---

## ✨ Core Features (MVP)
- Save a location with:
  - GPS coordinates
  - Gate codes
  - Access instructions
  - Walk‑through photos
  - Free‑form notes
 - Upvote or downvote tips, and gate codes
- Search saved locations by:
  - Name
  - Apartment complex
  - Address
- Mobile‑friendly UI for quick use during routes
- RecurringStack  login + user accounts (https://github.com/recurringstack/recurringstack-php)
- Simple dashboard listing saved locations

---

## 📂 Project Structure (initial)

/public
index.php
login.php
dashboard.php
save_location.php
view_location.php
search.php
upload_photo.php
/assets
/css
/js
/images

/app
auth.php
db.php
helpers.php

/database
schema.sql
