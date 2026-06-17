# Project Title
Notification Service (Dummy App)

## Overview
This repository contains a dummy notification service used to test a GitHub tech stack extractor. It simulates a minimal event-driven microservice in a ride-sharing context and is intentionally lightweight for tooling and parsing validation.

## Features
- Minimal Node.js service bootstrap for quick setup
- Environment variable loading via `.env`
- Kafka integration placeholder for consuming notification events
- Development mode with auto-reload support (`nodemon`)
- Simple, extractor-friendly project layout and metadata

## Tech Stack
- Frontend: React (planned for dashboard/admin UI)
- Backend: Node.js, JavaScript (CommonJS), FastAPI (planned integration service), Python (planned data-processing utilities)
- Database: PostgreSQL (planned)
- DevOps: Docker (planned containerization), AWS (planned deployment target), GitHub Actions (planned CI/CD)
- Testing: Jest (planned for unit/integration tests)

## Project Structure
```text
notification-service/
├── .env
├── .gitignore
├── package.json
└── src/
    ├── app.js
    └── kafkaConsumer.js
```

## Installation
1. Clone the repository.
2. Navigate to the project directory.
3. Install dependencies:

```bash
npm install
```

## Usage
Start in production mode:

```bash
npm start
```

Start in development mode:

```bash
npm run dev
```

Run the Kafka consumer placeholder directly (optional):

```bash
node src/kafkaConsumer.js
```

## API Endpoints (if applicable)
No HTTP API endpoints are currently implemented in this dummy service.

## Environment Variables
Create a `.env` file in the project root with the following variable:

```env
KAFKA_BROKER=localhost:9092
```

Notes:
- `KAFKA_BROKER` is read by the app and logged at startup.

## Testing
This repository currently includes a placeholder test command:

```bash
npm test
```

Current behavior:
- Returns a placeholder message (`No tests yet`).

## Roadmap
- Add real Kafka consumer and producer flow
- Implement notification delivery adapters (email/SMS/push)
- Add REST endpoints for health and metrics
- Introduce automated tests (unit and integration)
- Add Docker support and CI workflow with GitHub Actions
- Add PostgreSQL-backed notification persistence

## License
MIT License