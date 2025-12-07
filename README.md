# Permacia 🏥

[![Android](https://img.shields.io/badge/Platform-Android-green.svg)](https://developer.android.com/)
[![Kotlin](https://img.shields.io/badge/Language-Kotlin-blue.svg)](https://kotlinlang.org/)
[![Firebase](https://img.shields.io/badge/Backend-Firebase-orange.svg)](https://firebase.google.com/)

**Permacia** is a 24/7 pharmacy companion Android application that helps users locate nearby pharmacies, save their favorite pharmacies, and manage their profile with ease.

## 📱 Features

- **Pharmacy Locator**: Find pharmacies near your location using Google Maps integration
- **User Authentication**: Secure login and account creation with Firebase Authentication
- **Google Sign-In**: Quick and easy sign-in with your Google account
- **Favorite Pharmacies**: Save and manage your favorite pharmacies for quick access
- **User Profile**: View and manage your personal profile information
- **Location Services**: Real-time location tracking to find the nearest pharmacies
- **Interactive Maps**: Visual representation of pharmacy locations with Google Maps
- **Modern UI**: Clean and intuitive user interface with Material Design

## 📸 Screenshots

| Main Screen | Login | Home | Pharmacy List |
|-------------|-------|------|---------------|
| ![Main Screen](https://raw.githubusercontent.com/Waa-Ihaab/Application_Android_Kt/main/screens/Screenshot_20251204_040211.png) | ![Login](https://raw.githubusercontent.com/Waa-Ihaab/Application_Android_Kt/main/screens/Screenshot_20251204_040219.png) | ![Home](https://raw.githubusercontent.com/Waa-Ihaab/Application_Android_Kt/main/screens/Screenshot_20251204_040052.png) | ![Pharmacy List](https://raw.githubusercontent.com/Waa-Ihaab/Application_Android_Kt/main/screens/Screenshot_20251204_040144.png) |

| Pharmacy Details | Favorites | Profile |
|------------------|-----------|---------|
| ![Pharmacy Details](https://raw.githubusercontent.com/Waa-Ihaab/Application_Android_Kt/main/screens/Screenshot_20251204_040203.png) | ![Favorites](https://raw.githubusercontent.com/Waa-Ihaab/Application_Android_Kt/main/screens/Screenshot_20251204_041437.png) | ![Profile](https://raw.githubusercontent.com/Waa-Ihaab/Application_Android_Kt/main/screens/Screenshot_20251204_040114.png) |

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Waa-Ihaab/Application_Android_Kt.git
cd Application_Android_Kt
```

### 2. Set Up Firebase

1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a new project or use an existing one
3. Add an Android app to your Firebase project
4. Register your app with package name: `com.example.myapplication`
5. Download the `google-services.json` file
6. Place the `google-services.json` file in the `app/` directory

### 3. Configure Google Maps API

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select an existing one
3. Enable the **Maps SDK for Android**
4. Create an API key for Maps
5. Update the API key in `app/src/main/AndroidManifest.xml`:

```xml
<meta-data
    android:name="com.google.android.geo.API_KEY"
    android:value="YOUR_GOOGLE_MAPS_API_KEY"/>
```

⚠️ **Important**: Never commit your API keys to version control. Consider using local.properties or environment variables.

### 4. Configure Google Sign-In

1. In Firebase Console, enable Google Sign-In under Authentication
2. Download and update `google-services.json` if needed
3. The OAuth 2.0 Client ID should be automatically configured

### 5. Open in Android Studio

1. Open Android Studio
2. Select **File > Open**
3. Navigate to the cloned repository
4. Wait for Gradle sync to complete

## 📖 How to Use

### First Time Setup

1. **Launch the App**: Open Permacia on your Android device
2. **Create an Account**: 
   - Tap on "Create Account" on the main screen
   - Enter your email and password
   - Or use "Sign in with Google" for quick access
3. **Grant Permissions**: Allow location access when prompted for finding nearby pharmacies

### Finding Pharmacies

1. **Home Screen**: After logging in, you'll see the home screen with pharmacy options
2. **View All Pharmacies**: Tap "All Pharmacies" to see a list of available pharmacies
3. **Use Maps**: The map view shows pharmacies near your current location
4. **Tap on a Pharmacy**: Get detailed information about a specific pharmacy

### Managing Favorites

1. **Add to Favorites**: While viewing a pharmacy, tap the favorite/heart icon
2. **View Favorites**: Access "My Favorites" from the menu to see all saved pharmacies
3. **Remove from Favorites**: Tap the favorite icon again to remove

### Profile Management

1. **Access Profile**: Tap on the profile icon in the navigation
2. **View Information**: See your account details
3. **Update Profile**: Modify your personal information as needed
4. **Sign Out**: Use the sign-out option when you want to log out

## 📁 Project Structure

```
Application_Android_Kt/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/myapplication/
│   │   │   │   ├── MainActivity.kt
│   │   │   │   ├── Login.kt
│   │   │   │   ├── Creatacc.kt
│   │   │   │   ├── Pagehome.kt
│   │   │   │   ├── PharmacyPage.kt
│   │   │   │   ├── AllPharmacia.kt
│   │   │   │   ├── Fvpharmacie.kt
│   │   │   │   └── Monprofile.kt
│   │   │   ├── res/
│   │   │   │   ├── layout/         # XML layouts
│   │   │   │   ├── drawable/       # Images and icons
│   │   │   │   ├── values/         # Strings, colors, themes
│   │   │   │   └── font/           # Custom fonts
│   │   │   └── AndroidManifest.xml
│   │   ├── androidTest/            # Instrumented tests
│   │   └── test/                   # Unit tests
│   ├── build.gradle.kts
│   └── google-services.json        # Firebase configuration
├── gradle/
├── build.gradle.kts
├── settings.gradle.kts
└── README.md
```

## ⚙️ Configuration

### Minimum Requirements
- **Min SDK**: 28 (Android 9.0 Pie)
- **Target SDK**: 34 (Android 14)
- **Compile SDK**: 36

### Build Configuration
- **Java Version**: 11
- **Kotlin JVM Target**: 11

## 🤝 Contributing

Contributions are welcome! If you'd like to contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📞 Contact Me

If you have any questions about using the application or need assistance, feel free to reach out:

- **GitHub**: [@Waa-Ihaab](https://github.com/Waa-Ihaab)
- **Email**: contact.kariihab@gmail.com
- **Project Link**: [https://github.com/Waa-Ihaab/Application_Android_Kt](https://github.com/Waa-Ihaab/Application_Android_Kt)

### Support

For bug reports and feature requests, please use the [GitHub Issues](https://github.com/Waa-Ihaab/Application_Android_Kt/issues) page.

## 📝 License

This project is available for educational and personal use. Please contact the repository owner for commercial use inquiries.

## 🙏 Acknowledgments

- Firebase for backend services
- Google Maps Platform for location services
- Material Design for UI components
- All open-source contributors

---

**Made with ❤️ for making pharmacy access easier**
