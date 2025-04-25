# Reddit Tech News AI Agent

This project uses Google's Agent Development Kit (ADK) and Gemini 1.5 to create an AI agent that summarizes technology news from Reddit.

## Setup

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd adk_simple_agent
    ```
2.  **Set up Python environment:** (Using `uv` recommended)
    ```bash
    # Install uv (if needed)
    # pip install uv

    # Create virtual environment
    uv venv

    # Activate environment
    source .venv/bin/activate # Linux/macOS
    # .venv\Scripts\activate # Windows
    ```
3.  **Install dependencies:**
    ```bash
    uv pip install -r requirements.txt  # Or uv pip install -e . if using pyproject.toml
    ```
4.  **Configure Environment Variables:**
    - Copy `.env.example` to `.env` (or just create `.env`).
    - Add your `GOOGLE_API_KEY` to the `.env` file.
    ```
    GOOGLE_API_KEY="YOUR_API_KEY"
    ```

## Running the Agent

```bash
python main.py
```

This will start the FastAPI server. You can then interact with the agent using the ADK Development UI (details to be added) or a WebSocket client connecting to `ws://localhost:8080/ws/some_session_id`.

*(More details will be added as the project progresses)*
