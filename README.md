# christoffelmenuAppCode
Christoffel's Fine Dining Menu Manager
A sophisticated React Native mobile application for managing a luxury restaurant menu with an elegant, multi-screen interface.

https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white

App Overview
A complete restaurant management solution with separate interfaces for staff and customers, featuring a luxurious dark theme design.

 Features
 Multi-Screen Navigation
Login Screen - Elegant welcome interface
Home Screen - Main dashboard with background imagery
Add Menu Screen - Complete dish management form
Menu List Screen - Staff view of all menu items
Final Menu Screen - Customer-facing luxury menu display

 Menu Management
Add New Dishes with name, description, price, and course categorization
7 Pre-loaded Gourmet Items including starters, mains, and desserts
Course Organization - Starter, Main, Dessert categorization
Real-time Updates across all screens
Price Display in South African Rands (R)

 Design
Dark Theme with gold accents
Luxury Color Scheme with section-coded headers
Background Images with overlay effects
Professional Typography and spacing
Shadow Effects and smooth animations

 App Screens
Login Screen	Home Dashboard	Final Menu
Elegant welcome interface	Navigation hub with background image	Customer-facing luxury display

iOS Simulator or Android Emulator

Quick Start
Clone the repository
bash
cd christoffels-menu-manager

Install dependencies
bash
npm install
Install navigation dependencies

bash
npm install @react-navigation/native @react-navigation/stack react-native-screens react-native-safe-area-context
Run the application

bash
# For iOS
npx react-native run-ios

# For Android
npx react-native run-android

 Project Structure
text
christoffels-menu-manager/
├── App.tsx                          # Main navigation setup
├── screens/
│   ├── LoginScreen.tsx              # Welcome and login interface
│   ├── HomeScreen.tsx               # Main dashboard with navigation
│   ├── AddMenuScreen.tsx            # Dish addition and management
│   ├── MenuListScreen.tsx           # Staff menu overview
│   └── FinalMenuScreen.tsx          # Customer menu display
├── package.json
└── README.md

Usage Guide
For Restaurant Staff:
Login → Home → Add Menu to create new dishes
Menu List to view and manage all items
Real-time tracking of total menu items

For Customers:
GET DAMNED button from Home screen
Elegant menu display with categorized sections
Price visibility in South African Rands

Adding a New Dish:
Enter dish name and description
Set price in Rands
Select course type (Starter, Main, Dessert)
Automatic categorization in customer view

 Data Model
typescript
interface MenuItem {
  id: string;           // Unique identifier
  name: string;         // Dish name
  description: string;  // Detailed description
  price: number;        // Price in ZAR (R)
  course: string;       // 'Starter' | 'Main' | 'Dessert'
}
Pre-loaded Menu Items
The app comes with 7 gourmet dishes:
Starters
Oysters with Champagne Foam - R230
Wagyu Beef Carpaccio - R280
Pan-Seared Scallops - R190
Main Courses
Lobster Thermidor - R950
Truffle Wild Mushroom Risotto - R320
Desserts
Chocolate Lava Cake - R120
Berry Panna Cotta - R95

customization
Adding New Course Types
javascript
const courses = ['Starter', 'Main', 'Dessert', 'Drinks', 'Sides'];
Modifying Currency
javascript
// Change price display format
`R${item.price}` → `$${item.price}` or `€${item.price}`
Styling Updates
Edit the StyleSheet objects in each screen to customize:

Color schemes
Typography
Layout spacing
Background images

Acknowledgments
React Native community for excellent documentation

Restaurant professionals who provided design inspiration

Contributors and testers for valuable feedback
