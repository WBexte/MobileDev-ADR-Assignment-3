# Using React Native for UI Framework

## Status

The status for this AD is *accepted*

## Context

The team needs to design an interactive social networking and schedule app for students and professors. The app must provide a messaging feature and have the ability for students to share information, view and manage their schedule and see clubs or upcoming events on campus.

Some front-end requirements include:
- Support for cross-platform
- Offline support
- Push notification support
- Data security
- Accessibility features

## Decision

For the UI and frontend framework we will employ React Native and Tailwind CSS for styling. React Native is a popular mobile-development framework that allows for responsive design and will work well for a chat and scheduling application. It will also allow the team to produce a hybrid app that will function on both iOS and Android.

1. **Support for cross-platform:**
	React native provides an efficient framework for designing a cross-platform app for iOS and Android devices.

2. **Offline Support:**
	we can employ *Redux Offline* to implement offline support and local data storage

3. **Push Notification Support:**
	React native provides support for push notification services. We can use *OneSignal* as the push notification service which supports both iOS and Android notifications.

4. **Data Security:**
	React Native provides support for encrypted data transfer which will improve data security. However, data security will mainly be handled by the backend.

5. **Accessibility Features:**
	React Native has built-in accessibility APIs which we can leverage to provide text-to-speech, high contrast mode and other features.

## Consequences

1. Multi-platform support
	- React Native allows multiplatform development which will allow shared code across iOS and Android which will reduce the required code.
	- React Native is not as compatible with web apps which may mean more code is required if we wanted to expand to a web app
2. Tailwind CSS
	- Tailwind is an easy framework to provide styling to websites or mobile apps.
3. Push notifications
	- OneSignal provides support for both push notifications and in-app messages, creating an interactive experience for the user.
	- OneSignal only supports mobile devices, which means if we expanded to a web app, we would need to use a different provider for in-app messages.
4. Accessibility
	- React Native comes with a built-in accessibility API which will make integration incredibly easy
