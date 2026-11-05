# EventPulse

EventPulse is a modern Android application designed to help students
discover, explore, and participate in events happening across their
college campus.

The project is being developed using **Kotlin** and **Jetpack Compose**,
with a modern, attractive, and student-friendly interface.

------------------------------------------------------------------------

## 🚀 Project Progress

### Phase 0 -- Project Setup

-   Project created in Android Studio
-   Project name: **EventPulse**
-   Application ID: `com.eventpulse.app`
-   Kotlin selected as the development language
-   Jetpack Compose and Material 3 used for UI development
-   Off-white and sky-blue theme selected
-   EventPulse branding and logo finalized

------------------------------------------------------------------------

## 🔐 Phase 1 -- Authentication UI

### Student Login

Implemented student email/password login UI, Google login option, forgot
password, student registration navigation, organizer login navigation,
password show/hide, animations, and EventPulse branding.

### Student Registration

Implemented full name, student email, student ID, password, confirm
password, validation UI, account creation, Google signup option,
back/login navigation, and a scrollable registration form.

### Organizer Login

Implemented organizer email/password login UI, Google login option,
forgot password, organizer registration navigation, back navigation,
password show/hide, and EventPulse branding.

### Organizer Registration

Implemented organization name, organizer name, organizer email, phone
number, organization type, password, confirm password, account creation,
Google signup option, back/login navigation, and a scrollable
registration form.

------------------------------------------------------------------------

# 🔥 Phase 2 -- Firebase Backend & Authentication

Firebase has been integrated into EventPulse as the backend foundation
for authentication and future application features.

### Firebase Setup

-   Firebase project created for EventPulse
-   Android application registered with Firebase
-   Package name configured as `com.eventpulse.app`
-   `google-services.json` added to the Android app
-   Google Services Gradle plugin configured
-   Firebase Android BoM integrated
-   Firebase Authentication SDK integrated

### Email & Password Authentication

Student and organizer authentication flows are connected with Firebase
Authentication.

Implemented:

-   Student account creation
-   Student email/password login
-   Organizer account creation
-   Organizer email/password login
-   Firebase user account creation
-   Firebase login verification
-   Login loading state
-   Authentication error handling
-   Forgot password flow
-   Firebase Console user management

Current architecture:

``` text
EventPulse Android App
          ↓
Firebase Authentication
          ↓
     User Accounts
          ↓
   Firebase Console
```

### Current Authentication Flow

``` text
App Launch
    ↓
Student Login
    ├── Student Registration
    │       ↓
    │   Firebase Account
    │
    ├── Student Login
    │       ↓
    │   Firebase Authentication
    │       ↓
    │   Student Home
    │
    └── Organizer Login
            ↓
       Organizer Registration
            ↓
       Firebase Account
```

Google Sign-In configuration has also been started and is planned for
the complete authentication flow.

------------------------------------------------------------------------

# 🏠 Phase 3 -- Student Home / Dashboard UI

The initial Student Home screen has been implemented after
authentication.

### Current Student Home Features

-   Personalized greeting using the logged-in student's name
-   Modern EventPulse dashboard
-   Off-white and sky-blue visual language
-   Animated/light background decorative circles
-   Compact animated search interaction
-   Featured event section
-   Live events section
-   Event cards
-   Event dates and locations
-   Event categories
-   Category filtering UI
-   Upcoming events
-   Clubs section
-   Communities section
-   Hobbies section
-   Event memories / previous events section
-   Bottom navigation
-   Home navigation
-   Explore navigation
-   My Events navigation
-   Clubs navigation
-   Profile navigation
-   Floating chatbot button placeholder

### Student Home Navigation

``` text
Student Home
│
├── Home
├── Explore
├── My Events
├── Clubs
└── Profile
```

------------------------------------------------------------------------

## 🔎 Search Experience

The home screen uses a compact search interaction instead of keeping a
large search field permanently visible.

``` text
Search Icon
     ↓
Animated Search Bar
     ↓
Enter Event / Club / Community
     ↓
Search / Filter Results
```

The search architecture will later be connected to the real Firebase
event database.

------------------------------------------------------------------------

# 🤖 AI Assistant -- Planned

An AI-powered EventPulse assistant has been planned but is **not yet
implemented**.

The planned assistant will eventually support:

-   Voice interaction
-   "Hey Bot" style activation
-   Current event queries
-   Upcoming event queries
-   Natural-language event search
-   My Events queries
-   Event recommendations
-   Event registration commands
-   App navigation commands
-   Personalized campus event suggestions
-   Text-to-speech responses

Planned architecture:

``` text
User Voice
    ↓
Speech Recognition
    ↓
AI Assistant
    ↓
EventPulse Functions
    ↓
Firebase / Event Database
    ↓
AI Response
    ↓
Text-to-Speech
```

AI development will start after the core event database and
event-management functionality are completed.

------------------------------------------------------------------------

# 🎨 Design System

EventPulse currently follows a consistent visual design:

-   Off-white background
-   Sky-blue primary color
-   Dark navy text
-   Rounded cards and buttons
-   Soft shadows
-   Minimal modern layouts
-   Smooth animations
-   Student-focused interface
-   Consistent EventPulse branding

The same design language will be maintained across Student, Organizer,
Event, Profile, and other screens.

------------------------------------------------------------------------

# 🛠️ Technology Stack

-   **Kotlin**
-   **Android Studio**
-   **Jetpack Compose**
-   **Material 3**
-   **Android SDK**
-   **Gradle**
-   **Firebase**
-   **Firebase Authentication**

Planned technologies for later phases may include Firebase Firestore,
Firebase Storage, AI services, speech recognition, and text-to-speech.

------------------------------------------------------------------------

# 📱 Current Application Flow

``` text
                    EventPulse
                        ↓
                 Student Login
                        ↓
        ┌───────────────┴────────────────┐
        ↓                                ↓
Student Registration               Organizer Login
        ↓                                ↓
Firebase Account              Organizer Registration
        ↓                                ↓
        └───────────────┬────────────────┘
                        ↓
                 Authentication
                        ↓
                 Student Home
                        ↓
        ┌───────────────┼────────────────┐
        ↓               ↓                ↓
      Explore        My Events          Clubs
                        ↓
                     Profile
```

------------------------------------------------------------------------

# 🔮 Upcoming Development

### Core Event System

-   Firebase Firestore event database
-   Organizer event creation
-   Event editing
-   Event deletion
-   Event approval/management
-   Event details screen
-   Student event registration
-   My Events
-   Saved events
-   Event categories
-   Search and filters
-   Club management
-   Notifications

### Organizer Dashboard

-   Organizer dashboard
-   Create event
-   Manage events
-   View registrations
-   Event analytics
-   Organization profile

### AI Integration

After the core event system is functional:

-   AI text assistant
-   Voice assistant
-   Natural-language event search
-   Event recommendations
-   AI-powered event registration
-   "Hey Bot" style interaction

------------------------------------------------------------------------

# 📂 Current Project Structure

``` text
com.eventpulse.app
│
├── MainActivity.kt
│
└── ui
    ├── screens
    │   ├── login
    │   │   ├── StudentLoginScreen.kt
    │   │   ├── StudentRegistrationScreen.kt
    │   │   ├── OrganizerLoginScreen.kt
    │   │   └── OrganizerRegistrationScreen.kt
    │   │
    │   └── home
    │       └── StudentHomeScreen.kt
    │
    └── theme
        ├── Color.kt
        ├── Theme.kt
        └── Type.kt
```

------------------------------------------------------------------------

# 📌 Current Status

  Phase                                          Status
  ---------------------------------------------- ----------------
  Phase 0 -- Project Setup                       ✅ Completed
  Phase 1 -- Authentication UI                   ✅ Completed
  Phase 2 -- Firebase Backend & Authentication   ✅ Completed
  Phase 3 -- Student Home / Dashboard UI         🚧 In Progress
  Core Event Management                          ⏳ Upcoming
  Organizer Dashboard                            ⏳ Upcoming
  AI Assistant                                   ⏳ Planned

------------------------------------------------------------------------

# 🎯 Project Goal

EventPulse aims to provide a centralized campus platform where students
can:

-   Discover events
-   Explore clubs and communities
-   Search campus activities
-   Register for events
-   Manage their events
-   Receive notifications
-   Get personalized recommendations
-   Interact with an AI-powered campus assistant

The long-term goal is to make EventPulse a complete **campus event
discovery and management platform**.
