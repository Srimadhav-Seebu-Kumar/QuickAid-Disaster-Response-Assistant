# QuickAid Backend

This directory contains the backend API and server components for the QuickAid Disaster Response Assistant.

## Structure

- `api/` - REST API routes, controllers, and middleware
- `services/` - Business logic and external service integrations
- `database/` - Database models, migrations, and configurations
- `config/` - Server and application configuration files

## Getting Started

1. Install dependencies:
   ```bash
   npm install
   ```

2. Set up environment variables:
   ```bash
   cp .env.example .env
   ```

3. Run database migrations:
   ```bash
   npm run db:migrate
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

The server will be available at `http://localhost:8000`
