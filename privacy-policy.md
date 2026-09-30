# UnScroll Privacy Policy

**Effective date:** September 30, 2026

This Privacy Policy explains how **UnScroll** (package `com.otvmrnslv.unscroll`, "the App") handles information. The App is developed by **Almost Done Studios** ("we", "us").

UnScroll helps you limit time spent in apps you choose. It is designed to work almost entirely on your device: it has no user accounts, no ads, and no servers of its own.

---

## 1. Summary

- UnScroll uses Android's **Accessibility Service** and **Usage Access** only to detect when an app you selected (or the YouTube Shorts feed) is open in the foreground, so it can enforce the time limits you set.
- UnScroll **does not** read, record, or transmit your messages, text input, passwords, browsing history, or screen contents.
- Your settings and block history are stored **only on your device**.
- The App uses **Google Firebase** (Analytics, Crashlytics, Performance Monitoring) to collect limited, pseudonymous usage, crash, and performance data so we can improve stability.
- We do **not** sell your data or use it for advertising.

---

## 2. Permissions and why they are used

| Permission | Why UnScroll needs it |
|---|---|
| **Accessibility Service** | To detect which app is currently in the foreground and, for YouTube, whether the "Shorts" tab is the one selected. The App only inspects the on-screen interface to find that tab indicator. It does not read or store any other screen content, and it can perform a "Home" action to close a monitored app when you choose *Close app*. |
| **Usage Access** (`PACKAGE_USAGE_STATS`) | To list the apps installed on your device so you can choose which ones to monitor. |
| **Display over other apps** (`SYSTEM_ALERT_WINDOW`) | To show the blocker screen on top of a monitored app when your time limit is reached. |
| **Notifications** (`POST_NOTIFICATIONS`) | To show the countdown timer notification, alert you if the monitoring service stopped, and send a daily progress summary. |
| **Foreground service** | To keep the blocker countdown timer running reliably. |

You grant each permission manually in Android settings. You can revoke any of them at any time. The App will stop working correctly without them.

---

## 3. Information stored on your device

The following data is created and kept **locally on your device only**. It is not sent to us:

- **Your settings:** the list of apps you chose to monitor, time limits, pause durations, and grace periods.
- **Block history:** for each time the blocker is shown, the package name of the monitored app, the date and time, and the outcome (closed, bypassed, or completed).
- **Monitoring state:** temporary session timers used to track how long a monitored app has been open.

This data is used only to enforce your limits and to show your own progress, for example in the daily summary notification.

### Android Auto Backup

If you have **Google backup** enabled on your device, Android may include the App's local data (settings and block history) in your device backup to your Google account. That backup is handled by Google under [Google's Privacy Policy](https://policies.google.com/privacy). We cannot access it. You can turn backup off in your Android settings.

---

## 4. Information collected by third-party services

UnScroll uses the following Google Firebase services. They collect information automatically when you use the App and send it to Google's servers.

### Firebase Analytics

Used to understand how the App is used in aggregate, for example how often the blocker appears and whether users close the app or continue. The App logs these events:

- `starting_block`: includes the configured blocker wait time
- `stop_app`: no additional parameters
- `continue_app`: includes the grace period, in minutes, that you selected

These events **do not include the names of the apps you monitor**. Firebase Analytics also automatically collects information such as an app instance identifier, device model, OS version, app version, language, approximate location (country, region, and city, derived from your IP address), and session and engagement data.

### Firebase Crashlytics

Used to diagnose crashes. When the App crashes, Crashlytics collects the crash stack trace, device model, OS version, app version, device state at the time of the crash (for example free memory and orientation), and an installation identifier.

### Firebase Performance Monitoring

Used to measure app performance. It collects data such as app start-up time, screen rendering performance, network request timing, device model, OS version, and an installation identifier.

Google processes this data under its own terms:

- [Google Privacy Policy](https://policies.google.com/privacy)
- [Firebase Privacy and Security](https://firebase.google.com/support/privacy)

We use this data only to maintain and improve the App. We do not combine it with other data to identify you, and we do not use it for advertising.

---

## 5. How we share information

We do not sell, rent, or trade your information. Data is shared only:

- with **Google (Firebase)**, as a service provider, as described in Section 4;
- if required by law, regulation, or valid legal process.

---

## 6. Data retention

- **On-device data** stays on your device until you clear the App's data or uninstall the App.
- **Firebase data** is kept according to Google's retention settings. Analytics event-level data is kept for up to 2 months, and user-level data (linked to the app instance identifier) is kept for up to 14 months. Crashlytics crash reports are kept for up to 90 days.

---

## 7. Your choices and controls

- **Delete local data:** go to *Android Settings → Apps → UnScroll → Storage → Clear data*, or uninstall the App.
- **Stop monitoring:** turn off UnScroll's Accessibility Service or Usage Access in Android settings at any time.
- **Backups:** turn off Google backup in Android settings to prevent local data from being included in device backups.
- **Other requests:** to ask about, access, or delete data collected through Firebase, contact us (see Section 10). Because we do not collect your name, email, or account information, we may need your help to identify which data relates to you.

Depending on where you live (for example the EU/EEA, the UK, California, or Brazil under the LGPD), you may have rights to access, correct, delete, or object to the processing of your personal data. Contact us to exercise these rights.

---

## 8. Security

Local data is stored in the App's private storage, which other apps cannot access on a non-rooted device. Data sent to Firebase is encrypted in transit using HTTPS. No method of storage or transmission is completely secure, but we take reasonable steps to protect your information.

---

## 9. Children's privacy

UnScroll is not directed at children under 13 (or the minimum age required in your country). We do not knowingly collect personal information from children. If you believe a child has provided personal information through the App, contact us and we will take steps to delete it.

---

## 10. Contact

If you have questions about this Privacy Policy, contact:

**Almost Done Studios**
Email: **otaviosmarin@gmail.com**

---

## 11. Changes to this policy

We may update this Privacy Policy from time to time. Changes will be posted on this page with a new effective date. Significant changes will also be noted in the App's release notes.
