# Task Manager Application

A full-stack task management application built with FastAPI backend and HTML/CSS/JavaScript frontend.

## Features

- 🔐 User authentication (register, login, JWT)
- ✅ Create, read, update, and delete tasks
- 🗂️ Task prioritization and categorization
- 📅 Due date scheduling and tracking
- 🔄 Real-time updates with modern UI
- 📱 Responsive design for mobile and desktop
- 📊 API documentation with Swagger UI

## Tech Stack

### Backend
- FastAPI - Modern, fast web framework for building APIs
- SQLAlchemy - SQL toolkit and ORM
- Pydantic - Data validation and settings management
- JWT - Token-based authentication
- SQLite - Database (can be easily swapped for PostgreSQL, MySQL, etc.)

### Frontend
- HTML5 / CSS3 / JavaScript (ES6+)
- Tailwind CSS - Utility-first CSS framework
- Axios - Promise-based HTTP client

## Getting Started

### Prerequisites
- Python 3.8+
- pip (Python package installer)

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/task-manager.git
cd task-manager
```

2. Create and activate a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install fastapi uvicorn sqlalchemy pydantic python-jose[cryptography] passlib[bcrypt] python-multipart
```

4. Run the application
```bash
uvicorn main:app --reload
```

5. Open your browser and navigate to:
   - Frontend: Open `index.html` in your browser
   - API Documentation: http://localhost:8000/docs

## Project Structure

```
task-manager/
├── main.py           # FastAPI application and endpoints
├── models.py         # SQLAlchemy models
├── schemas.py        # Pydantic schemas for validation
├── database.py       # Database connection configuration
├── index.html        # Frontend application
├── task_manager.db   # SQLite database
└── README.md         # Project documentation
```

## API Endpoints

| Method | Endpoint          | Description                   | Authentication Required |
|--------|-------------------|-------------------------------|-------------------------|
| POST   | /token            | Login and get access token    | No                     |
| POST   | /users/           | Register new user             | No                     |
| GET    | /users/me/        | Get current user info         | Yes                    |
| POST   | /tasks/           | Create new task               | Yes                    |
| GET    | /tasks/           | Get all user tasks            | Yes                    |
| GET    | /tasks/{task_id}  | Get specific task             | Yes                    |
| PUT    | /tasks/{task_id}  | Update task                   | Yes                    |
| DELETE | /tasks/{task_id}  | Delete task                   | Yes                    |

## Resume Skills Demonstrated

- ✅ Backend API development with FastAPI
- ✅ RESTful API design principles
- ✅ Database design and ORM usage
- ✅ Authentication and security implementation
- ✅ Frontend development with modern web technologies
- ✅ Responsive UI/UX design
- ✅ CRUD operations implementation
- ✅ Error handling and validation
- ✅ Full-stack integration
- ✅ Clean code and project organization

## Future Enhancements

- Task categories/tags
- Collaborative tasks and sharing
- Task notes and attachments
- Email notifications for due dates
- Task analytics and reports
- Dark mode theme
- Progressive Web App (PWA) features

## License

This project is licensed under the MIT License.