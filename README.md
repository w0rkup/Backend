# NestJS Backend Project Core Services

## Local Machine Infrastructure Quickstart

### 1. System Requirements
* Node.js Engine (v22+)
* PostgreSQL Server (v15+) installed natively on your machine

### 2. Local Database Setup
1. Open your local PostgreSQL instance (via pgAdmin or psql shell).
2. Create a new database named `nest_backend_db`.
3. Ensure your local PostgreSQL user (`postgres`) has a password matching the configuration.

### 3. Quick Environment Setup
```bash
# Get runtime packages mapped locally
npm install --legacy-peer-deps

# Bootstrap variables configuration profiles
cp .env.example .env
```
*Note: Make sure to update the `DB_PASSWORD` value in your local `.env` file to match your native machine's PostgreSQL master password.*

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
  "timestamp": "2026-09-17T00:00:00.000Z",
  "uptime": 15.42
}
```
