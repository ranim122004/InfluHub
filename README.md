# InfluHub — Android (Kotlin) + Node.js (Express)

InfluHub is a mobile app for creators & brands with a **Kotlin Android** frontend and a **Node.js/Express** backend.  
It ships a **complete authentication flow** (signup, login, forgot/reset, OTP), a **type-safe Retrofit** data layer, robust validation & error handling, and production-ready deployment (DNS + environment configs).

## ✨ Features

- **Full Authentication**: Signup, Login, Forgot/Reset Password, OTP verification, logout
- **Secure Sessions**: JWT access tokens, hashed passwords, guarded routes
- **Typed Networking**: Retrofit interfaces + data models, timeouts, error parsing
- **Smooth UX**: Fragment-based flows with Jetpack **Navigation** (safe transitions & arguments)
- 
*Why these tools?* Retrofit is the de-facto type-safe HTTP client on Android; Jetpack Navigation standardizes screen transitions; Express gives a minimal, fast API layer; JWT enables stateless auth on mobile. 
  
## 🧱 Architecture

**Android (Kotlin)**
- UI: XML layouts + `Fragment` screens for the auth flow  
- Data: **Retrofit** + **OkHttp** (logging) + **Gson** converter  
- Async: **Kotlin Coroutines** for main-safe network calls  
- Nav: Jetpack **Navigation** (graphs, `NavController`, Safe Args)

**Backend (Node.js)**
- **Express** REST API (auth & user endpoints)  
- **JWT** (`jsonwebtoken`) for tokens  
- **bcrypt** for password hashing  
- **cors** for cross-origin policy  
- **dotenv** for environment variables

