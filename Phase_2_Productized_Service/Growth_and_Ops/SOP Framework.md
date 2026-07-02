# Solo SOP Framework

**Phase:** 1 & 2 (Freelancer → Productized Service)
**Status:** Active Execution Playbook

---

## 1. Why a Solo Creator Needs SOPs
As a solo operator, your greatest enemy is context switching and repetitive admin work. Standard Operating Procedures (SOPs) allow you to turn on "autopilot" for delivery, increasing your effective hourly rate and reducing burnout.

SOPs are the prerequisite for Phase 3 (Agency). You cannot hire someone if you don't have instructions for them to follow.

## 2. Core Solo SOPs to Build Immediately

### A. The Tech Boilerplate SOP
Never start a React/Next.js project from scratch.
- Maintain a highly opinionated GitHub template repository.
- **Includes:** Tailwind setup, standard folder structure, Prettier/ESLint configs, basic auth routes, and reusable UI components (buttons, modals).
- **Goal:** Run `npx create-next-app -e your-repo-url` and be ready to code business logic in 5 minutes.

### B. The Figma Starter File SOP
Never start a design from a blank canvas.
- Maintain a master Figma file with your typography scales, color variables, grid systems, and standard UI components.
- Duplicate this file for every new client project.

### C. Client Onboarding SOP
Automate the friction of starting a project.
1. Client signs proposal & pays deposit.
2. Zapier triggers an automated email with a link to an Onboarding Questionnaire (Typeform).
3. Questionnaire asks for: Brand assets, API keys, domain access, competitor references.
4. Zapier creates a client folder in Google Drive and a project in Linear/Notion.

### D. The Weekly Update SOP
Client anxiety is the number one cause of scope creep. Kill anxiety with predictable communication.
- **Every Friday at 4 PM:** Send the standard update email.
  - *What was completed this week.*
  - *What is blocked / needs their approval.*
  - *What is scheduled for next week.*

## 3. How to Document an SOP
When documenting a process for your future Phase 3 hires, use this format:
1. **Trigger:** What causes this SOP to start? (e.g., Client pays invoice).
2. **Tools Required:** What software is needed?
3. **Step-by-Step Actions:** Bulleted list of clicks, code commands, and copy-paste templates.
4. **Definition of Done:** How do we know this process was completed successfully?

## 4. The "Rule of 3"
If you find yourself doing the exact same manual task 3 times, you must pause and turn it into an SOP, an automation, or a boilerplate.
