# 📡 API Specifications – Adaptive Music AI with Closed-Loop Learning

---

## 🎯 Purpose
This document defines the **API endpoints, request/response formats, and authentication** for the MVP.  
It ensures backend and frontend teams can work in parallel with a clear contract.

---

## 1️⃣ Authentication

### Endpoint: `POST /auth/register`
Registers a new user.

**Request:**
```json
{
  "email": "user@example.com",
  "password": "securepassword",
  "name": "John Doe"
}

** Response**
{
  "message": "User registered successfully",
  "user_id": "uuid"
}

Endpoint: POST /auth/login
Logs in a user and returns a JWT token.

Request:

json
Copy
Edit
{
  "email": "user@example.com",
  "password": "securepassword"
}
Response:

json
Copy
Edit
{
  "access_token": "jwt_token_here",
  "token_type": "bearer"
}

2️⃣ Onboarding
Endpoint: POST /onboarding/preferences
Stores user's initial preferences.

Request:

json
Copy
Edit
{
  "genres": ["Indie", "Rock"],
  "moods": ["Chill", "Energetic"],
  "artists": ["Artist 1", "Artist 2"]
}
Response:

json
Copy
Edit
{
  "message": "Preferences saved"
}
3️⃣ Recommendations
Endpoint: GET /recommendations
Fetches personalized playlists for the user.

Headers:
Authorization: Bearer jwt_token_here
Response:
{
  "playlists": [
    {
      "playlist_id": "123",
      "title": "Fresh Indie Hits",
      "cover_url": "https://cdn.app.com/covers/indie.jpg",
      "tracks": [
        {
          "track_id": "t1",
          "title": "Song 1",
          "artist": "Artist A",
          "duration": 210
        }
      ]
    }
  ]
}


4️⃣ Feedback Loop
Endpoint: POST /feedback/skip
Logs a skipped track.

Request:
{
  "track_id": "t1",
  "reason": "Not Relevant"
}
Response:
{
  "message": "Feedback recorded"
}
Endpoint: GET /feedback/stats
Fetches skip rate and engagement metrics (for AI retraining trigger).

Response:
{
  "skip_rate": 0.45,
  "average_listen_time": 125
}



5️⃣ AI Model Management
Endpoint: POST /ai/retrain
Triggers AI retraining with recent listening data.

Request:
{
  "time_range": "last_30_days"
}
Response:

{
  "message": "Model retraining started",
  "status": "in_progress"
}


6️⃣ Internal Dashboard
Endpoint: GET /dashboard/metrics
Returns engagement and retraining logs for internal team use.

Response:
{
  "metrics": {
    "skip_rate_trend": [0.45, 0.38, 0.29],
    "retraining_dates": ["2025-07-01", "2025-07-15"]
  }
}


📌 Next Step in ACSPO Flow
Proceed to testing-plan.md – outline the test strategy, types of testing, and tools to ensure the MVP meets quality standards.
