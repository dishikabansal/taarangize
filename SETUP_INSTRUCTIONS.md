# Project Setup Instructions

## Steps to Create the Project in Android Studio

1. Open Android Studio
2. Click on "Create New Project"
3. Select "Empty Activity" template
4. Configure your project with these settings:
   - Name: FestOrganizer
   - Package name: com.your.college.festorganizer (replace with your college name)
   - Save location: Choose the FestOrganizer directory you created
   - Language: Kotlin
   - Minimum SDK: API 24 (Android 7.0) or higher
   - Target SDK: Latest stable (API 34)
   - Build System: Gradle

5. Click "Finish" to create the project

## Add Required Dependencies

Add these dependencies to your app's build.gradle file:

```gradle
// Firebase core, auth, firestore, and cloud messaging
implementation platform('com.google.firebase:firebase-bom:32.7.0')
implementation 'com.google.firebase:firebase-analytics-ktx'
implementation 'com.google.firebase:firebase-auth-ktx'
implementation 'com.google.firebase:firebase-firestore-ktx'
implementation 'com.google.firebase:firebase-messaging-ktx'

// Material Design components
implementation 'com.google.android.material:material:1.9.0'

// Android Jetpack
implementation 'androidx.core:core-ktx:1.12.0'
implementation 'androidx.appcompat:appcompat:1.6.1'
implementation 'androidx.constraintlayout:constraintlayout:2.1.4'
implementation 'androidx.lifecycle:lifecycle-viewmodel-ktx:2.6.2'
implementation 'androidx.lifecycle:lifecycle-livedata-ktx:2.6.2'
implementation 'androidx.navigation:navigation-fragment-ktx:2.7.5'
implementation 'androidx.navigation:navigation-ui-ktx:2.7.5'

// Calendar view
implementation 'com.github.kizitonwose:CalendarView:1.0.4'

// Image loading
implementation 'com.github.bumptech.glide:glide:4.15.1'
annotationProcessor 'com.github.bumptech.glide:compiler:4.15.1'
```

## Firebase Setup

1. Go to the [Firebase Console](https://console.firebase.google.com/)
2. Create a new project
3. Add an Android app to your Firebase project
   - Use the same package name as your Android project
   - Download the `google-services.json` file
   - Place it in the app directory of your Android project

4. In your project-level build.gradle, add:
```gradle
buildscript {
    dependencies {
        classpath 'com.google.gms:google-services:4.4.0'
    }
}
```

5. In your app-level build.gradle, add:
```gradle
apply plugin: 'com.google.gms.google-services'
```

6. Enable Authentication, Firestore, and Cloud Messaging in the Firebase Console 

## Additional Steps

1. **Open your project-level build.gradle file**:
   - In Android Studio, navigate to Project view
   - Expand Gradle Scripts
   - Open `build.gradle (Project: FestOrganizer)`

2. **Add JitPack repository**:
   - Add the following line to the `repositories` block:
   ```gradle
   repositories {
       google()
       mavenCentral()
       maven { url 'https://jitpack.io' }
   }
   ```

3. **Sync Project**:
   - Click "Sync Now" when prompted, or manually sync by clicking the "Sync Project with Gradle Files" button in the toolbar

Once you've added these dependencies, your project will be ready for Firebase integration and implementing the app features. 

plugins {
    id 'com.android.application'
    id 'org.jetbrains.kotlin.android'
    id 'com.google.gms.google-services'
} 