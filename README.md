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

# 🔐 Phase 1 – Authentication UI

## Student Login

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

## Student Registration

Implemented the Student Registration screen with:

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

## Organizer Login

Implemented the Organizer Login screen with:

- Organizer email field
- Password field
- Show/Hide password option
- Forgot password option
- Login button
- Google login option
- Organizer registration navigation
- Back to Student Login navigation
- Firebase email/password login
- Login success and error handling
- EventPulse branding
- Consistent off-white and sky-blue design

## Organizer Registration

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

# 🔥 Phase 2 – Firebase Backend & Authentication

Firebase has now been connected to the EventPulse Android application and is being used as the backend foundation for user authentication.

## Firebase Project Setup

Completed the initial Firebase backend integration:

- Firebase project created for **EventPulse**
- Firebase Android application registered
- Android package name configured as:
  `com.eventpulse.app`
- `google-services.json` added to the Android application
- Google Services Gradle plugin configured
- Firebase Android BoM integrated
- Firebase Authentication SDK added
- Firebase successfully connected with the Android application
- Internet permission configured in `AndroidManifest.xml`

## 📧 Email & Password Authentication

Email/password authentication has been successfully integrated.

### Student Authentication

- Student registration connected with Firebase Authentication
- Student login connected with Firebase Authentication
- Firebase user accounts are created successfully
- Registered users are visible in the Firebase Console
- Incorrect credentials are handled with user-friendly error messages
- Authentication success state is displayed in the application
- Forgot password functionality connected with Firebase Authentication

### Organizer Authentication

Organizer authentication has also been connected with Firebase.

- Organizer registration connected with Firebase Authentication
- Organizer login connected with Firebase Authentication
- Organizer accounts are created successfully
- Organizer users are visible in the Firebase Console
- Organizer login has been tested successfully
- Authentication success and error states are handled

## 🔑 Firebase Authentication Flow

```text
EventPulse Android App
        ↓
Firebase Authentication
        ↓
 ┌───────────────┐
 │               │
Student       Organizer
 │               │
 ↓               ↓
Login /        Login /
Register       Register
 │               │
 └───────┬───────┘
         ↓
   Firebase Users
