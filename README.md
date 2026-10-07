# Cyberbullying Detection

A Django application for detecting cyberbullying in social media posts using machine-learning models.

## Project files

- `Cyberbullying/` contains the Django project and application.
- `Cyberbullying/model/` contains model and vectorizer assets.

The 665 MB `Cyberbullying/model/X.npy` file and the MySQL installer are excluded from this repository because they exceed GitHub's standard file size limit. The application currently loads `model/X.npy` at startup, so provide that file locally before running the project.

## Configuration

Set `DB_PASSWORD` in the environment to the password for the local MySQL account used by the application. Set `DJANGO_SECRET_KEY` to a unique secret before deploying; the built-in development fallback is not suitable for production.

Install the packages in `Cyberbullying/requirements.txt`, configure the MySQL database using `Cyberbullying/DB.txt`, then run the Django server from the `Cyberbullying` directory.
