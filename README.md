<!--
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages).

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages).
-->

The Flutter Social Login Buttons package provides a set of easy-to-use and customizable buttons for integrating social login functionality into your Flutter applications. With this package, you can allow users to log in or sign up using their existing social media accounts such as Google, Facebook, Twitter, and GitHub etc.

## Features

- Ready-to-use buttons for Google, Facebook, Twitter, and GitHub login.
- Easily customizable to match your app's design and theme.
- Seamless integration with popular authentication providers.

## Installation

To use this package, add it to your pubspec.yaml file:

```yaml
dependencies:
  social_login_buttons_plugin: ^1.0.0
```

Then, run flutter pub get to install the package.

## Usage

Import the package in your Dart code:

```dart
import 'package:social_login_buttons_plugin/social_login_buttons_plugin.dart';
```

Add the SignInButton to your UI:

```dart
Column(
  mainAxisAlignment: MainAxisAlignment.center,
  children: [
    SignInButton(
      Buttons.Google,
      onPressed: () => _handleGoogleSignIn(),
      text: 'Sign in with Google',
      shape: RoundedRectangleBorder(borderRadius: BorderRadius.circular(8.0)),
    ),
    SignInButton(
      Buttons.Facebook,
      onPressed: () => _handleFacebookSignIn(),
      text: 'Sign in with Facebook',
      shape: RoundedRectangleBorder(borderRadius: BorderRadius.circular(8.0)),
    ),
    // Add more social login buttons as needed
  ],
),
```

## Contributions

Contributions to this package are welcome! If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request on GitHub.
