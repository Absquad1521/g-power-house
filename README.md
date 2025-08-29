# G-POWER HOUSE

Simple game store website (play external web games) with support for Firebase Auth, Firestore, Storage and admin role.

## Setup

1. Copy files into web host folder.
2. Create a Firebase project (optional for production):
   - Enable Authentication (Email/Password & Google).
   - Enable Firestore and Storage (for thumbnails & profile pics).
3. In `firebase/firebase-config.js` paste your Firebase config and set `window.USE_FIREBASE = true`.
4. Ensure each HTML includes Firebase SDK `<script>` tags (already present in files).
5. Open site via a static server (VSCode Live Server or `npx http-server`).

## Notes

- Local mode (USE_FIREBASE=false) works for testing but is not secure.
- Admin role: set `users/{uid}.role = "admin"` in Firestore for admin access.
- If external sites block iframe embedding (X-Frame-Options), `play.html` provides "Open External" button.

## Files
See folder structure inside project root.
