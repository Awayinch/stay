# Stay Agent Rules

This is a clean rebuild repo for Stay.

Do not copy secrets, databases, backups, uploads, memory data, or private worldbook content.
Do not add real API keys.
Do not add .env files except .env.example.
Do not add chat.db, sqlite files, uploads, backups, or Brain data.

Architecture:
- apps/web: React/Vite web chat
- apps/mobile: Capacitor Android app
- services/chat-api: synchronous chat API
- services/tool-api: async job API
- services/worker: background tool worker
- services/memory-gateway: memory system adapter
- packages/ui: shared UI
- packages/sdk: frontend API clients
- packages/native-bridge: Android/Web native bridge abstraction
- packages/tool-contracts: shared job/tool schemas

Principles:
- Main chat stays synchronous and responsive.
- Slow tools run asynchronously through jobs.
- ElevenLabs keys stay server-side.
- Android permissions go through native bridge abstractions.
- Prefer small PRs.
