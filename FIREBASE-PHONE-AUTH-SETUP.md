# FICTION CLUB demo — Firebase Phone OTP activation

The phone-authentication UI and Firebase Phone Auth client flow are implemented in `login.html`. Real OTP delivery remains intentionally inactive until the project owner connects a Firebase Web App.

## One-time Firebase Console steps

1. Open the Firebase project that should own FICTION CLUB demo authentication.
2. Go to **Project settings → General → Your apps** and register a **Web app** if one does not already exist.
3. Copy that Web app's Firebase config into `firebase-config.js`:
   - `apiKey`
   - `authDomain`
   - `projectId`
   - `storageBucket`
   - `messagingSenderId`
   - `appId`
4. Go to **Authentication → Sign-in method** and enable **Phone**.
5. In **Authentication → Settings → Authorized domains**, add:
   - `shafiintj-source.github.io`
6. In Phone provider settings, review the SMS region policy and allow **India (+91)** if the project policy blocks it.
7. For safe initial testing, add a Firebase **test phone number and fixed test code** under the Phone provider's testing section. Test numbers do not send real SMS.
8. Open the demo login page, choose **Phone**, enter a mobile number, complete the reCAPTCHA, press **Send verification code** again, and verify the received code.

## Important safety notes

- `firebase-config.js` contains public Firebase web-app configuration, not a private credential. Do not add service-account JSON, Admin SDK private keys, private API tokens, or payment secrets to this public repository.
- Firebase Phone Auth sends a real SMS only after the project is configured and the domain is authorized. SMS usage is subject to Firebase quotas, billing and abuse controls.
- Do not test using a real customer's phone number without their consent.
- The demo login does not yet have a backend user profile, role system, account deletion workflow, or production security review.
- Email and Google authentication are intentionally left for the next phase.
- This is isolated from the production FICTION CLUB website and its Firebase Hosting deployment.

## Current implementation status

- [x] Firebase Phone Auth client integration
- [x] reCAPTCHA verifier flow
- [x] India +91 normalization for 10-digit numbers
- [x] OTP confirmation and Firebase session sign-in
- [x] Clear configuration / setup messaging
- [ ] Project owner's Firebase Web App config
- [ ] Enable Phone provider and authorize GitHub Pages domain
- [ ] Live SMS test and end-to-end verification
