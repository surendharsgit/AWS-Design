# ThinkFix AI – System Design

## 1. Design Philosophy
- Learning-first, not speed-first
- Prevent shortcut-based AI usage
- Encourage deep thinking through guided reasoning

---

## 2. High-Level Workflow
User → Web App → Backend Orchestrator → AI Engine → Guided Response


---

## 3. System Components

### 3.1 Frontend (Web Application)
- Code input field
- Error message input
- Chat-style Socratic interface
- Explanation input area
- No "Give Solution" or skip button

**UX Guardrails**
- Minimum explanation length
- No skipping steps
- Optional response delay

---

### 3.2 Backend (FastAPI – Prototype)
- Handles API requests
- Manages debugging session state
- Routes prompts to AI engine
- Enforces no-direct-answer policy

---

### 3.3 AI Intelligence Layer (AWS Bedrock)
- Socratic Question Generator
- Answer Evaluation Engine
- Difficulty Adapter
- Guardrail Layer to block solution leakage

---

### 3.4 Data Handling
- Session-based in-memory storage
- Stores:
  - Error category
  - Question progression
- No persistent storage in prototype

---

## 4. Security and Ethics
- No personal data collected
- No permanent code storage
- Transparent AI behavior

---

## 5. Future Enhancements
- DynamoDB for persistent learning history
- VS Code extension integration
- Learning analytics dashboard
- Personalized concept recommendations

---

## 6. Key Design Insight
The system controls the AI behavior to ensure learning, not shortcut completion.
