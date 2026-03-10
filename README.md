Flutter Todo App Herody

A clean, modern Todo application built with Flutter, demonstrating Firebase integration, state management with Riverpod, and clean architecture principles.

Features

✅ Firebase Authentication (Email & Password)

✅ Firebase Realtime Database for storing tasks

✅ State management using Riverpod

✅ Add, update, and delete tasks

✅ Mark tasks as completed

✅ Responsive and clean UI design

  ***Tech Stack

1. Flutter – Cross-platform mobile framework

2. Firebase Authentication – User login and registration

3. Firebase Realtime Database – Store and sync tasks in real-time

4. Riverpod – Reactive state management

** Project Structure**
lib/
├── core/
│   └── constants/        # App constants and configurations
├── application/
│   └── providers/        # State management with Riverpod
├── domain/
│   └── models/           # Data models
├── infrastructure/
│   └── services/         # Firebase and external services
└── presentation/
    ├── screens/          # UI Screens
    └── widgets/          # Reusable UI components

This structure follows clean architecture principles:

Domain → Core business logic and data models

Application → State management and providers

Infrastructure → External services (Firebase)

Presentation → UI layer (screens and widgets)

** Getting Started **
1. Clone the repository
git clone <repository-url>
cd flutter-todo-app
2. Install dependencies
flutter pub get
3. Configure Firebase

Go to Firebase Console
 and create a new project.

Add an Android and/or iOS app to the project.

Download the configuration files:

google-services.json → Android (android/app/)

GoogleService-Info.plist → iOS (ios/Runner/)

4. Run the app
flutter run
Usage

Register or log in with your email and password.

Add new tasks in the input field and tap the Add button.

Mark tasks as completed using the checkbox.

Delete tasks using the trash icon.

Purpose

This project was developed to demonstrate:

Firebase integration with Flutter

State management using Riverpod

Clean architecture in mobile app development

CRUD operations in a Todo application

