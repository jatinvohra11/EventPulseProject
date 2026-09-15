# EventPulse

EventPulse is a modern Android application designed to help students discover, explore, and participate in events happening across their college campus.

The project is being developed as an Android application using **Kotlin** and **Jetpack Compose**, with a focus on a modern, attractive, and user-friendly experience.

---

## 🚀 Current Progress

### Phase 0 – Project Setup

- Project created in Android Studio
- Project name: **EventPulse**
- Application ID: `com.eventpulse.app`
- Kotlin selected as the development language
- Jetpack Compose used for UI development
- Initial project structure created
- Off-white and sky-blue color theme selected for the complete application
- EventPulse logo and branding finalized

---

## 🔐 Phase 1 – Authentication UI

### Student Login

Implemented the initial Student Login screen with:

- Student email field
- Password field
- Show/Hide password option
- Login button
- Google login option
- Student registration navigation
- Organizer login navigation
- Forgot password option
- Modern off-white and sky-blue UI
- Rounded input fields and buttons
- Smooth entrance animations
- EventPulse branding animation
- Typing animation for the EventPulse app name

### Student Registration

Implemented the initial Student Registration screen with:

- Full name field
- Student email field
- Student ID field
- Password field
- Confirm password field
- Show/Hide password option
- Password validation UI
- Create Student Account button
- Google registration option
- Back to Login navigation
- Smooth screen entrance animations
- EventPulse branding
- Off-white and sky-blue theme
- Scrollable registration form

### Organizer Login

Implemented the Organizer Login screen with:

- Organizer email field
- Password field
- Show/Hide password option
- Forgot password option
- Login button
- Google login option
- Organizer registration navigation
- Back to Student Login navigation
- EventPulse branding
- Consistent off-white and sky-blue design

### Organizer Registration

Implemented the Organizer Registration screen with:

- Organization name field
- Organizer name field
- Organizer email field
- Phone number field
- Organization type field
- Password field
- Confirm password field
- Show/Hide password option
- Create Organizer Account button
- Google registration option
- Back to Organizer Login navigation
- Scrollable registration form
- EventPulse branding
- Consistent off-white and sky-blue design

---

## 🔥 Phase 2 – Firebase Backend & Authentication

Firebase has been integrated into the EventPulse Android application as the backend foundation for authentication and future application features.

### Firebase Project Setup

- Firebase project created for **EventPulse**
- Firebase Android application registered
- Android package name configured as:
  `com.eventpulse.app`
- Firebase configuration file `google-services.json` added to the Android app
- Google Services Gradle plugin configured
- Firebase Android BoM integrated
- Firebase Authentication SDK added
- Firebase connected with the EventPulse Android application

### Email & Password Authentication

- Email/Password authentication enabled in Firebase
- Firebase Authentication connected with the Student Login screen
- Firebase user accounts can be managed through the Firebase Console
- Student authentication flow prepared using Firebase Authentication
- Password reset functionality connected with Firebase Authentication

### Google Authentication

- Google Sign-In provider enabled in Firebase
- Google authentication configuration initiated
- Google Sign-In integration planned for the authentication flow

### Firebase Authentication Structure

```text
EventPulse Android App
        ↓
Firebase Authentication
        ↓
   User Accounts
        ↓
Firebase Console
```

🎨 Design Theme

The current application uses a consistent:

Off-White background
Sky Blue primary color
Clean and modern UI
Rounded components
Minimal design
Smooth animations
Student-focused visual style
Consistent EventPulse branding

The same design language will be maintained throughout the application.

🛠️ Technology Stack
Kotlin
Android Studio
Jetpack Compose
Material 3
Android SDK
Gradle
Firebase
Firebase Authentication
📱 Current Application Flow
App Launch
    ↓
Student Login
    ↓
    ├── Email & Password Login
    │          ↓
    │    Firebase Authentication
    │
    ├── Continue with Google
    │
    ├── Forgot Password
    │
    ├── Create Student Account
    │          ↓
    │    Student Registration
    │          ↓
    │    Firebase Account
    │
    └── Organizer Login
               ↓
        Organizer Login
               ↓
        Organizer Registration
