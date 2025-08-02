# 📋 Product Backlog – Adaptive Music AI with Closed-Loop Learning

---

## 🎯 Objective
Maintain a **prioritized list of user stories** with acceptance criteria for the MVP.  
This backlog will evolve as feedback is collected during development.

---

## 🗂 Backlog Structure
- **Epic** – Large feature area (e.g., Onboarding, Feedback System)
- **User Story** – Describes functionality from the user’s perspective
- **Acceptance Criteria** – Conditions that must be met for the story to be complete
- **Priority** – High / Medium / Low

---

## 1️⃣ Epic: Onboarding & Preference Capture

**User Story 1 – Initial Genre/Mood Selection**  
_As a new user, I want to select my favorite genres and moods so that my playlists feel personal from the start._

**Acceptance Criteria:**
- User can select at least 3 genres and 1 mood
- Selections are saved in the database
- First playlist generated based on selections
- UI confirmation that preferences are saved

**Priority:** High

---

**User Story 2 – Artist Search & Selection**  
_As a new user, I want to pick favorite artists so that recommendations include them._

**Acceptance Criteria:**
- Search bar allows artist name entry
- Autocomplete suggestions appear
- Selected artists are saved and used in initial recommendations

**Priority:** Medium

---

## 2️⃣ Epic: Playlist Recommendations

**User Story 3 – Home Screen Playlist Display**  
_As a user, I want to see my playlists on the home screen so I can start listening right away._

**Acceptance Criteria:**
- Playlist cards show title, cover art, and play button
- Data fetched from `/recommendations/initial`
- At least 5 playlists displayed

**Priority:** High

---

## 3️⃣ Epic: Feedback Capture

**User Story 4 – Skip & Dislike Tracking**  
_As a user, I want the app to remember when I skip or dislike songs so it can improve recommendations._

**Acceptance Criteria:**
- Skip button event sent to `/events/playback`
- Dislike button sends feedback to `/feedback`
- Feedback stored in DB with timestamp

**Priority:** High

---

**User Story 5 – “Not Relevant” Feedback Pop-Up**  
_As a user, I want to quickly mark a song as not relevant so that the AI can avoid similar tracks._

**Acceptance Criteria:**
- Pop-up appears when skip rate is high for a playlist
- User can select a reason (Not Relevant, Wrong Genre, Overplayed)
- Data sent to `/feedback` API

**Priority:** High

---

## 4️⃣ Epic: AI Retraining

**User Story 6 – Automatic Retraining Trigger**  
_As a system, I want to retrain the model when skip rates exceed a threshold so that recommendations adapt._

**Acceptance Criteria:**
- Skip rate threshold configurable
- Retraining process starts automatically
- Updated model deployed within 24 hours

**Priority:** High

---

**User Story 7 – Updated Playlist Notification**  
_As a user, I want to know when my playlists have been refreshed so I can check new recommendations._

**Acceptance Criteria:**
- Push notification sent after retraining
- Notification links directly to updated playlist

**Priority:** Medium

---

## 5️⃣ Epic: Engagement Validation

**User Story 8 – Engagement Dashboard (Internal)**  
_As a product team member, I want to see engagement metrics so I can measure AI effectiveness._

**Acceptance Criteria:**
- Dashboard displays skip rate trends
- Engagement time per user tracked
- Export option available for CSV

**Priority:** Low

---

## 📌 Next Step in ACSPO Flow
Proceed to **Sprint Backlog (`sprint-backlog.md`)** – break this backlog into tasks for each sprint.
