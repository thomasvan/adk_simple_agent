# Reddit Tech News AI Agent - Tasks

## Project Tasks - 2025-04-25

*(Revised Plan: Focus on Core Agent -> Mock Data -> Real Data)*

### Phase 1: Minimal ADK Agent & UI Setup

- [ ] Set up basic project structure (agent/, main.py, .env, pyproject.toml, README.md)
- [ ] Initialize uv package management (`pyproject.toml`)
- [ ] Add initial dependencies (google-adk, google-generativeai) to `pyproject.toml`
- [ ] Set up environment variables configuration (`.env` for API keys)
- [ ] Create `main.py` as the ADK FastAPI entry point
- [ ] Create basic `agent/agent.py` with minimal ADK agent structure
- [ ] Configure Google ADK environment and Gemini 1.5 model access
- [ ] Implement a simple interaction loop in the agent
- [ ] Start the ADK Development UI and test basic interaction
- [ ] Create test environment with local ADK installation

### Phase 2: Mock Data Integration & Summarization

- [ ] Define Python data structures for mock Reddit posts
- [ ] Create sample mock data (e.g., in a JSON file or Python dict)
- [ ] Develop initial summarization prompts for Gemini
- [ ] Implement summarization logic in `summarizer/gemini_summarizer.py` using mock data
- [ ] Integrate the summarizer tool/function into the ADK agent
- [ ] Display summaries generated from mock data in the ADK UI
- [ ] Add basic caching for summarization results (optional, consider Redis later)
- [ ] Create basic unit tests for the summarization logic with mock data
- [ ] Create evaluation metrics for summary quality (placeholder)

### Phase 3: Reddit Crawler & Database Implementation

- [ ] Create `crawler/reddit_crawler.py` module
- [ ] Add PRAW dependency to `pyproject.toml`
- [ ] Implement authentication with Reddit API (using `.env`)
- [ ] Configure target subreddits
- [ ] Implement post fetching logic with filters
- [ ] Add rate limiting and error handling for PRAW
- [ ] Define database schema for posts and summaries in `data/models.py`
- [ ] Set up SQLite for development
- [ ] Implement data models and basic ORM interaction (e.g., SQLAlchemy)
- [ ] Implement logic to store crawled posts in the database
- [ ] Modify agent to fetch data from DB instead of mock source
- [ ] Create unit tests for crawler functionality
- [ ] Create unit tests for basic database operations

### Phase 4: Refinement, API, UI & Deployment

- [ ] **API Development:**
    - [ ] Configure ADK's built-in FastAPI server further
    - [ ] Create RESTful API endpoints for summaries (list, get, search)
    - [ ] Implement pagination and filtering for API
    - [ ] Add API error handling and logging
    - [ ] Create OpenAPI documentation for API
    - [ ] Set up rate limiting for API endpoints
    - [ ] Implement authentication for potential admin functions
    - [ ] Create unit tests for API endpoints
- [ ] **Web Portal / ADK UI Integration:**
    - [ ] Configure ADK Development UI further (monitoring, etc.)
    - [ ] Create a simple web portal (e.g., using Streamlit, Flask, or basic HTML/JS) that calls the FastAPI backend
    - [ ] Add search and filtering to the web portal
    - [ ] Create feedback mechanism for summary quality
    - [ ] Implement responsive design (optional)
- [ ] **Database Enhancements:**
    - [ ] Set up PostgreSQL for production (optional)
    - [ ] Create migration scripts (if using PostgreSQL)
    - [ ] Add data validation and sanitization
    - [ ] Implement database backup strategy
- [ ] **Deployment & Operations:**
    - [ ] Set up production logging and monitoring
    - [ ] Configure CI/CD pipeline
    - [ ] Create Docker container configuration (local, staging, production)
    - [ ] Implement scheduled jobs for regular crawling
    - [ ] Set up health checks and alerts
    - [ ] Create backup and recovery procedures
- [ ] **Documentation:**
    - [ ] Write comprehensive API documentation
    - [ ] Create user guide for the application
    - [ ] Document system architecture
    - [ ] Create developer guide for contributions
    - [ ] Document testing procedures
    - [ ] Create ADK Development UI usage guide
    - [ ] Create troubleshooting guide

## Discovered During Work

<!-- New tasks discovered during development will be added here -->

## Completed Tasks
<!-- Tasks will be moved here when completed with date -->