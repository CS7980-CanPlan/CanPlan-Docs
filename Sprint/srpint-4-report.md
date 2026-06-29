# CanPlan 2.0 — Sprint Progress Report

CS7980 | Team CanPlan | Week 7 - Week 8

---

## 1. Sprint Leadership

Sprint 3 Leader: Siyi Pan
Sprint 4 Leader: Siyi Pan

---

## 2. What We Accomplished This Sprint

**Theodore Pei：**

- createAiTask — AI task-preview feature (RAG over Bedrock KB) — 12h
 New Lambda + GraphQL input/mutation/types, resolver wiring, KB+Bedrock+DynamoDB IAM construct, prompt + parser helpers, `stepsService` / `task.persistTask` refactors, plan/spec docs, tests. 
- Per-owner task ordering (`updateTaskOrder`). - 7h
 `Task.order` field + `updateTaskOrder` mutation, plus a data migration to backfill `order` onto every existing task (schema, tasks handler, `task.ts`/`batch`/`taskCascade`, heavy tests). 
- Knowledge Base → S3 Vectors migration + IAM fix — 3h
 Re-backed the KB with S3 Vectors once the SCP allowed it; debugged and fixed an `s3vectors` 403 by making the KB depend on the KB role's inline policy.
- Research paper — Week 9 summary + gap review — 3h
 Reviewed the paper against the actual build and wrote the single-vs-multi-agent reflection.
- Team meeting — 2h


**Langze An：**

- Set up an individual AWS development environment for backend development and testing — 2h
- Added admin features and web portal admin pages — 5h
- Developed the assignment and schedule features — 15h
- Tested backend functionality and reviewed pull requests — 5h
- Attended backend meetings to discuss testing strategy and backend repository development — 5h
- Fixed bugs found during development and testing — 3h
- Built category pages for the mobile app and added simple mode for the all-task view — 5h

**Siyi Pan：**

- Calendar Page — redesigned layout and visual hierarchy, added new components, and improved mobile responsiveness. - 4h 
- Settings Page — designed the interface structure and organized key settings functions for mobile - 6h 
- Wrote the design doc for the Caregiver / Support-Person Portal — covering the role-based entry flow, caregiver auth screens, caregiver home dashboard, patient linking, and how existing patient screens will be reused under caregiver context. - 4h
- Participated in team meetings and contributed to code reviews. - 3h
- Led the sprint - facilitated team meetings, coordinated sprint goals, and drove code reviews. - 3h

**Liecheng Jiang：**

- Implemented the mobile login screen (account flow UI + form validation, wired to the auth endpoints) — 6h
- Built the all-tasks module on the mobile app. - 6h
- Reworked the mobile UI for better usability — refined interaction patterns and layout so the flows feel more intuitive. - 5h
- Prepared and ran the Wednesday midterm demo (frontend walkthrough, demo flow rehearsal). - 2h
- Scoped the Setting page and Calendar views over the weekend — drafted layout and interaction plan ahead of implementation. - 3h
- Research paper: reviewed Sprint 4 frontend build against the paper framework, drafted the weekly summary and single-vs-multi-agent reflection. - 4h
- Supervisor meetings (Hao + Lino) and team standup. - 2h

**Yifan Wei：**

- API testing for newly added backend endpoints (createAiTask, updateTaskOrder, assignment/schedule features) — 6h
- Coordinated with Theodore on AI task feature testing, documented findings and edge cases — 3h
- Research paper: reviewed Sprint 4 build against paper framework, drafted weekly summary and single-vs-multi-agent reflection section — 4h
- Bruno collection updates: added new test cases for newly available endpoints, updated environment variables after backend changes — 2h
- Supervisor meetings (Hao + Lino) and team standup — 2h
- Sprint 5 lead responsibilities: facilitated team meetings, tracked task progress, updated GitHub project board — 3h


---

## 3. Retrospective

**What went well:**

- The development process is on track
- The setup process went smoothly
- Team communication was clear

**What could be improved:**

- None

---

## 4. Plan for Next Sprint

Sprint 4 Leader: Siyi Pan

**Goals:**

- AI report endpoint — build the AI-generated report interface.
- RAG optimization *(Pending — depends on the report endpoint's progress)* — tune retrieval / generation quality once the report endpoint is in place.
- Set up support person APIs and permissions
- Develop offline mode for the mobile app
- Test support person APIs and permission flows once available
- Research paper: finalize experimental design section and research question before Lino meeting
- Coordinate mid-point demo prep with Paul
- Begin implementation based on the design doc — starting with the welcome screen, caregiver auth flow, and mock data setup.
- Add the Create AI Task feature into the caregiver portal uiux design.
- Implement the Calendar feature on the mobile app, building on Michael's completed backend (assignment/schedule) endpoints
- Coordinate with Siyi on the support-person UI design
- Begin Setting page implementation based on this week's scoped plan


**Task assignments:**

- Yifan Wei — database design and generate test data
- Michael An — infrastructure and backend API development
- Theodore Pei — AI system design
- Siyi Pan — UI/UX design
- Liecheng Jiang — mobile app and web portal frontend development

---

## 5. Blockers & Concerns

- None

---

## 6. Track Hours

**Working Hours:**

- Yifan Wei —  20 hours
- Michael An — 40 hours
- Theodore Pei — 27 hours
- Siyi Pan — 20 hours
- Liecheng Jiang — 28 hours

**Meting Hours:**

- Hao - 30 mins/week
- Lino - 30 mins/week
- Group - 3 hours+/week

---

## 6. Links

- GitHub Repository: https://github.com/orgs/CS7980-CanPlan