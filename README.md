# TDS-2![image](https://github.com/user-attachments/assets/4fd407a4-2564-463b-b582-b46b7ec6361f)
TDS GA Solver is a FastAPI-based web application designed to automate and assist with solving various Guided Assignment (GA) tasks. It supports multiple file formats, integrates with external APIs (GitHub and OpenAI), and is optimized for both local development and Vercel deployment. The tool is especially useful for educational use cases involving automated question solving, file processing, and assignment evaluation.
![TDS GA Solver UI](https://user-images.githubusercontent.com/your-id/filename.png)

## 🔧 Features

- 🧠 Handles multiple GA task types (GA1.x to GA5.x)
- 📁 Supports uploading files in various formats: `.png`, `.json`, `.pdf`, `.xlsx`, etc.
- 🌐 Web interface for user interaction (built with Bootstrap)
- 🤖 Integrates with OpenAI API (via proxy) for handling unknown or complex tasks
- 🛠 GitHub API integration for repository-related operations
- ☁️ Vercel-ready deployment configuration
- 🔁 CORS enabled for cross-origin support
- 🧩 Modular architecture for clean task separation

### Prerequisites

- Python 3.8+
- FastAPI
- Uvicorn
- GitHub API token (for repo operations)
- OpenAI API key (through proxy if needed)

### Installation

```bash
git clone https://github.com/yourusername/tds-ga-solver.git
cd tds-ga-solver
pip install -r requirements.txt
uvicorn app.main:app --reload This project is configured for deployment on Vercel.

To deploy:

Add vercel.json for routing.

Configure environment variables (OpenAI/GitHub keys) in the Vercel dashboard.

📤 APIs
POST /upload – Upload files and process based on GA type

POST /question – Submit a plain-text question

GET /status – Check service status

📚 Technologies Used
Backend: FastAPI, Uvicorn

Frontend: Bootstrap, HTML

APIs: OpenAI, GitHub

Deployment: Vercel
