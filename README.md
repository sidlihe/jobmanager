# Database
POSTGRES_USER=jobmanager
POSTGRES_PASSWORD=password
POSTGRES_DB=jobs
POSTGRES_HOST=db
POSTGRES_PORT=5432
DATABASE_URL=postgresql://jobmanager:password@db:5432/jobs

# pgAdmin
PGADMIN_EMAIL=admin@admin.com
PGADMIN_PASSWORD=root

# Application
BACKEND_PORT=8001
FRONTEND_PORT=5173
VITE_API_URL=http://localhost:8001

SECRET_KEY=09d25e094faa6ca2556c818166b7a9563b93f7099f6f0f4caa6cf63b88e8d3e7
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30




# for startup
use 3 terminal for,docker,frontend,backend
# docker
(venv) PS C:\Users\SiddheshLihe\jobmanager> docker-compose up -d
[+] Running 2/2
 ✔ Container jobmanager-db-1       Running                                                                                                              0.0s
 ✔ Container jobmanager-pgadmin-1  Started  

# backend
 (venv) PS C:\Users\SiddheshLihe\jobmanager\backend> uvicorn main:app --reload --port 8001
INFO:     Will watch for changes in these directories: ['C:\\Users\\SiddheshLihe\\jobmanager\\backend']
INFO:     Uvicorn running on http://127.0.0.1:8001 (Press CTRL+C to quit)

# frontend
(venv) PS C:\Users\SiddheshLihe\jobmanager\frontend> npm run dev

> frontend@0.0.0 dev
> vite


  VITE v7.2.7  ready in 433 ms

  ➜  Local:   http://localhost:5173/