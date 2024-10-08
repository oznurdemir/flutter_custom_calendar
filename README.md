<!--
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/tools/pub/writing-package-pages).

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/to/develop-packages).
-->


# flutter_custom_calendar

A Flutter package that provides a customizable calendar widget for your applications. 
This calendar allows users to select dates and navigate between months seamlessly, 
while also being fully customizable in terms of appearance.

<p align="center">
  <img src="https://github.com/user-attachments/assets/049461b2-568e-44fe-87fe-5c6ad37c6390" alt="Calendar Widget Screenshot" height="250"/>
</p>

Below is a short screen recording demonstrating how the calendar widget I created works:

https://github.com/user-attachments/assets/49c74eb9-59b7-4ddb-91ef-504aec1f93f7

This widget allows users to easily view and manage their events.

## Features

- **Customizable appearance**: Change the background color, selected day color, and text color.
- **Date selection**: Users can easily select a date by tapping on the desired day.
- **Month navigation**: Navigate between months using intuitive back and forward buttons.
- **Responsive design**: Adaptable to various screen sizes with a user-friendly layout.
- **Multiple language support**: The calendar widget supports different languages, allowing users to select their preferred language for a better experience.

## Getting started

1. Add `flutter_custom_calendar` as a dependency in your `pubspec.yaml` file:

   ```yaml
   dependencies:
     flutter_custom_calendar: ^0.0.1
   
2. Install the package:

   ```bash
   flutter pub get

3. Import the package in your Dart file:

   ```dart
   import 'package:flutter_custom_calendar/flutter_custom_calendar.dart';

## Usage

Here’s a simple example of how to use the `CustomCalendar` widget in your application:
   
      ```dart
      import 'package:flutter/material.dart';
      import 'package:flutter_custom_calendar/flutter_custom_calendar.dart';
   
       class MyApp extends StatelessWidget {
         @override
         Widget build(BuildContext context) {
           return MaterialApp(
             home: Scaffold(
               appBar: AppBar(
                 title: Text('Custom Calendar Example'),
               ),
               body: Center(
                 child: CustomCalendar(
                   selectedDate: DateTime.now(),
                   backgroundColor: Colors.white,
                   selectedDayColor: Colors.orange,
                   textColor: Colors.black,
                   onDateSelected: (DateTime date) {
                     print('Selected date: $date');
                   },
                 ),
               ),
             ),
           );
         }
       }
       
       void main() {
         runApp(MyApp());
       }

## Contributing

Contributions are welcome! If you would like to contribute to the flutter_custom_calendar, please follow these steps:

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes and commit them (git commit -m 'Add some feature').
4. Push to the branch (git push origin feature-branch).
5. Open a Pull Request.



