# Stay Architecture

Stay is a personal AI companion system.

Core principle:

- Chat stays synchronous and responsive.
- Slow tools run asynchronously through jobs.
- Mobile native capabilities go through a bridge layer.
- Secrets stay server-side.
- Memory data stays outside Git.

## Workspaces

- apps/web: React/Vite web chat.
- apps/mobile: Capacitor Android app.
- services/chat-api: synchronous chat API.
- services/tool-api: async job API.
- services/worker: background job executor.
- services/memory-gateway: memory system adapter.
- packages/ui: shared UI components.
- packages/sdk: frontend API clients.
- packages/native-bridge: Android/Web native bridge abstraction.
- packages/tool-contracts: shared tool and job schemas.
