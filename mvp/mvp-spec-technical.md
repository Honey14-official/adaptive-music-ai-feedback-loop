# 📄 MVP Specification – Adaptive Music AI with Closed-Loop Learning

---

## 🎯 Objective
Define the **functional requirements**, **technical specifications**, and **success criteria** for the MVP of the Adaptive Music AI project.  
This document will guide development, testing, and validation.

---

## 1️⃣ MVP Goals
- Deliver a **music recommendation engine** that adapts to user preferences using a **closed-loop feedback system**.
- Minimize irrelevant recommendations by integrating **real-time skip detection** and **explicit user feedback**.
- Validate improvement in engagement after preference shifts.

---

## 2️⃣ Core MVP Features

| ID | Feature | Description | Priority |
|----|---------|-------------|----------|
| F1 | **Onboarding – Mood & Genre Selection** | First-time user selects preferred genres, moods, and artists. | High |
| F2 | **Feedback Capture** | Users can mark tracks as "Not Relevant" or provide quick feedback. | High |
| F3 | **Listening History Tracking** | System logs play, skip, like, and dislike events. | High |
| F4 | **Retraining Trigger** | Skip rate thresholds trigger AI model retraining. | Medium |
| F5 | **Updated Playlist Generation** | New playlists created post-retraining with fresher recommendations. | High |
| F6 | **Engagement Validation Dashboard** | Tracks engagement and validates recommendation quality. | Low (Internal) |

---

## 3️⃣ Technical Requirements

### Backend
- **Language/Framework:** Python (FastAPI / Flask)
- **Database:** PostgreSQL (User profiles, listening history), Redis (real-time events)
- **AI/ML:** Scikit-learn / TensorFlow / PyTorch for recommendation model
- **Data Processing:** Pandas / NumPy for feedback analysis

### Frontend
- **Language/Framework:** React Native (cross-platform mobile app)
- **UI Components:** Expo, Material UI for styling
- **API Communication:** Axios or Fetch API

### Infrastructure
- **Hosting:** AWS EC2 / Elastic Beanstalk
- **Storage:** AWS S3 for storing logs/models
- **Monitoring:** AWS CloudWatch or Prometheus

---

## 4️⃣ APIs to be Developed

| API | Method | Endpoint | Purpose |
|-----|--------|----------|---------|
| Get Initial Recommendations | GET | `/recommendations/initial` | Fetch first playlists after onboarding |
| Submit Feedback | POST | `/feedback` | Send explicit feedback data |
| Get Updated Recommendations | GET | `/recommendations/updated` | Fetch playlists post-retraining |
| Log Playback Event | POST | `/events/playback` | Store play/skip/like/dislike events |
| Trigger Retraining | POST | `/model/retrain` | Start retraining pipeline (internal) |

---

## 5️⃣ Data Flow
[User Action] → [Frontend Event Capture] → [Backend API] → [DB/Cache] → [Analysis Engine] → [Retraining Trigger] → [Updated Model] → [Refreshed Recommendations]


---

## 6️⃣ Success Metrics (Validation)

| Metric | Target |
|--------|--------|
| Skip Rate Reduction | ≥ 20% after retraining |
| Increase in Engagement Time | ≥ 15% |
| Feedback Participation Rate | ≥ 30% of active users |
| Recommendation Relevance Score | ≥ 80% based on post-update surveys |

---

## 7️⃣ Assumptions
- Users will provide **explicit feedback** if prompted simply and non-intrusively.
- Skip rate is a reliable proxy for content irrelevance.
- Initial onboarding preferences are **only a starting point**; the system must adapt over time.

---

## 8️⃣ Out of Scope for MVP
- Multi-language support
- Advanced collaborative filtering with social graph integration
- Offline playback
- Complex playlist curation beyond retraining updates

---

## 📌 Next Step in ACSPO Flow
Proceed to **Development Plan (`dev-plan.md`)** – break down MVP features into sprints, tasks, and ownership.

