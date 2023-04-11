# ZZZ Portal

## Getting Started

ZZZ Portal is a Flutter project for booking medical appointments and automatically tracking patient results.

It is an all-in-one healthcare app to book appointments with your doctors automatically, access your medical records anywhere, anytime, and receive constant medical advice and follow-up.


## Installation

**Step 1:**

Download or clone this repo by using the link below:

```
https://github.com/asleep-ai/zzz-portal-mobile-frontend
```

**Step 2:**

Go to project root and execute the following command in console to get the required dependencies:

```
flutter pub get 
```

Alternately, select Pub Get in the top right corner of the Visual Studio Code or Android Studio editors.

Then select virtual device or connect real device and execute the following command in console to run the project:

```
flutter run lib/main.dart
```
## Technologies used
* Flutter as cross platform framework
* Dart as a programming language
* Firebase for OTP generation as well as authentication and Push notification
* Provider package for state management
* DIO package for managing network requests## Features
* Cross-platform
* Splash Screen
* Introduction Screen
* Log in using your phone number and SSO ()
* Registration
* Verification
* Forget your password and reset password
* Home page with appointment view
* Book an appointment by selecting the clinic, doctor, and appointment date.
* Automatic and real-time appointment status update
* Checking in and questionnaire forms
* Appointment history view
* Lifestyle suggestions
* Profile views and updates
* State Management using Provider
* Validation
* Notifications
* Multilingual Support

## Folder Structure

### Flutter Structure
Here is the core folder structure which flutter provides.

```
flutter-app/
|- android
|- build
|- ios
|- lib
|- test
```

Here is the folder structure we have been using in this project

```
lib/
|- models/
|- providers/
|- routes/
|- services/
|- utils/
|- views/
|- main.dart
|- routes
```

Now, lets dive into the lib folder which has the main code for the application.

```
1- models - Models are just classes that help us determine the structure of the data, for example, API responses. JSON decoding and encoding for API responses and requests is done inside this section.

2- providers - This is where the state management implmented, to connect the reactive data of the application with the UI.

3- services — All API endpoints are called here by categories.

4- utils — Contains the utilities/common functions, styls and coloring of the application.

5- views — Contains all the ui of the project, contains sub directory for each screen.

6- routes — This one contains all the routes for the application.

7- main.dart - This is the starting point of the application. All the application level configurations are defined in this file i.e, theme, routes, title, orientation etc.
```

### Models

This directory contains all the models by category for each API end point.

```
model
|- appointment
|- clinic
|- doctor
|- exam
|- marketplace
|- profile
|- questionnaire
```

### providers

This directory contains all the states of the app by category.

```
providers
|- appointment
|- authentication
|- clinic
|- doctor
|- exam
|- marketplace
|- profile
|- questionnaire
|- setting

```

### utils

Contains the common file(s) and utilities used in a project. The folder structure is as follows: 

```
utils/
|- app_colors.dart
|- app_style.dart
|- basics.dart
|- language.dart
|- text_fonts.dart
|- validator.dart
```

### views

This directory contains all the ui of the application. Each screen is located in a separate folder making it easy to combine group of files related to that particular screen. Splash screen, Introduction screen and Authentication screens such as Sign in and Sign up are included inside the `Pre-login` directory. All the screen specific widgets and common widgets such as buttons, text fields are placed in `custome_widgets` directory as shown in the example below:

```
views/
|- custome_widgets/
|- Pre-login
|- Home
|- History
|- Lifestyle
|- MyAccount
```

## Used By

This project is used by the following companies:

- Asleep

