# SaaS Product Requirements Document (PRD)

**Phase:** 4 (AI Product Company / SaaS)
**Status:** Active Execution Playbook

---

## 1. Feature Name: [Insert Name]
**Target Launch Date:** [Date]
**Lead Engineer:** [Name]
**Product Manager:** [Name - Initially Founder]

## 2. The Problem Statement
Do not build features because they are "cool." Build features because users are churning or prospects are failing to convert.
*   **User Problem:** (What is the user trying to achieve, and why is it currently hard?)
*   **Business Problem:** (Why is it important for us to solve this? e.g., Reduces churn, increases expansion revenue).

## 3. The "AI-Native" Approach
If this is an AI SaaS feature, we must define the AI contract:
*   **The Model:** Which LLM/Model is best for this? (e.g., GPT-4 for reasoning, Claude 3 for large context, local models for speed/privacy).
*   **The Prompt Strategy:** How are we retrieving context? (RAG, few-shot prompting, fine-tuning).
*   **Fallback:** What happens when the AI hallucinated or the API times out? (The UI must fail gracefully).

## 4. User Stories & Acceptance Criteria
*As a [persona], I want to [action] so that [outcome].*

| User Story | Acceptance Criteria (Definition of Done) |
| :--- | :--- |
| As a user, I want to upload a CSV. | File size limit is 50MB. Only accepts .csv. Validates headers. |
| As a user, I want the AI to summarize it. | Summary generates in < 5 seconds. Shows loading state. |

## 5. Scope & Out of Scope
Scope creep is the death of SaaS velocity.
*   **In Scope for v1:** [List 3-5 core things]
*   **Out of Scope (Save for v2):** [List things we explicitly will NOT build yet]

## 6. Go-To-Market / Launch Strategy
A feature is not done when it is deployed. It is done when users are actively using it.
*   [ ] Update Changelog.
*   [ ] Send targeted email to users who requested this.
*   [ ] Create a quick Loom tutorial for the Help Center.
