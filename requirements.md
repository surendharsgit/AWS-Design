# ThinkFix AI – Requirements

## 1. Overview
ThinkFix AI is an AI-powered learning assistant designed to help students and developers debug code by guiding their reasoning instead of providing instant fixes. The system uses Socratic questioning to improve long-term understanding and reduce AI dependency.

---

## 2. Functional Requirements

### 2.1 Submit Code & Error
- Users must be able to paste:
  - Source code
  - Compiler or runtime error message
- Input should accept plain text
- Prototype supports common programming languages (Python / Java / C)

---

### 2.2 Error Analysis
- System classifies errors into:
  - Syntax errors
  - Runtime errors
  - Logical or conceptual errors
- Relevant code context must be extracted for analysis

---

### 2.3 Socratic Questioning
- AI must:
  - Ask guided questions only
  - Avoid giving direct solutions initially
  - Progress step-by-step based on user responses

---

### 2.4 Forced Reasoning
- Users must provide written explanations
- Minimum explanation length is enforced
- No skip or direct-answer option allowed

---

### 2.5 Answer Evaluation
- AI evaluates:
  - Depth of reasoning
  - Conceptual correctness
- Incorrect reasoning triggers follow-up questions
- Correct reasoning advances the flow

---

### 2.6 Controlled Solution Reveal
- Final fix is revealed only after understanding is demonstrated
- Explanation must connect reasoning to the solution

---

### 2.7 Session Tracking (Prototype)
- Track per-session data:
  - Error type
  - Question progression
- No personal user data stored

---

## 3. Non-Functional Requirements
- Low latency responses
- Secure API communication
- Scalable backend architecture
- Simple UI for hackathon demo

---

## 4. Constraints
- Web-based prototype
- Single-session debugging flow
- Focus on clarity and learning effectiveness
