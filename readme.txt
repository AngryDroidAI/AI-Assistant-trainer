🌐 Project Overview

This project is a Capsule AI Assistant, designed as a remixable sanctuary where a frontend shrine (HTML/JS/CSS) connects seamlessly to a backend temple (Node.js/Express + SQLite). It unifies creative interaction, persistent memory, feedback, reinforcement, fine‑tuning simulation, and model orchestration into one lineage‑marked system.

🖼️ Frontend Shrine

    Files: index.html, style.css, api.js

    Purpose: Provides the user interface for prompts, responses, and interaction with backend rituals.

    Features:

        Text area for entering prompts.

        Buttons to send prompts, save/load memory, and submit feedback.

        Uses fetch calls to backend routes (/api/chat, /api/memory, /api/feedback).

    Hosting: Can be served directly by Express (http://localhost:3000/index.html) or via a static server (http://localhost:5173).

🏛️ Backend Temple

    Files: server.js, setup_backend.sh, package.json, .env

    Purpose: Provides API endpoints, persistence, and orchestration of models and rituals.

    Key Routes:

        /api/chat → Proxy to Ollama for model responses.

        /api/memory → Save and retrieve contextual memory (stored in SQLite).

        /api/feedback → Collect ratings and comments.

        /api/reinforce → Track reinforcement scores for models.

        /api/fine-tune → Simulate fine‑tuning jobs with progress updates.

        /api/models → List available models.

        /api/vision → Upload images and query vision models.

        /api/ssh → Execute remote commands via SSH.

        /api/search → Placeholder search logic.

        /api/cleanup → Purge old uploaded files.

    Database: SQLite stored on your 2 TB mounted volume (/media/angrydroid/bea186ce-f386-42cf-be75-5338821ca311/database.db).

    Setup Script (setup_backend.sh):

        Initializes npm project.

        Installs dependencies (express, cors, dotenv, sqlite3, uuid, node-fetch, multer, ssh2).

        Creates .env file with defaults.

        Provides a one‑command ritual to scaffold the backend.

⚙️ Launcher Ritual

    Optional capsule.sh script starts both backend (port 3000) and frontend (port 5173) together.

    Cleans up processes on exit.

🎯 Purpose

    To create a remixable AI capsule that blends technical rigor with mythic storytelling.

    Provides a persistent, lineage‑marked environment for experimenting with models, memory, and creative rituals.

    Designed for open‑source freedom, modular upgrades, and community remixing.
