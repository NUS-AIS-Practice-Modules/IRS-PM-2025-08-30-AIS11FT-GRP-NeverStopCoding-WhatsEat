### [ Practice Module ] PRACTICE MODULE BRIEFING for Certificate in Intelligent Reasoning Systems (IRS)

**[ Naming Convention ]** IRS-PM-2025-08-30-AIS11FT-GRP-NeverStopCoding-WhatsEat

## SECTION 1 : PROJECT TITLE
### WhatsEat - Multi-agent Powered Restaurant Recommendation Assistant
![home](assets/home.png)


<p align="center">
  <em>An intelligent multi-agent system that delivers personalized restaurant recommendations by conversational UI</em>
</p>

### Tech-Stack

<p align="left">
  <em>Frontend </em>
</p>
<p align="left" style="display:flex; gap:20px; flex-wrap:wrap; align-items:center;">
  <a href="https://reactjs.org/" target="_blank"><img src="assets/icons/react.svg" alt="React" width="40" height="40"></a>
  <a href="https://www.typescriptlang.org/" target="_blank"><img src="assets/icons/typescript.svg" alt="TypeScript" width="40" height="40"></a>
</p>


<p align="left">
  <em>Backend</em>
</p>
<p align="left" style="display:flex;gap:20px;flex-wrap:wrap;align-items:center;">
  <a href="https://openai.com/" target="_blank"><img src="assets/icons/openai.svg" alt="OpenAI" width="40" height="40"></a>
  <a href="https://www.langgraph.com/" target="_blank"><img src="assets/icons/langgraph.svg" alt="LangGraph" width="40" height="40"></a>
  <a href="https://www.langsmith.com/" target="_blank"><img src="assets/icons/langsmith.svg" alt="LangSmith" width="40" height="40"></a>
  <a href="https://www.langchain.com/" target="_blank"><img src="assets/icons/langchain.svg" alt="LangChain" width="40" height="40"></a>
  <a href="https://neo4j.com/" target="_blank"><img src="assets/icons/neo4j.svg" alt="Neo4j" width="40" height="40"></a>
  <a href="https://pinecone.io/" target="_blank"><img src="assets/icons/pinecone.svg" alt="Pinecone" width="40" height="40"></a>
  <a href="https://www.python.org/" target="_blank"><img src="assets/icons/python.svg" alt="Python" width="40" height="40"></a>
  <a href="https://maps.google.com/" target="_blank"><img src="assets/icons/map.svg" alt="Google Map" width="40" height="40"></a>
  <a href="https://www.youtube.com/" target="_blank"><img src="assets/icons/youtube.svg" alt="YouTube" width="40" height="40"></a>
</p>

---

## SECTION 2 : EXECUTIVE SUMMARY / PAPER ABSTRACT

Amid a shift from static “nearby + rating” lists to context-aware personalization, Whats'Eat presents an explainable, multi-agent restaurant recommendation system. Built on a Supervisor–Agents graph using *LangGraph*, the system concurrently orchestrates an Places Agent and a User Profile Agent (both idempotent) to gather geographic evidence and lightweight behavioral signals. A KG-based RAG Recommender Agent then fuses a *Neo4j* knowledge graph with *Pinecone* vector retrieval for candidate recall and multi-factor ranking, and a Summarizer Agent produces a UI-ready {cards, rationale} JSON payload. Engineering contributions include contract-first JSON flows, idempotent tool calls with retries, field-masked API usage, pagination-stable ingestion, and a React frontend for map/route and card rendering. Functional tests cover places, profile, RAG, and summarization paths; in real use cases the system improves preference fit and explanation clarity over non-retrieval conversational baselines. This work contributes: 

- **A parallel-yet-controlled multi-agent orchestration pattern**
- **An evidence that hybrid KG + vector retrieval is effective for local-services recommendations**
- **A strict output contract with reproducible implementation details, providing a foundation for broader local-service scenarios.**

​		


<p align="center">
  <img alt="demo1" src="assets/demo_langgraph.gif"> 
</p>

<p align="center">
  <em>LangGraph-Supervisor Multi-agent Monitoring</em>
</p>

---

## SECTION 3 : CREDITS / PROJECT CONTRIBUTION

| Name         | Email              | Phone    | Student ID |
| ------------ | ------------------ | -------- | ---------- |
| Ke Liwen     | e1553817@u.nus.edu | 80840573 | A0329490X  |
| Shang Jiakun | e1553372@u.nus.edu | 86696094 | A0329045E  |
| Liu Jiajia   | e1553327@u.nus.edu | 80387717 | A0329000X  |
| Yu Guotao    | e1554269@u.nus.edu | 94458679 | A0329942U  |
| Yan Huaju    | e1553823@u.nus.edu | 89415266 | A0329496L  |

## SECTION 4 : VIDEO OF SYSTEM MODELLING & USE CASE DEMO

[![video_cover](assets/video_cover.png)](https://www.youtube.com/watch?v=kfHtMgUZ3Eo)

Video Link (YouTube): *https://www.youtube.com/watch?v=kfHtMgUZ3Eo*

---

## SECTION 5 : USER GUIDE

`Refer to appendix <Installation & User Guide> in project report at Github Folder: ProjectReport`

<p align="center">
  <img src="assets/demo_current_location.gif" alt="demo_card" width="350">
  <img src="assets/demo_specific_location.gif" alt="demo_map" width="350">
</p>

<p align="center">
  <em>Recommend by Current Location (Left) & Specific location (Right) </em>
</p>

<p align="center">
  <img src="assets/demo_card.gif" alt="demo_card" width="350">
  <img src="assets/demo_map.gif" alt="demo_map" width="350">
</p>

<p align="center">
  <em>Restaurants Card Display (Left) & Interactive Map (Right) </em>
</p>



---
## SECTION 6 : PROJECT REPORT / PAPER

`Refer to project report at Github Folder: ProjectReport`

**Recommended Sections for Project Report / Paper:**

- Executive Summary / Paper Abstract
- Business Problem Background
- Market Research
- Project Objectives & Success Measurements
- Project Solution (To detail domain modelling & system design.)
- Project Implementation (To detail system development & testing approach.)
- Project Performance & Validation (To prove project objectives are met.)
- Project Conclusions: Findings & Recommendation
- Appendix of report: Project Proposal
- Appendix of report: Mapped System Functionalities against knowledge, techniques and skills of modular courses: MR, RS, CGS
- Appendix of report: Installation and User Guide
- Appendix of report: 1-2 pages individual project report per project member, including: Individual reflection of project journey: (1) personal contribution to group project (2) what learnt is most useful for you (3) how you can apply the knowledge and skills in other situations or your workplaces
- Appendix of report: List of Abbreviations (if applicable)
- Appendix of report: References (if applicable)

---
## SECTION 7 : MISCELLANEOUS

`Refer to Github Folder: Miscellaneous`

