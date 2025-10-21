## SECTION 1 : PROJECT TITLE
WhatsEat – Multi-Agent Meal Discovery Assistant

---

## SECTION 2 : EXECUTIVE SUMMARY / PAPER ABSTRACT
WhatsEat brings together a LangGraph-powered reasoning backend and a React-based conversation interface to help users decide what to eat faster and with greater confidence. The system orchestrates specialised agents that gather context, reason about user intents, and assemble actionable meal suggestions. The result is a guided dialogue that feels natural while remaining grounded in curated culinary and dietary knowledge sources.

This parent repository acts as the umbrella for the full solution. It keeps the backend and frontend codebases aligned as Git submodules, captures system-wide documentation (such as the included architecture diagram), and provides a single entry point for deployment automation or release management. Teams can therefore clone one repository and immediately gain access to both halves of the stack, making collaboration across disciplines significantly smoother.

---

## SECTION 3 : CREDITS / PROJECT CONTRIBUTION

| Name         | Email              | Phone    | Student ID |
| ------------ | ------------------ | -------- | ---------- |
| Shang Jiakun | e1553372@u.nus.edu | 86696094 | A0329045E  |
| Ke Liwen     | e1553817@u.nus.edu | 80840573 | A0329490X  |
| Yu Guotao    | e1554269@u.nus.edu | 94458679 | A0329942U  |
| Liu Jiajia   | e1553327@u.nus.edu | 80387717 | A0329000X  |
| Yan Huaju    | e1553823@u.nus.edu | 89415266 | A0329496L  |

---

## SECTION 4 : VIDEO OF SYSTEM MODELLING & USE CASE DEMO
Embed a link to the latest walkthrough once it is available. A suggested placeholder is shown below—replace the URL and thumbnail with your final recording:

[![WhatsEat System Demo](http://img.youtube.com/vi/VIDEO_ID/0.jpg)](https://youtu.be/VIDEO_ID "WhatsEat System Demo")

---

## SECTION 5 : USER GUIDE

### Repository structure
- `What2Eat-frontend-agent-chat-ui/` – React application that renders the chat-driven meal discovery experience.
- `WhatsEat-backend-LangGraph-supervisor-py/` – LangGraph workflow coordinating the reasoning, retrieval, and action agents.
- `system design_final.png` – High-level architecture diagram for quick reference during onboarding.

### Cloning the project
```bash
git clone --recurse-submodules git@github.com:NUS-AIS-Practice-Modules/IRS-PM-2025-08-30-IS02PT-GRP-NeverStopCoding-WhatsEat.git
# If you do not have SSH access, swap the URL for the HTTPS variant before cloning.
```
If you already cloned the repository without submodules, run:
```bash
git submodule update --init --recursive --remote
```

### Frontend (React chat UI)
1. Navigate to the submodule directory: `cd What2Eat-frontend-agent-chat-ui`.
2. Follow the setup instructions in that repository's README (expected flow: install Node.js LTS, run `npm install`, then `npm run dev` or `npm start`).
3. Configure environment variables (e.g., API base URLs) as described in the submodule documentation.
4. Start the development server and ensure it can reach the backend endpoint.

### Backend (LangGraph orchestration)
1. Navigate to `WhatsEat-backend-LangGraph-supervisor-py`.
2. Create and activate a Python virtual environment (e.g., `python -m venv .venv && source .venv/bin/activate`).
3. Install the dependencies listed in the backend README (typically `pip install -r requirements.txt`).
4. Populate any required API keys, dataset paths, or tool credentials via environment variables or `.env` files.
5. Launch the LangGraph supervisor service (commonly via `python main.py` or a similar entrypoint) and confirm that the REST or websocket interface is reachable by the frontend.

### Running the full stack locally
1. Start the backend service and verify that the health endpoint responds.
2. Start the frontend development server and point it to the backend URL (default `http://localhost:<backend-port>`).
3. Open the UI in your browser, initiate a conversation, and monitor backend logs to validate agent behaviour.
4. Use the architecture diagram (`system design_final.png`) as a reference for debugging message flow across agents.

### Common maintenance tasks
- **Sync submodules:** `git submodule update --remote --merge` keeps frontend and backend pinned to their latest main branches.
- **Issue tracking:** Use the parent repository for cross-cutting issues; keep component-specific bugs within their respective submodule issue trackers.
- **Releases:** Tag this repository once both submodules reach the desired release commit, ensuring reproducible builds.

---

## SECTION 6 : PROJECT REPORT / PAPER
Store final documentation (project proposal, architecture write-up, testing evidence, etc.) inside a `ProjectReport/` directory in this repository. Link the primary PDF or paper here once published so reviewers can access it from the root README.

---

## SECTION 7 : MISCELLANEOUS
- Maintain any supplementary assets (datasets, slide decks, experiment logs) inside a `Miscellaneous/` folder alongside clear sub-folders.
- Use git-lfs or cloud storage links for large media files.
- Record retrospective notes or onboarding checklists here to keep institutional knowledge discoverable by new contributors.

---

**This [Machine Reasoning (MR)](https://www.iss.nus.edu.sg/executive-education/course/detail/machine-reasoning "Machine Reasoning") course is part of the Analytics and Intelligent Systems and Graduate Certificate in [Intelligent Reasoning Systems (IRS)](https://www.iss.nus.edu.sg/stackable-certificate-programmes/intelligent-systems "Intelligent Reasoning Systems") series offered by [NUS-ISS](https://www.iss.nus.edu.sg "Institute of Systems Science, National University of Singapore").**

**Lecturer: [GU Zhan (Sam)](https://www.iss.nus.edu.sg/about-us/staff/detail/201/GU%20Zhan "GU Zhan (Sam)")**

**zhan.gu@nus.edu.sg**
