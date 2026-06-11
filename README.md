# Restaurant Package Booking

Flutter Android application for premium private dining reservations. Customers can browse curated menu packages without login, register/login, book by event date/time and guest count, see live per-guest pricing, manage reservations, and administrators can manage packages, users, and all bookings.

## Tech Stack

- Flutter + Material 3
- `go_router` for routing
- `flutter_riverpod` for state management
- `sqflite` + `path` for SQLite database `restaurant_package_booking.db`
- `shared_preferences` for session persistence
- `cached_network_image` for package images
- `intl` for date/time/currency formatting
- `uuid` for local IDs

## Demo Accounts

- Customer: `guest@luxe.test` / `guest123`
- Admin: `admin@luxe.test` / `admin123`

## Run

Install Flutter first, then run:

```powershell
flutter pub get
flutter run
```

If this folder does not contain native Android wrapper files yet, run this once from the project root:

```powershell
flutter create --platforms=android .
flutter pub get
flutter run
```

## Core Features

- Guest package browsing with search and category filter
- Customer registration and unified role-aware login
- Booking form with event date, event time, number of guests, optional service customizations, and live price calculation
- Summary confirmation and success notification
- My Reservations with view, update, and cancel flows
- Admin dashboard for package CRUD, user management, and reservation management
