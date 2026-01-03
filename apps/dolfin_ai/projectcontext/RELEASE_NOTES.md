# Release Notes

## Version 0.0.2 (Build 3)
**Release Date:** January 4, 2026

### Key Highlights
- **Play Store Compliance**: Removed Advertising ID permission to comply with Google Play policies.
- **Security Hardening**: Implemented database encryption, biometric authentication, and code obfuscation (ProGuard) for enhanced security.
- **Dashboard Improvements**: Fixed critical issues with dashboard data refreshing. The dashboard now updates instantly when you edit or delete transactions.
- **Improved Stability**: Addressed multiple crash scenarios in Chat, Subscription, and Analytics modules.

### Detailed Changelog

#### 🔒 Security
- **Database Encryption**: Secured local database with SQLCipher encryption.
- **Biometric Auth**: Added functional App Lock with biometric verification (Face ID/Fingerprint).
- **Obfuscation**: Enabled code shrinking and obfuscation to protect app logic.

#### 🏠 Dashboard & Home
- **Instant Refresh**: Fixed an issue where the dashboard metrics (Balance, Spending Trend) wouldn't update after modifying transactions.
- **View All Navigation**: Resolved a bug where returning from the "View All" transactions page would prevent the dashboard from refreshing.
- **Spending Graph**: Fixed rendering issues (handling sparse data, hiding graph when expenses are 0, fixing syntax errors).
- **Navigation**: Improved navigation stability to prevent widget context invalidation errors.

#### 💬 Chat & AI
- **Crash Fixes**: Resolved a crash related to analytics event logging in the Chat module.
- **Error Handling**: Enforced consistent error handling in manual transaction input flows.

#### ⚙️ Settings & Core
- **Database Reset**: Added a recovery mechanism to handle unrecoverable database states by resetting safely.
- **Subscription**: Fixed a crash in analytics logging for subscription events.
- **Google Auth**: Ensured Google Auth tokens are correctly saved and handled.
- **Profile**: Added a visual tick mark indicator to the currency selector sheet.
- **UI Refinements**: Modernized snackbar designs for better visibility and aesthetics.
