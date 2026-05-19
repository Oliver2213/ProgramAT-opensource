I want you to fully set up and run this repository locally for me.

Important constraints:
- DO NOT try to acquire API keys or create accounts for me.
- I have ALREADY created and filled in backend/.env.
- Do NOT overwrite or recreate backend/.env.
- You may read values from backend/.env when needed.
- You ARE allowed to:
  - create/edit files
  - install dependencies
  - create virtual environments
  - configure ngrok
  - start servers
  - run commands
  - debug issues
  - modify configuration files other than backend/.env
  - verify the server is working

Your goal:
1. Read the README carefully.
2. Set up the backend environment automatically.
3. Use the existing backend/.env configuration.
4. Validate that required environment variables exist.
5. If something is missing from backend/.env, tell me exactly which variable is missing instead of recreating the file.
6. Install ngrok if it is missing.
7. Configure ngrok with my authtoken if needed.
8. Start the backend server.
9. Start ngrok forwarding for port 8080.
10. Extract the public forwarding URL automatically.
11. Convert the URL from https:// to wss://.
12. Print the exact websocket URL I should paste into the app settings.
13. If anything fails, debug and fix it automatically.

Implementation details:
- Use Python 3.11 if required.
- Create backend/.venv if it does not exist.
- Install dependencies from requirements.txt.
- Use the repository’s documented commands whenever possible.
- Prefer automated shell commands over asking me to do manual setup.
- Explain briefly what you are doing at each major step.
- If a command fails, investigate logs and retry with fixes.
- Keep going until the websocket server is reachable through ngrok.

Important:
- Never overwrite backend/.env.
- Never expose secrets in logs or output.
- Preserve all existing configuration values.

When the server is running:
- Verify the backend is listening on port 8080.
- Verify ngrok forwarding works.
- Show me:
  - local server address
  - ngrok forwarding address
  - final wss:// websocket URL

Assume I prefer autonomous behavior unless a secret/token is strictly required from me.

Do not ask me to debug terminal issues manually unless you have already attempted at least two fixes yourself.