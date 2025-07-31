# 🗂️ LinguoAI Data Model

## 🧍 Entity: User

| Field             | Type        | Description                                      |
|------------------|-------------|--------------------------------------------------|
| user_id          | UUID        | Unique identifier for the user                  |
| name             | String      | Full name of the user                           |
| email            | String      | User's email address                            |
| native_language  | String      | User’s first language                           |
| english_level    | String      | CEFR level (e.g., A2, B1, C1)                   |
| interests        | [String]    | Topics user wants to practice                   |
| goals            | [String]    | Learning and professional development goals     |
| preferences      | JSON        | User-defined preferences (voice, tone, etc.)    |
| created_at       | Timestamp   | When the user was created                       |
| last_active_at   | Timestamp   | Last time user engaged with the agent           |

---

## 📄 Entity: UserContext

| Field             | Type        | Description                                      |
|------------------|-------------|--------------------------------------------------|
| context_id       | UUID        | Unique identifier for the context source        |
| user_id          | UUID        | Foreign key to `User`                           |
| source_type      | String      | Type (e.g., 'email', 'document', 'calendar')    |
| source_uri       | String      | Path or API URI to fetch data                   |
| keywords         | [String]    | Extracted work-related terms                    |
| topics           | [String]    | Detected topics from context                    |
| updated_at       | Timestamp   | Last updated time                               |

---

## 🗣️ Entity: ConversationSession

| Field             | Type        | Description                                      |
|------------------|-------------|--------------------------------------------------|
| session_id       | UUID        | Unique identifier for a conversation            |
| user_id          | UUID        | Foreign key to `User`                           |
| mode             | String      | Mode of session (freeform, roleplay, etc.)      |
| transcript       | Text        | Full text transcript of the session             |
| audio_uri        | String      | Location of recorded audio                      |
| duration         | Integer     | Duration in seconds                             |
| timestamp        | Timestamp   | Start time of the session                       |

---

## 🧠 Entity: FeedbackLog

| Field             | Type        | Description                                      |
|------------------|-------------|--------------------------------------------------|
| feedback_id      | UUID        | Unique identifier                               |
| session_id       | UUID        | Foreign key to `ConversationSession`            |
| type             | String      | Type (grammar, pronunciation, vocabulary)       |
| content          | Text        | Feedback content                                |
| severity         | String      | Suggestion, Minor, Major                        |
| timestamp        | Timestamp   | When the feedback was generated                 |

---

## 🧾 Entity: VocabularyTracker

| Field             | Type        | Description                                      |
|------------------|-------------|--------------------------------------------------|
| word_id          | UUID        | Unique identifier                               |
| user_id          | UUID        | Foreign key to `User`                           |
| word             | String      | The vocabulary word                             |
| context_sample   | Text        | Sentence used in conversation                   |
| status           | String      | ('New', 'Practicing', 'Mastered')               |
| added_at         | Timestamp   | When the word was added                         |

---

## 📅 Entity: ProgressReport

| Field             | Type        | Description                                      |
|------------------|-------------|--------------------------------------------------|
| report_id        | UUID        | Unique identifier for the report                |
| user_id          | UUID        | Foreign key to `User`                           |
| period_start     | Date        | Start date of the report                        |
| period_end       | Date        | End date of the report                          |
| summary          | Text        | Summary of improvement and challenges           |
| stats            | JSON        | Metrics (e.g., errors reduced, time practiced)  |

---

## 🔗 Relationships

- `User` 1—∞ `UserContext`
- `User` 1—∞ `ConversationSession`
- `ConversationSession` 1—∞ `FeedbackLog`
- `User` 1—∞ `VocabularyTracker`
- `User` 1—∞ `ProgressReport`

