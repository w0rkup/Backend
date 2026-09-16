# NestJS Backend Project Core Services

## Local Machine Infrastructure Quickstart

### 1. System Requirements
* Node.js Engine (v22+)
* Docker Desktop Environment

### 2. Quick Environment Setup
```bash
# Get runtime packages mapped locally
npm install --legacy-peer-deps

# Bootstrap variables configuration profiles
cp .env.example .env
```

### 3. Spin Up Infrastructure Layers
```bash
docker compose up -d
```

### 4. Running the Development Node App
```bash
npm run start:dev
```

### 5. Expected Endpoint Validation
Validate application connectivity via:
`GET http://localhost:3000/health`

Target Payload Response:
```json
{
  "status": "up",
  "timestamp": "2026-09-16T12:00:00.000Z",
  "uptime": 15.42
}
```
