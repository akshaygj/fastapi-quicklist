# QuickList - A Todo App

This is a simple Todo application built with Next.js, Supabase, and FastAPI.

## Setup

### Frontend (Next.js)

1. Clone the repository
2. Navigate to the project directory
3. Install dependencies: `npm install`
4. Create a `.env.local` file with your Supabase credentials:
```
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
```
5. Run the development server: `npm run dev`

### Backend (FastAPI)

1. Navigate to the `fastapi-server` directory
2. Create a virtual environment: `python -m venv venv`
3. Activate the virtual environment:
- On macOS/Linux: `source venv/bin/activate`
- On Windows: `venv\Scripts\activate`
4. Install dependencies: `pip install -r requirements.txt`
5. Create a `.env` file with your Supabase credentials:
```
SUPABASE_URL=your_supabase_project_url
SUPABASE_KEY=your_supabase_service_role_key
```
6. Run the FastAPI server: `uvicorn main:app --reload`

## Usage

1. Open your browser and go to `http://localhost:3000`
2. Register a new account or log in with an existing one
3. Add, view, and delete todo items

## Access Control

- Users must be authenticated to access the todo functionality
- Each user can only see and manage their own todos
