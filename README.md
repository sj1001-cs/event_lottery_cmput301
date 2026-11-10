# event_lottery_cmput301
# Linko: Event Lottery App

Linko is an Android app for running event sign-ups as a lottery. Entrants join an event's waiting list, the organizer draws winners at random, and the people who get picked can accept or decline their spot. If someone declines, the organizer can draw a replacement.

This was a team project for CMPUT 301 (Fall 2025) at the University of Alberta. The original course repo is `CMPUT301F25virtue1/virtue1-events`. This is a copy of it on my own account.

![Linko logo](doc/img/LinkoLogoAnimation.gif)

## What it does

**For entrants**
- Sign up with a profile and edit or delete it later
- Browse and search events, and filter them
- Join or leave an event's waiting list
- Scan an event's QR code to open it
- Get notified when selected, and accept or decline the invitation
- See your event history

**For organizers**
- Create and edit events, including the poster image
- Generate a QR code for each event
- Run the lottery draw and see the list of entrants
- See where entrants signed up from on a map
- Send notifications to entrants

**For admins**
- Browse and remove events, profiles and uploaded images

## Built with

- Java, Android Studio, Gradle
- Firebase Firestore (data) and Firebase Storage (images)
- Google Maps and Location services
- ZXing for QR codes
- JUnit and Espresso for tests

## Running it

1. Clone the repo and open it in Android Studio.
2. Let Gradle sync, then pick an emulator (API 24 or newer) or a phone.
3. Press Run.

The app talks to the team's Firebase project through `app/google-services.json`, so it should run as is. If you want to use your own Firebase project, replace that file with your own and add your own Google Maps key in `AndroidManifest.xml`.

## Design

The storyboards and mockups from our planning are in `doc/img`, and the generated Javadoc is in `doc`.

![Storyboard](doc/img/StoryboardMockup.png)

