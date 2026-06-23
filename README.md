During Deployment on Streamlit Cloud
When you are actually deploying your project on Streamlit Community Cloud, follow these quick steps to make sure your README instructions match your actions:

Go to Your App Console: Once your app starts building on Streamlit, click the "Manage App" button at the bottom-right corner.

Open Advanced Settings: Click the three dots (menu) next to your app status and open Settings > Secrets.

Paste the Config: Copy your exact key structure into the text panel and hit save:

Ini, TOML
GEMINI_API_KEY = "your_actual_new_gemini_api_key_here"
Your app will automatically securely grab the key from its backend environment variable vault, restart itself cleanly, and go live!
Ensure that your .streamlit/secrets.toml fileis added to your local .gitignore file before pushing your codebase to the public repository.
