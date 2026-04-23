# Jammin

A social music review and discovery app — think Letterboxd, but for music. Share what you're listening to, write reviews, and see what your friends are into.

Built with React Native (Expo), Firebase, and the Spotify API.

---

## Features

- **Social feed** — see your friends' reviews and listening activity in real time
- **Music reviews** — rate and review songs and albums, leave comments on friends' reviews
- **Discovery** — browse new releases, featured playlists, and personalized recommendations based on your Spotify listening history
- **Spotify stats** — view your top tracks and artists across different time ranges
- **Profiles** — follow friends, see their reviews, saved items, and listening stats

## Tech Stack

| Layer | Tech |
|---|---|
| Framework | React Native + Expo (SDK 53) |
| Auth & Database | Firebase (Auth, Firestore, Storage) |
| Music Data | Spotify Web API |
| Analytics | Amplitude |
| Navigation | React Navigation (bottom tabs + stack) |

## Getting Started

### Prerequisites

- Node.js 18+
- Xcode (for iOS simulator)
- A Spotify developer app with a registered redirect URI (`jammin://auth/callback`)
- A Firebase project with Auth and Firestore enabled

### Install

```bash
git clone https://github.com/cjindart/jammin.git
cd jammin
npm install
```

### Run on iOS Simulator

```bash
npx expo run:ios
```

> This app uses `expo-dev-client` and cannot run in Expo Go. `npx expo run:ios` builds the native app and launches it in the simulator.

### Run on Android

```bash
npx expo run:android
```

## Project Structure

```
jammin/
├── screens/          # All app screens (Feed, Review, Profile, Auth, etc.)
├── components/       # Reusable UI components
├── services/         # Firebase and Spotify API logic
├── context/          # React context providers (auth, Spotify stats)
├── navigation/       # Stack and tab navigator definitions
└── assets/           # Icons, images, splash screen
```
