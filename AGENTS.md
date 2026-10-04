# Agent Guidelines for VokabelMeister Android

## Critical Security Rule
- **NEVER** commit keystores (`release.keystore`, `*.jks`, `*.p12`) or passwords to Git.
- `release.keystore` must remain strictly local and excluded via `.gitignore`.
- Gradle uses `if (file('release.keystore').exists())` fallback.

## Build Requirements
- Node.js >= 22 (Capacitor 8.5 requirement).
- Java 21 LTS (`temurin`).
- Sync assets using `npx cap sync android`.
- Build APKs with `./gradlew assembleDebug assembleRelease`.
- Tagging `v*` triggers release workflow and automated F-Droid repository updates via `PAT_TRIGGER`.
