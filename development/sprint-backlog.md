# 🗓 Sprint Backlog – Adaptive Music AI with Closed-Loop Learning

---

## 🎯 Objective
Translate the **Product Backlog** into actionable sprint-level tasks with direct mapping to user stories.

---

## Sprint 1 – Backend Setup & Database  
**Goal:** Build foundational backend infrastructure.

| Task ID | Linked User Story | Task Description | Status |
|---------|------------------|------------------|--------|
| S1-T1 | US1, US3 | Set up FastAPI backend with initial folder structure | ⬜ Not Started |
| S1-T2 | US1, US3 | Design PostgreSQL schema for `users`, `listening_history`, and `feedback_events` | ⬜ Not Started |
| S1-T3 | US3 | Implement `/recommendations/initial` API endpoint | ⬜ Not Started |
| S1-T4 | US4 | Integrate Redis for real-time skip tracking | ⬜ Not Started |
| S1-T5 | US3 | Write unit tests for initial API endpoints | ⬜ Not Started |

---

## Sprint 2 – Frontend Onboarding & Recommendations  
**Goal:** Enable new users to set preferences and receive playlists.

| Task ID | Linked User Story | Task Description | Status |
|---------|------------------|------------------|--------|
| S2-T1 | US1 | Build onboarding UI for genre & mood selection in React Native | ⬜ Not Started |
| S2-T2 | US2 | Implement artist search with autocomplete | ⬜ Not Started |
| S2-T3 | US1 | Connect onboarding form to `/recommendations/initial` API | ⬜ Not Started |
| S2-T4 | US3 | Build home screen playlist display with title, cover art, and play button | ⬜ Not Started |

---

## Sprint 3 – Feedback Capture & Event Logging  
**Goal:** Record user feedback to improve recommendations.

| Task ID | Linked User Story | Task Description | Status |
|---------|------------------|------------------|--------|
| S3-T1 | US4 | Implement skip button event tracking linked to `/events/playback` | ⬜ Not Started |
| S3-T2 | US4 | Implement dislike button feedback linked to `/feedback` | ⬜ Not Started |
| S3-T3 | US5 | Create “Not Relevant” feedback pop-up with reason options | ⬜ Not Started |
| S3-T4 | US4, US5 | Ensure all feedback events are saved in DB with timestamps | ⬜ Not Started |

---

## Sprint 4 – AI Model Integration & Retraining Logic  
**Goal:** Adapt playlists automatically based on user behavior.

| Task ID | Linked User Story | Task Description | Status |
|---------|------------------|------------------|--------|
| S4-T1 | US6 | Implement skip rate threshold detection logic | ⬜ Not Started |
| S4-T2 | US6 | Integrate initial AI recommendation model | ⬜ Not Started |
| S4-T3 | US6 | Build retraining pipeline (batch or incremental) | ⬜ Not Started |
| S4-T4 | US6 | Create `/model/retrain` API endpoint | ⬜ Not Started |
| S4-T5 | US7 | Send push notification when playlists are updated | ⬜ Not Started |

---

## Sprint 5 – Engagement Validation & Testing  
**Goal:** Measure AI effectiveness and fix issues.

| Task ID | Linked User Story | Task Description | Status |
|---------|------------------|------------------|--------|
| S5-T1 | US8 | Build internal dashboard for engagement metrics | ⬜ Not Started |
| S5-T2 | US8 | Integrate skip rate and engagement tracking | ⬜ Not Started |
| S5-T3 | All | Conduct QA testing on all features | ⬜ Not Started |
| S5-T4 | All | Fix critical bugs found during QA | ⬜ Not Started |

---

## Sprint 6 – Final Refinements & Deployment  
**Goal:** Prepare for MVP release.

| Task ID | Linked User Story | Task Description | Status |
|---------|------------------|------------------|--------|
| S6-T1 | All | Optimize API performance and query efficiency | ⬜ Not Started |
| S6-T2 | All | Implement basic error handling in backend & frontend | ⬜ Not Started |
| S6-T3 | All | Deploy backend to AWS EC2/Beanstalk | ⬜ Not Started |
| S6-T4 | All | Deploy frontend to TestFlight & Play Store internal testing | ⬜ Not Started |

---

## 📌 Next Step in ACSPO Flow
Move to **Wireframing & UI/UX Design (`wireframes.md`)** – visually map onboarding, playlist, and feedback flows before starting development.
