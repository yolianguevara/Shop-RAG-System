# Usage — Shop-RAG-System

Local development quickstart

1. Copy .env.example to .env and populate your keys and settings (e.g., OPENAI_API_KEY).
2. Start the backend:
   - cd backend
   - npm install
   - npm run dev
3. Start the frontend:
   - cd frontend
   - npm install
   - npm run dev
4. Ingestion (example):
   - python3 scripts/ingest/ingest.py --data samples/products.csv --persist-dir ./chromadb

Notes
- Do not commit API keys. Use .env locally or configure GitHub Secrets for CI.
- The repository uses a local Chroma instance (persist directory) by default in examples.
