This project builds upon the DEV@Deakin platform to create a seamless, multi-page authentication flow. Users can create an account, securely log in, and navigate across the platform with consistent layouts.

### Key Features
* **Shared Navigation & Footer:** Consistent top navbar and footer rendered across all pages.
* **Responsive Routing:** Built using `react-router-dom` to switch seamlessly between Home, Login, and Registration pages.
* **User Registration:** Validates inputs (full name, email format, password matching) before safely storing details in Firebase Firestore.
* **Password Encryption:** Ensures user security by hashing passwords with `bcryptjs` instead of storing them as plain text.
* **User Authentication:** Validates email and credentials against Firestore records, automatically redirecting users to the home dashboard upon success or prompting retry/sign-up on failure.
* **Environment Variable Protection:** Protects Firebase API keys and secrets via `.env`, keeping credentials out of version control.


## Tech Stack

* **Frontend Framework:** React (via Vite)
* **Routing:** React Router v6
* **Database & Auth:** Firebase Firestore
* **Security & Utilities:** `bcryptjs` (password hashing)
* **Styling:** CSS3 / Modern Flexbox & Grid
