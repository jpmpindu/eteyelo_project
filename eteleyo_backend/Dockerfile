# Utilise une image Python légère
FROM python:3.14-slim

# Évite que Python génère des fichiers .pyc et permet un affichage direct des logs
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Définit le dossier de travail dans le conteneur
WORKDIR /code

# Installe les dépendances
COPY requirements.txt /code/
RUN pip install --no-cache-dir -r requirements.txt

# Copie le reste du code
COPY . /code/