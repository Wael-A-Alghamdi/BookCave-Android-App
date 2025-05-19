# BookCave – Android Bookstore App

BookCave is a fully functional Android application for managing a digital bookstore. It includes two distinct user roles: **Customer** and **Seller**, each with their own UI, features, and workflows. The app allows book browsing, ordering, renting, profile management, seller uploads, and payment history tracking — all handled locally within the app.

---

## 📱 Main Features

### 👤 Customer Features
- Login / Registration  
- Browse and search books  
- View book details  
- Rent or buy books  
- View current and past orders  
- Track payment history  
- Edit profile (username, password, address, etc.)

### 🛒 Seller Features
- Login / Registration  
- Upload and manage book listings  
- Accept or reject incoming orders  
- View active and completed sales  
- Track payment history from customers  
- Edit seller profile  

### ⚙ Shared App Features
- Fully separate home screens for customers and sellers  
- Navigation drawer and bottom navigation bar per user type  
- Uses Activities and Fragments for modular UI  
- Custom dialogs for confirmations, form inputs, etc.  
- Local data persistence via model logic (no server/backend)

---

## 🛠 Tech Stack

- **Java** (Android SDK)
- **Android Studio**
- **Activities & Fragments**
- **Custom Adapters (RecyclerView)**
- **DrawerLayout + BottomNavigationView**
- **Intent-based navigation**
- **ConstraintLayout / RelativeLayout for UI**
- **Resource-based menus, layouts, strings, drawables**

---

## 📁 Project Structure

BookCave/

├── activities/ # Login, Home screens for customer & seller

├── ui/ # Fragments for each section (home, search, profile)

│ ├── search/ # Book search + filter system

│ ├── home/ # Book previews

│ ├── seller_booklist/ # Seller's uploaded books

│ ├── seller_currentorders/ # Active order list

│ ├── seller_profile/ # Seller info screen

│ └── profile/ # Customer profile & history

├── profile/ # About, ContactDeveloper, OrderHistoryC, PaymentHistoryC

├── extras/ # RecyclerView adapters, models, utility functions

├── res/

│ ├── layout/ # XML files for all screens and list rows

│ ├── drawable/ # App icons, backgrounds, buttons

│ ├── menu/ # Drawer menus and top action menus

│ └── values/ # Strings, colors, styles

├── AndroidManifest.xml

├── build.gradle

└── README.md

---

## 📝 Notes

- This app does **not** use a backend or database — all logic is handled client-side for demo purposes.
- User and seller actions are simulated using static logic and in-memory object storage.
- No payment gateway integration — only mock payment history screens exist.
- The app is optimized for smartphones only (portrait orientation).

---

## 🚀 Getting Started

1. Open the project in **Android Studio**.
2. Sync Gradle and resolve dependencies.
3. Use **"Run"** to launch on an emulator or connected Android device.
