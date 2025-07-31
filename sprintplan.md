# 🏃 Sprint Plan – LinguoAI Agent (for Windsurf)

## 🗓️ Overview

**Product:** LinguoAI – Speech-Based English Practice Agent  
**Platform:** Windsurf (Agent-based AI IDE)  
**Team Roles:**
- 🧠 PromptOps: Responsible for prompt tuning and natural language understanding.
- 🤖 CodeGenAgent: Builds and tests backend logic and API connectors.
- 🎨 UI Agent: Creates interactive UI workflows.
- 🔬 QA Agent: Validates outputs, speech recognition, and language correction logic.

---

## 🚀 Sprint 1: Core Infrastructure & Onboarding (Weeks 1–2)

### Goals:
- Establish user onboarding flow
- Build foundational memory & context storage
- Implement basic speech-to-text and text-to-speech agent workflows

### Key Deliverables:
- User entity schema
- Onboarding quiz + interest tagging flow
- Memory module to store and retrieve interests, context, and CEFR level
- Voice input/output system (browser-based or app stub)

### User Stories:
- US 1.1: Onboarding quiz assigns CEFR level
- US 1.2: User selects interests, domains, and personal goals
- US 2.1: Enable voice input + TTS response loop
- US 5.1: Memory recalls preferences and interests per session

### Agents Activated:
- PromptOps: Quiz prompt design, CEFR scoring
- CodeGenAgent: MemoryStore and onboarding API
- UI Agent: Build quiz UI + onboarding wizard
- QA Agent: Validate speech-to-text latency and CEFR accuracy

---

## 🧠 Sprint 2: Mode Switching + Feedback (Weeks 3–4)

### Goals:
- Launch conversational mode switching
- Real-time feedback on grammar and pronunciation
- Early document-based context ingestion

### Key Deliverables:
- Modular “conversation mode” agent
- Feedback log generator (with severity classification)
- OAuth integration with Google Docs/Calendar
- Early work-related vocabulary extraction

### User Stories:
- US 2.2: User selects or speaks mode (e.g., “Let’s do roleplay”)
- US 3.1: Real-time grammar feedback with colored tags
- US 3.2: Pronunciation detection and feedback with waveform hints
- US 1.3: Connect work context via OAuth and auto-ingest top 5 topics

### Agents Activated:
- PromptOps: Feedback correction style, context-based conversation prompts
- CodeGenAgent: FeedbackLog schema + Google API calls
- UI Agent: Mode switch UI + feedback popover
- QA Agent: Test document ingestion and speech mode routing

---

## 📅 Sprint 3 (Optional / Future): Progress Reports + Task Assistant

### Goals:
- Build weekly auto-generated progress reports
- Implement task assistant to summarize docs, send emails

### Key Deliverables:
- Report generator with CEFR delta, usage stats
- Email draft assistant via speech
- Summarization-to-voice loop

### User Stories:
- US 3.2: Weekly summary with strengths and weaknesses
- US 4.1: Dictate emails using work vocabulary
- US 4.2: Summarize linked documents with agent voice

---

## 📌 Rituals

| Meeting             | Frequency     | Description                                      |
|---------------------|---------------|--------------------------------------------------|
| Planning Kickoff    | Sprint Day 1  | Set scope, assign agent tasks                   |
| Agent Standups      | Daily         | Log agent task success/fail states              |
| Demo Day            | Sprint End    | Show off working flows, test interactively      |
| Retrospective       | Sprint End    | Adjust agent roles, prompt quality, task limits |

---

## ✅ Success Metrics

- ⏱️ Voice latency < 2s for roundtrip
- 🎯 Mode accuracy > 90%
- 📊 Feedback logged for > 80% of user utterances
- 📈 CEFR-level adjusted based on agent logs after 2 weeks
- 📥 Document ingestion populates at least 10 unique keywords per user

