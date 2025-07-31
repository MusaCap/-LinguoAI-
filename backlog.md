# 📋 LinguoAI Backlog: Epics & User Stories

## 🧠 Epic 1: Personalized User Onboarding

### 🧾 User Story 1.1
**As a** new user  
**I want to** complete an onboarding quiz  
**So that** the agent can assess my English level and personalize interactions.

**Acceptance Criteria:**
- Quiz includes grammar, vocabulary, pronunciation segments.
- CEFR level is inferred and stored in user profile.
- Results are shown in a friendly summary.

---

### 🧾 User Story 1.2
**As a** user  
**I want to** select my interests and work domains  
**So that** the agent can tailor conversations around them.

**Acceptance Criteria:**
- User selects tags like "VC", "startups", "climate", "tech hiring", etc.
- Tags stored and used to inform context engine.

---

### 🧾 User Story 1.3
**As a** user  
**I want to** link my Google Docs, Email, or Calendar  
**So that** the agent can learn my work vocabulary and tasks.

**Acceptance Criteria:**
- OAuth-based secure linking.
- Basic summary of what is extracted shown to user.

---

## 🗣️ Epic 2: Voice-Driven Conversational Engine

### 🧾 User Story 2.1
**As a** user  
**I want to** initiate and maintain conversations with voice  
**So that** I can practice speaking without typing.

**Acceptance Criteria:**
- Wake-word or push-to-talk supported.
- Microphone stream captured and transcribed in real time.
- Conversational turn-taking maintained.

---

### 🧾 User Story 2.2
**As a** user  
**I want to** choose between different conversation modes  
**So that** I can practice what’s most useful to me.

**Modes:**
- Freeform Chat
- Roleplay (e.g., investor meeting)
- Pronunciation Practice
- Vocabulary Builder
- Translation Assistant

**Acceptance Criteria:**
- Mode switch works via voice and UI.
- State saved between sessions.

---

## 📈 Epic 3: Feedback and Progress Tracking

### 🧾 User Story 3.1
**As a** user  
**I want to** receive feedback on grammar, pronunciation, and vocabulary  
**So that** I can learn from my mistakes.

**Acceptance Criteria:**
- Real-time corrections during or after session.
- Visual & audio feedback available.

---

### 🧾 User Story 3.2
**As a** user  
**I want to** receive weekly progress reports  
**So that** I can track my learning and improvements.

**Acceptance Criteria:**
- CEFR trends, errors reduced, time spent shown.
- Summary and highlights emailed or displayed.

---

## 🧾 Epic 4: Task-Oriented Assistant Capabilities

### 🧾 User Story 4.1
**As a** user  
**I want to** dictate work-related notes or emails  
**So that** I can save time while practicing English.

**Acceptance Criteria:**
- Dictation transcribed with formatting suggestions.
- Integration with Gmail or task apps optional.

---

### 🧾 User Story 4.2
**As a** user  
**I want to** have the agent summarize documents aloud  
**So that** I can understand complex topics while practicing listening.

**Acceptance Criteria:**
- Document URI provided or selected from calendar/email.
- Audio summary generated in natural speech.

---

## 🛡️ Epic 5: Memory and Personalization

### 🧾 User Story 5.1
**As a** returning user  
**I want to** have the agent remember previous conversations and vocabulary  
**So that** learning feels consistent.

**Acceptance Criteria:**
- Context history and learned words stored in memory.
- Agent recalls and revisits concepts naturally.

---

### 🧾 User Story 5.2
**As a** user  
**I want to** configure how much memory or context the agent keeps  
**So that** I can control personalization and privacy.

**Acceptance Criteria:**
- User toggles memory features and sets retention rules.
- Preferences respected in real-time interactions.

---

## 🔒 Epic 6: Privacy, Security & Controls

### 🧾 User Story 6.1
**As a** user  
**I want to** view and delete my stored data  
**So that** I retain full control over my privacy.

**Acceptance Criteria:**
- Clear dashboard of stored content.
- Deletion immediate and irreversible.

---

### 🧾 User Story 6.2
**As a** user  
**I want to** see what context the agent is using during a session  
**So that** I can verify what’s influencing its answers.

**Acceptance Criteria:**
- Active context shown on demand.
- Easy "pause" or "mute memory" control available.

---

## 🎯 Epic 7: Progress-Based Curriculum Builder (Future)

### 🧾 User Story 7.1
**As a** user  
**I want to** receive curated lessons based on my weak areas  
**So that** my study time is more efficient.

**Acceptance Criteria:**
- Vocabulary, grammar, listening modules assigned dynamically.
- Lesson difficulty adapts to performance over time.

---

## 🧪 Epic 8: Evaluation & Testing

### 🧾 User Story 8.1
**As a** QA team  
**I want to** simulate edge cases in speech recognition  
**So that** we can ensure consistent understanding for all accents.

**Acceptance Criteria:**
- Test suite includes accented English, background noise, and disfluency.
- Accuracy benchmarks > 85% per test set.

---

