# Tuesday League - Firebase Admin/Password Setup

This version uses a simple visible username `admin`. The password is NOT stored in the GitHub page.
Firebase Authentication securely checks the password using the hidden account email `admin@league-b6d74.app`.

## Firebase setup

1. Open the Firebase project `league-b6d74`.
2. Go to Authentication > Sign-in method.
3. Enable **Email/Password** and save.
4. Go to Authentication > Users and create one user:
   - Email: `admin@league-b6d74.app`
   - Password: choose your own strong password.
5. Go to Firestore Database > Rules.
6. Replace the rules with the contents of `firestore.rules` in this folder and click Publish.
7. Make sure Firestore Database itself has already been created.

## GitHub

Replace the `index.html` in your `League` repository with this new `index.html`.

## How it works

Visitors can view the league without signing in.
To edit, click **Admin Sign In** and use:
- Username: `admin`
- Password: the password you created in Firebase Authentication.

Once signed in, score changes save to Firebase automatically and sync to other devices.

## Latest interface changes

- Teams default to alphabetical order by the first teammate name (the name before the comma).
- The search box filters instantly by either teammate name.
- Rank by Avg is still available; click Alphabetical to return to the normal view.
