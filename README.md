 **Manual Mobile App Testing — My Demo App**

About the Project:
A practical manual testing project focused on Android mobile application behaviour, usability, compatibility, reliability, and device-specific scenarios. Testing was performed using a real Android phone and Android emulators.

## Application & Test Environment
- **Application:** My Demo App (React Native)
- **Version:** 1.3.0, Build 244
- **Real Device:** Samsung SM-A307FN, Android 11
- **Emulators:** Small phone (720 × 1280) and medium phone (1080 × 2400, 420 dpi)
- **Testing Period:** 17–25 October 2026

## Testing Coverage
- Smoke testing and core functionality
- Login validation and session persistence
- Cart, quantity, item removal, and price calculations
- Network connectivity and offline behaviour
- App lifecycle: background, foreground, restart, and interruptions
- Screen size, resolution, orientation, keyboard, font size, display size, and split-screen testing
- Runtime permissions: allow, deny, and revoke
- Performance: launch time, memory usage, scrolling smoothness, and battery observations
- Localization and right-to-left (RTL) layout
- Basic security checks, logout behaviour, and sensitive data in logs
- Touch gestures and navigation
- Low-resource conditions, cache, app data, and background process termination
- Accessibility checks using TalkBack
- Store readiness: version information, Android API levels, and permissions

## Test Results Summary
- **15** test scenarios documented
- **112** test cases listed
- **82** results marked Passed/OK
- **6** results marked as bugs
- **13** questions or improvement ideas
- **4** bug reports documented
- **Smoke Test:** PASS — build accepted for further testing

Performance measurements were recorded separately and are not included in the pass/fail totals.

## Key Bugs Identified
1. **High — Incorrect cart total:** The cart displayed -$16,274.58 instead of the expected $39.98 for two products. The issue was not reproduced after resetting app data in the tested quantities up to 21.
2. **Low — Offline image recovery:** Some Wikipedia article images did not reload after internet connectivity returned. A repeat test later worked correctly.
3. **High — Font-size configuration crash:** My Demo App crashed when the system font size was changed while the app was in the background.
4. **High — Activity recreation crash:** My Demo App displayed “keeps stopping” after returning from Home with Android's “Don't keep activities” developer setting enabled.

## Tools Used
- Android Debug Bridge (ADB)
- Android Studio Emulator
- Real Android device
- Android Developer Options and system settings
- Manual test cases and exploratory testing
- Logcat for crash investigation
- Spreadsheet-based test tracking and bug reporting

## Project Learnings
- Designing and executing mobile-specific test scenarios
- Testing across device sizes and Android system configurations
- Reproducing and documenting defects
- Recording expected versus actual results
- Investigating crashes and app lifecycle behaviour
- Understanding the difference between a test observation, a confirmed defect, and an unresolved question

## Test Documentation
The accompanying Excel workbook contains the test summary, scenarios, detailed test cases, observations, performance measurements, and bug reports.


