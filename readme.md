# Project Creator API

A Flask-based API that generates project structures and code using OpenAI and Swarm. The API creates files, manages directories, and packages projects as ZIP files based on user input.

Features:
- Project Structure Creation: Automatically generates project directories and files.
- Code Generation: Creates code based on the specified language and framework.
- File Management: Supports creating, deleting, and managing project files.
- Downloadable ZIP Files: Packages the project as a ZIP file for easy download.
- CORS Support: Allows cross-origin requests.
- Environment Variables: Loads API keys from `.env.local`.

Requirements:
- Python 3.x
- Flask
- Flask-CORS
- OpenAI Python client
- Swarm library
- python-dotenv

Installation:
1. Clone the repository:
   git clone <your-repo-url>
   cd <your-repo-folder>

2. Install dependencies:
   pip install -r requirements.txt

3. Set up environment variables in `.env.local`:
   OPENAI_API_KEY=<your-openai-api-key>

4. Run the application:
   python app.py

API Usage:
Create a Project:
POST /create_project

Request:
```json
{
  "project_description": "A web app using HTML, CSS, JavaScript",
  "project_name": "my_web_app"
}
```
Response:
`Returns a ZIP file of the generated project.`

License:
This project is licensed under the MIT License.
