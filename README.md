# level_rendering

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.



Dynamic Modules Project
Approach

This project dynamically fetches modules and their associated cakes from Firebase Firestore and displays them in a user-friendly Flutter application. It utilizes the Provider package for state management to ensure seamless UI updates when data changes. Firebase is integrated for backend data management, enabling real-time updates and scalability.
Key Features:

    Dynamic Rendering: Modules are loaded dynamically from Firestore, and the UI updates automatically.
    State Management: Provider ensures efficient data flow and UI state updates.
    Firebase Integration: Firestore provides a robust and scalable backend.

Assumptions

    Firestore Structure: The database is structured with a modules collection where each document contains:
        name (String): The module name.
        cakes (List): A list of associated cakes.
    Firestore Rules: During development, Firestore rules are set to allow unrestricted access for testing purposes.
    Testing Environment: The app runs on an Android or iOS emulator/device with proper Firebase configuration.

Instructions for Running the Project Locally
Prerequisites:

    Flutter SDK: Ensure Flutter is installed (Download Flutter).
    Firebase Setup:
        Create a Firebase project and enable Firestore.
        Download the google-services.json file for Android or GoogleService-Info.plist for iOS and place it in the respective directories:
            Android: android/app/google-services.json

Steps to Run:

    Clone the Repository:

git clone <repository-url>
cd <repository-folder>

Install Dependencies:

flutter pub get

Run Firebase CLI Configuration:

    Ensure the Firebase CLI is installed. If not, install it (Firebase CLI).
    Authenticate Firebase:

firebase login

Set up the Firebase project:

    flutterfire configure

Run the App:

flutter run
