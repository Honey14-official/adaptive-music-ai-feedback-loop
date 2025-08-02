# 🎨 Wireframes – Adaptive Music AI with Closed-Loop Learning

---

## 🎯 Objective
Visually map out the **core user flows** of the MVP: onboarding, playlist recommendations, and feedback loop.  
These wireframes act as the blueprint for frontend development and ensure a consistent UX.

---

## 1️⃣ Onboarding Flow

### Screen 1 – Welcome
- **Elements:**
  - Logo + App Name
  - Short tagline: "Your music, always evolving"
  - CTA button: "Get Started"
- **Purpose:** Create first impression & encourage sign-up.

---

### Screen 2 – Genre & Mood Selection
- **Elements:**
  - Multi-select chips for genres (Pop, Rock, Indie, Jazz, etc.)
  - Mood selector (Happy, Chill, Energetic, etc.)
  - CTA: "Continue"
- **Purpose:** Capture core preferences to seed recommendations.

---

### Screen 3 – Artist Selection
- **Elements:**
  - Search bar with autocomplete
  - Select favorite artists
  - CTA: "Finish Setup"
- **Purpose:** Personalize recommendations further.

---

**Flow Diagram:**
Welcome → Genre & Mood Selection → Artist Selection → Home Screen


---

## 2️⃣ Playlist Recommendation Flow

### Screen 4 – Home Screen
- **Elements:**
  - Playlist cards with:
    - Cover art
    - Playlist title
    - Play button
  - Tabs for “Recommended” and “Recently Played”
- **Purpose:** Provide immediate listening options.

---

### Screen 5 – Now Playing
- **Elements:**
  - Song title, artist, album art
  - Playback controls (Play/Pause, Skip, Like, Dislike)
  - “Not Relevant” button
- **Purpose:** Central hub for music playback and feedback.

---

**Flow Diagram:**
Home Screen → Now Playing → Feedback Capture


---

## 3️⃣ Feedback Capture Flow

### Screen 6 – Feedback Pop-Up
- **Trigger:** High skip rate detected for playlist
- **Elements:**
  - Title: “Help us improve your mix”
  - Options:
    - Not Relevant
    - Wrong Genre
    - Overplayed
  - Submit button
- **Purpose:** Gather explicit feedback to adjust recommendations.

---

**Flow Diagram:**
Now Playing → Feedback Pop-Up → Save Feedback to DB



---

## 4️⃣ AI Adaptation & Validation Flow (Internal)

### Screen 7 – Engagement Dashboard
- **Elements:**
  - Charts for skip rate trends
  - Average listening time
  - Retraining history log
- **Purpose:** Internal team tool to validate AI improvements.

---

**Flow Diagram:**
Feedback Data → AI Retraining → Updated Playlists → Dashboard Metrics


---

## 📌 Next Step in ACSPO Flow
Move to **`ui-style-guide.md`** – define typography, color palette, and component styles to keep the design consistent across the MVP.

