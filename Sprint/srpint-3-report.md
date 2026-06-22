# CanPlan 2.0 — Sprint Progress Report

CS7980 | Team CanPlan | Week 7 - Week 8

---

## 1. Sprint Leadership

Sprint 3 Leader: Siyi Pan
Sprint 4 Leader: Siyi Pan

---

## 2. What We Accomplished This Sprint

**Theodore Pei：**

- Set up the frontend clients (mobile app and web portal) to integrate with the backend APIs.
- Created user groups and assigned permissions for backend API access.
- Implemented and tested authentication flows using Cognito.
- Migrated the AI step-generation pipeline from the local prototype to AWS using a Bedrock Knowledge Base.
- Vendored the HealthLink BC corpus and wrote a build script that converts the seed data into a per-passage S3 layout for ingestion.
- Provisioned the Knowledge Base through CDK with Titan v2 embeddings, backing it with OpenSearch Serverless after S3 Vectors turned out to be blocked by an SCP.
- Split the Knowledge Base into a dedicated us-east-1 stack to handle the cross-region setup.
- Implemented the `generateTaskSteps` Lambda and a shared Bedrock KB client that retrieve from the Knowledge Base and return cited, plain-language steps over GraphQL.

**Langze An：**

- Set up the frontend clients (mobile app and web portal) to integrate with the backend APIs.
- Created user groups and assigned permissions for backend API access.
- Implemented and tested authentication flows using Cognito.

**Siyi Pan：**

- Finished UI/UX design for the app in iOS version.

**Liecheng Jiang：**

- Prepared the mobile app.

**Yifan Wei：**

- Help Langze An test API 

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

- Be ready for the Week 4 demo.
- Complete the UX design for iPad and Android app pages.
- Upgrade the mobile app pages.
- Add test data for the database.

**Task assignments:**

- Yifan Wei — database design and generate test data
- Michael An — infrastructure and backend API development
- Theodore Pei — AI system design
- Siyi Pan — UI/UX design
- Liecheng Jiang — mobile app and web portal frontend development

---

## 5. Blockers & Concerns

- [None — remove if no blockers]

---

## 6. Track Hours

**Working Hours:**

- Yifan Wei —  12 hours
- Michael An — 13 hours
- Theodore Pei — 12 hours
- Siyi Pan — 12 hours
- Liecheng Jiang — 13 hours

**Meting Hours:**

- Hao - 30 mins/week
- Lino - 30 mins/week
- Group - 3 hours+/week


## 6. Links

- GitHub Repository: https://github.com/orgs/CS7980-CanPlan