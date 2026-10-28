Smart Pantry AI - Vercel project files

Keep this structure when uploading to GitHub:
app.py
requirements.txt
vercel.json
templates/auth.html
templates/index.html
static/app.js
static/style.css

Vercel environment variables:
SECRET_KEY = a long random secret value
GROQ_API_KEY = your Groq API key (keep it secret; never put it in code)
GROQ_MODEL = llama-3.3-70b-versatile (optional)

IMPORTANT: This Vercel configuration stores SQLite at /tmp/smart_pantry.db. Vercel's /tmp storage is temporary and can be reset, so account/pantry data is not reliably persistent. For a real public app with saved accounts and pantry items, use a persistent database (such as managed PostgreSQL) or deploy the included original project to Render with its persistent disk configuration.
