# Musement-Project

<div align="center">
  <h1>Musement</h1>
  <p>Discover concerts based on your favorite tracks — explore events, discuss them, and manage tickets effortlessly.</p>
</div>

## 🎶 About this Project

Musement is an interactive platform that helps users find their next live music experience. By importing your playlists from Spotify, the app analyzes your favorite artists, ranks them by listening frequency, and searches for upcoming concerts in your area. Beyond tailored event recommendations, Musement encourages social engagement: invite friends, join group outings, and discuss shows in dedicated concert threads. Manage your tickets in-app, store media securely in the cloud, and keep up with friends’ musical adventures—all from one intuitive interface.

## ✨ Features

* **User Authentication**: Sign up with email/password or Google OAuth2
* **Playlist Integration**: Import and parse playlists from Spotify
* **Personalized Recommendations**: Artist frequency ranking drives concert suggestions
* **Social Interaction**: Follow friends, send invitations, request to join groups
* **Discussion Threads**: Comment and share experiences under each concert event
* **Ticket Management**: Store, view, and manage tickets within the app
* **Cloud Media Storage**: Upload and serve photos/videos via Cloudinary

## 🛠️ Technology Stack

| Purpose               | Technology                |
| --------------------- | ------------------------- |
| UI (Android)          | Android SDK               |
| HTTP Framework        | Spring Boot               |
| ORM                   | Hibernate                 |
| Database              | PostgreSQL                |
| Full-Text Search      | Elasticsearch             |
| HTTP Client (Android) | Retrofit                  |
| Authentication        | Google Play Services Auth |
| Media Storage         | Cloudinary                |
| Testing               | JUnit                     |

## 🏛️ Application Architecture

Our high-level architecture consists of the following components:

1. **Client (Android)**: Native Android app uses Retrofit and Google Auth modules to send requests.
2. **Security Filter**: Validates incoming requests and passes authenticated calls to the server.
3. **Server**:

    * **Controllers**: Expose REST endpoints.
    * **Services**: Implement business logic (playlist parsing, recommendations, social features).
    * **Repositories**: Handle data persistence (Spring Data/Hibernate).
4. **Musement DB (PostgreSQL)**: Persists users, playlists, artists, events, tickets, and threads.
5. **External Services**:

    * **Spotify API**: Fetches user playlist data.
    * **Cloudinary**: Stores and serves user-uploaded media.

![Architecture Diagram](media/architecture.png)

## 🧩 Modules

This project contains two main modules of the Musement app:

1. **`Backend/`**: Spring Boot based REST API server (see [Backend/README.md](https://github.com/MusementProject/Backend/blob/main/README.md)  
2. **`Frontend/`**: Android application built with Android SDK (see [Frontend/README.md](https://github.com/MusementProject/Frontend/blob/main/README.md))

---

## 👥 About Authors

**Developers:**

* [Anna Artamonova](https://github.com/chepyr)
* [Julia Burmistrova](https://github.com/gtmnnn)
* [Nastia Malysheva](https://github.com/MalyshevaAN)

**Mentor:**

* [Anna Polupanova](https://github.com/polupanovaanna)

*National Research University Higher School of Economics, St. Petersburg, Spring 2025*
