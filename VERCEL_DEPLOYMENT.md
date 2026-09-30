# Deploy Aary's portfolio to Vercel

This package is ready for a same-origin deployment: the frontend calls `POST /api/chat`, and `server.py` exposes that exact FastAPI route. Vercel recognizes the root `server.py` entrypoint automatically.

## 1. Create the repository

1. Extract this project.
2. Create a new GitHub repository.
3. Upload every included file and folder, including `public/`, `server.py`, `requirements.txt`, `vercel.json`, and `.python-version`.
4. Do **not** upload a real `.env` file.

## 2. Import into Vercel

1. Sign in to Vercel and select **Add New → Project**.
2. Import the GitHub repository.
3. Leave **Framework Preset** as **Other** or allow automatic detection.
4. Keep the project root as the repository root.
5. Do not add a custom Build Command or Output Directory.

## 3. Add the private API key

Before deploying, open **Project Settings → Environment Variables** and add:

- `GEMINI_API_KEY`: your key from Google AI Studio.
- `GEMINI_MODEL`: `gemini-3.5-flash` (optional because this is already the default).
- `ALLOWED_ORIGINS`: `*` for the simplest same-origin deployment. You can later replace it with your production URL.

Apply the variables to **Production**, **Preview**, and **Development** as needed. Never put the real key in HTML, GitHub, or `vercel.json`.

## 4. Deploy and verify

1. Select **Deploy**.
2. Open `https://YOUR-PROJECT.vercel.app/api/health`.
3. Confirm the response contains `"status":"ok"` and `"geminiConfigured":true`.
4. Open the site, select **Ask anything**, and send a question such as “What projects has Aary built?”
5. If you add or change an environment variable, redeploy so the new value is applied.

## Local test

```bash
python -m venv .venv
# macOS/Linux
source .venv/bin/activate
# Windows PowerShell: .venv\Scripts\Activate.ps1
pip install -r requirements.txt
cp .env.example .env
# Put your real GEMINI_API_KEY in .env
uvicorn server:app --reload
```

Then visit `http://127.0.0.1:8000`, check `http://127.0.0.1:8000/api/health`, and test **Ask anything**.

## Troubleshooting

- `geminiConfigured:false`: add `GEMINI_API_KEY` in Vercel and redeploy.
- HTTP 502 from `/api/chat`: inspect **Vercel → Project → Logs**; confirm the model name and API-key permissions.
- Frontend loads but chat says the server is offline: confirm this is one Vercel project and the frontend still calls `/api/chat`.
