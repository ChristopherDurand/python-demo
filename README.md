# Sample Apps to Run with Gander

## 1) Python / Django App (python-demo)

#### gander init
What directory is your application's entrypoint in? `./`
What is the path to your database setup file? `./db/migrate.sql`
What is the name of your database? `django_gander`

#### special configuration needs for Django
1) Include `'*'` in `ALLOWED_HOSTS`

2) Make sure the application is running with host `0.0.0.0` on port `8080`

3) Add a `Procfile` with the entrypoint command for your application.

   This demo app uses the following `Procfile`:
  `web: python3 manage.py runserver 0.0.0.0:8080`