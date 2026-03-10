# flutter-firebase-todo

A Flutter To-Do List App with **Firebase Authentication** and **Firebase Realtime Database**. Users can sign up or log in securely, create and manage tasks (add, edit, delete, mark as completed), with **real-time updates** and **efficient state management** using Riverpod. The app features a clean, responsive UI.

---

## Features

- Firebase Authentication (Email & Password)
- Firebase Realtime Database
- Add, Edit, Delete Tasks
- Mark Tasks as Completed
- Real-time Updates
- Riverpod State Management
- Clean Architecture & Responsive UI

---

## Tech Stack

- Flutter
- Firebase (Authentication & Realtime Database)
- Riverpod (State Management)

2️⃣ Install Dependencies
flutter pub get


3️⃣ Setup Firebase
a. Create Firebase Project

1. Go to Firebase Console

2. Click Add project and follow the steps.

b. Add Android App

1 .Click Add App → Android

2. Enter your package name (e.g., com.example.flutter_firebase_todo)

3. Download google-services.json

4. Place it in your Flutter project at:

5. android/app/google-services.json

   
c. Add iOS App (Optional)

1. Click Add App → iOS

2. Enter your iOS bundle ID

3. Download GoogleService-Info.plist

4. Place it in your Flutter project at:

5. ios/Runner/GoogleService-Info.plist
   
d. Enable Firebase Authentication

1. Go to Authentication → Sign-in method

2. Enable Email/Password

e. Enable Realtime Database

1. Go to Realtime Database → Create Database
2.Set rules (for testing):

{
  "rules": {
    ".read": "auth != null",
    ".write": "auth != null"
  }
}

4️⃣ Run the App
a. On Emulator / Device
flutter run

b. Build APK (for Android)
flutter build apk --release

APK will be available at:

build/app/outputs/flutter-apk/app-release.apk


Troubleshooting

Firebase not initialized error → Make sure firebase_core is initialized in main.dart:

void main() async {
  WidgetsFlutterBinding.ensureInitialized();
  await Firebase.initializeApp();
  runApp(MyApp());
}

Network / Internet issues → Make sure your emulator/device is connected.

Packages not found → Run flutter pub get again.

*** Folder / File Highlights

1. main.dart → App entry point

2. application/providers/ → Riverpod state management

3. domain/models/task_model.dart → Task data structure

4. infrastructure/firebase/ → Firebase CRUD operations

5. presentation/screens/ → UI screens (Login, Signup, Tasks)

6. presentation/widgets/ → Reusable widgets like buttons, task cards
Set rules (for testing):
## Project Structure
