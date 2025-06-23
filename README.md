# 🚗 Institute Parking Management System

A full-stack Parking Management System for IIIT Allahabad that allows registered users and visitors to search, book, and manage parking slots — with admin tools for efficient record-keeping and notifications.

---

## 🎯 Objective

To develop a parking management system where:
- Registered institute users can search and book empty parking slots.
- Visitors can pre-book slots ahead of arrival.
- Administrators can manage incoming and outgoing vehicle records efficiently.

---

## ⚙️ Tech Stack

- **Frontend**: React (Create React App)
- **Backend**: Node.js + Express
- **Database**: MySQL

---

## ✨ Key Features

- **Slot Management**: Real-time search and booking of slots with time-based rules.
- **Admin Features**: Manage vehicle records (plate number, name, phone number) and reserve slots.
- **User Features**: Book slots anytime by specifying start and end time.
- **Visitor Features**: Pre-book slots in advance with reservation confirmation.
- **Email Notifications**: Auto-emails for:
  - Parking time exceeded
  - Vehicle release
  - Booking/reservation status

---

## 🛠️ Admin Functionalities

- **Add Location**: 
  - Add new parking locations with images and slot counts (2W, 4W, Bus).
  - Auto-generate parking slots based on type.
  - `POST /admin/addLocation`

- **Delete Location**: 
  - Delete parking locations or slots.

- **Notifications**: 
  - Email confirmations and reminders for users.

- **Slot Management**: 
  - Occupied status after booking.
  - Automatic release after end time or cancellation.
  - View past/current/reserved bookings.

---

## 🙋‍♂️ Visitor Functionalities

- **Book Visitor Slot**: 
  - Pre-book slots with reservation status.

- **Confirm Visitor Slot**: 
  - Confirm booking upon arrival and activate the slot.

- **Automatic Release**: 
  - If not confirmed within 30 mins, slot is auto-released and booking is marked as "Released."

---

## 📬 Notifications

- Email updates sent at key booking moments:
  - After successful booking
  - Before release time
  - After release or cancellation

---
