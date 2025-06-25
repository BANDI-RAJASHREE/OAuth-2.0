# Spring Boot Google OAuth2 Login Demo

This project demonstrates how to implement Google OAuth2 login in a Spring Boot application securely manage credentials.

---

## Features

- Google Sign-In using OAuth2
- Public and protected routes
- Secure handling of client ID and secret via `.env`

---

## Prerequisites

- Java 17 or later
- Maven
- Google Cloud Console account

---

## Google Cloud Setup

1. Go to the Google Cloud Console and create a new project.
2. Enable the "People API".
3. Set up the OAuth Consent Screen with user details and test users.
4. Create OAuth2 credentials for a Web application.
5. Add the following URI to the Authorized Redirect URIs section:

   `http://localhost:8080/login/oauth2/code/google`

6. After creation, copy the client ID and client secret.

---


## Running the App

1. Ensure `.env` contains your Google credentials.
2. Run the project using Maven (or through your IDE).
3. Visit the `/secure` endpoint to trigger Google OAuth2 login.
4. After successful login, you'll be redirected and authenticated.

---

## Environment Variables

Use the following keys in your `.env` file:

- `GOOGLE_CLIENT_ID`
- `GOOGLE_CLIENT_SECRET`


---
http://localhost:8080/secure
redirects to 
![image](https://github.com/user-attachments/assets/cc46656f-611d-4661-a3a7-d339f011a9b4)
and displays
Hello Rajashree Bandi (rajashreebandi21@gmail.com)
