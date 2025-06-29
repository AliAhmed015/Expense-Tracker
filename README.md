<<<<<<< HEAD
# expense_tracker

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
=======
# Flutter Expense Tracker

A clean, intuitive expense tracking application built with Flutter that helps users manage their personal finances by tracking daily expenses and visualizing spending patterns through interactive charts and categorized transactions.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Screenshots](#screenshots)
- [Architecture](#architecture)
- [Getting Started](#getting-started)
- [Technical Requirements](#technical-requirements)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Flutter Expense Tracker is a cross-platform mobile application designed to simplify personal finance management. Built with Flutter's Material Design 3, it offers a responsive UI that adapts to different screen sizes and supports both light and dark themes. The app provides an intuitive interface for tracking expenses with visual charts and categorized spending analysis.

## Features

### Core Functionality
- **Add Expenses**: Quick expense entry with title, amount, date, and category
- **Delete & Undo**: Remove expenses with undo functionality via snackbar
- **Date Selection**: Built-in date picker for accurate expense tracking
- **Category Management**: Organize expenses into Food, Travel, Leisure, and Work categories

### Data Visualization
- **Interactive Charts**: Visual representation of spending patterns
- **Category Icons**: Intuitive icons for each expense category
- **Expense Summary**: Real-time calculation of total expenses per category

### User Experience
- **Responsive Design**: Adapts layout for tablets and phones
- **Material Design 3**: Modern UI following Google's latest design principles
- **Dark/Light Theme**: Automatic theme switching based on system preferences
- **Smooth Animations**: Fluid transitions and micro-interactions

### Technical Features
- **State Management**: Efficient state management using StatefulWidget
- **Form Validation**: Comprehensive input validation for all expense fields
- **Cross-Platform**: Single codebase for both Android and iOS
- **Memory Efficient**: Optimized performance with proper widget lifecycle management

## Architecture

The application follows a clean, modular architecture pattern:

```
lib/
├── main.dart                 # App entry point and theme configuration
├── models/
│   └── expense.dart         # Data models and enums
└── widgets/
    ├── expenses.dart        # Main expense management screen
    ├── new_expense.dart     # Add expense modal
    ├── chart/
    │   └── chart.dart       # Chart visualization widget
    └── expenses_list/
        └── expenses_list.dart # Expense list display widget
```

### Key Design Patterns
- **Widget Composition**: Modular widgets for reusability and maintainability
- **State Lifting**: Proper state management between parent and child widgets
- **Separation of Concerns**: Clear separation between UI, models, and business logic
- **Responsive Design**: Adaptive layouts using MediaQuery for different screen sizes

## Getting Started

### Prerequisites
- Flutter SDK (3.0.0 or higher)
- Dart SDK (2.17.0 or higher)
- Android Studio / VS Code with Flutter extensions
- iOS Simulator (for iOS development)
- Android Emulator or physical device

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/flutter-expense-tracker.git
   cd flutter-expense-tracker
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the application**
   ```bash
   # For development
   flutter run

   # For specific platform
   flutter run -d android
   flutter run -d ios
   ```

4. **Build for production**
   ```bash
   # Android APK
   flutter build apk --release

   # iOS (requires macOS and Xcode)
   flutter build ios --release
   ```

## Technical Requirements

### Dependencies
```yaml
dependencies:
  flutter:
    sdk: flutter
  uuid: ^3.0.7           # Unique ID generation
  intl: ^0.18.1          # Date formatting
  firebase_core: ^2.15.0 # Firebase integration
  firebase_crashlytics: ^3.3.4 # Crash reporting

dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^2.0.0
```

### Minimum Platform Versions
- **Android**: API level 21 (Android 5.0)
- **iOS**: iOS 11.0
- **Flutter**: 3.0.0+

## Project Structure

```
flutter_expense_tracker/
├── android/                 # Android-specific configuration
├── ios/                     # iOS-specific configuration
├── lib/
│   ├── main.dart           # Application entry point
│   ├── models/             # Data models
│   └── widgets/            # UI components
├── test/                   # Unit and widget tests
├── images/                 # Screenshots and assets
├── pubspec.yaml           # Project dependencies
└── README.md              # Project documentation
```

## Usage

### Adding an Expense
1. Tap the "+" button in the app bar
2. Fill in the expense details:
   - **Title**: Description of the expense
   - **Amount**: Cost in your local currency
   - **Date**: Select using the calendar picker
   - **Category**: Choose from Food, Travel, Leisure, or Work
3. Tap "Save Expense" to add it to your list

### Managing Expenses
- **View**: All expenses are displayed in a categorized list
- **Delete**: Swipe left on any expense or tap the delete icon
- **Undo**: Use the undo action in the snackbar to restore deleted expenses
- **Chart**: View your spending patterns in the visual chart at the top

### Responsive Features
- **Phone**: Vertical layout with chart above the expense list
- **Tablet**: Horizontal layout with chart and list side-by-side
- **Theme**: Automatically adapts to your device's light/dark theme preference

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
>>>>>>> 679c6e27e1fccead2f7676e6ac9d5810cdc739af
