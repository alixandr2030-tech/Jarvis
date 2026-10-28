# JARVIS AI — Android Starter

A minimal Kotlin Android Studio starter for an assistant prototype.

## Included
- Basic home screen
- In-app incoming-call-style screen with system ringtone
- A button that schedules one inexact reminder/check-in after 30 minutes
- Notification channel and tap-to-open behavior

## Not included yet
- Real AI model/API integration
- Speech-to-text or text-to-speech conversation
- True ongoing incoming-call UI while app is backgrounded
- Reliable recurring/random proactive conversations
- Phone-network calls

## Build
1. Install Android Studio with Android SDK 35.
2. Open this folder as a project.
3. Let Gradle sync.
4. Run on an Android device or emulator.

## Important Android limitations
- The scheduled reminder uses an inexact alarm and may be delayed by Doze/battery optimization.
- Android 13+ notification permission must be granted for normal notifications.
- Android may restrict background activity launches, full-screen notifications, and continuous background microphone access.
- The current call screen is launched from the app or notification. It is a prototype, not a telecom call.
- Do not put private API keys directly in the APK. A production AI API integration should use a secure backend or an appropriately designed key strategy.

## Suggested next steps
1. Add a backend endpoint for AI responses.
2. Add Android TextToSpeech for spoken replies.
3. Add speech recognition with clear microphone permission and user-visible controls.
4. Implement a proper foreground service only for user-visible ongoing sessions.
5. Add user-controlled check-in frequency, quiet hours, and a stop switch.
