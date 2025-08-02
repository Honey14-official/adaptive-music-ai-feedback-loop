# 🗺 User Journey – Adaptive Music AI with Closed-Loop Learning

---

## 🎯 Objective
Map out how a **first-time user** and a **returning user** will interact with the MVP features, highlighting **touchpoints**, **pain points**, and **system actions**.

---

## 📌 User Journey Overview

We will consider **two main scenarios**:

1. **First-Time User Onboarding & Personalization**
2. **Returning User with Changing Music Preferences**

---

## 1️⃣ First-Time User – Onboarding Flow

| Step | User Action | System Action | MVP Feature |
|------|-------------|--------------|-------------|
| 1 | Downloads and opens the app | App loads onboarding module | F1 – Mood & Genre Onboarding |
| 2 | Selects preferred genres, moods, and favorite artists | Preferences saved in **User Preferences DB** | F1 |
| 3 | Receives first set of recommended playlists | Recommendations fetched from initial AI model | F1 |
| 4 | Starts playing music | Playback events sent to **Listening History DB** | F3 |
| 5 | Skips some tracks, likes others | Feedback events logged in **Feedback Event Store** | F2 |
| 6 | Closes app | Data syncs for analytics & future personalization | F3, F4 |

---

## 2️⃣ Returning User – Preference Shift Flow

| Step | User Action | System Action | MVP Feature |
|------|-------------|--------------|-------------|
| 1 | Logs in after a week | Fetches latest recommendations | F5 – Weekly Playlist Refresh |
| 2 | Starts skipping 90s pop songs more frequently | Skip events detected by **Skip Pattern Detection Engine** | F3 |
| 3 | Taps “Not Relevant” on multiple tracks | Events stored in **Feedback Event Store** | F2 |
| 4 | Skip rate threshold exceeded | System triggers **Real-Time Retraining Pipeline** | F4 |
| 5 | AI model updates recommendations to indie music | New playlists generated | F4, F5 |
| 6 | User listens more and skips less | **Engagement Validation Dashboard** records improvement | F6 |

---

## 🔄 Visual Journey Map (Text-Based)

First-Time User:
[App Download] → [Mood & Genre Selection] → [Initial Playlist] → [Play / Skip / Like] → [Feedback Stored] → [Future Personalization]

Returning User with Changing Taste:
[Login] → [Playlists Loaded] → [High Skip Rate Detected] → [Feedback Captured] → [Retraining Triggered] → [Updated Recommendations] → [Increased Engagement]


---

## 🧠 Key Touchpoints
- **Onboarding** – Captures initial preferences (critical for first impressions).
- **Feedback Capture** – Quick tap + skip tracking for real-time signals.
- **Retraining Trigger** – Adapts to shifts in taste automatically.
- **Playlist Refresh** – Keeps recommendations fresh and relevant.
- **Engagement Validation** – Confirms changes improve user experience.

---

## 🚩 Potential Pain Points & Solutions

| Pain Point | Potential Fix |
|------------|---------------|
| Users ignore “Not Relevant” button | Gamify feedback collection with rewards/badges |
| Model retraining too slow | Use incremental retraining instead of full retrains |
| Playlist feels repetitive | Enforce diversity rules in playlist generation |
| Users skip onboarding | Provide default playlists + lightweight personalization prompts later |

---

## 📌 Next Step in ACSPO Flow
Proceed to **Wireframe Design** – visually design each key screen (Onboarding, Playlist, Feedback) to guide development and ensure usability.
