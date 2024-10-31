# Tutotriel Django

## Powershell : Installation de l'environnement Ubuntu via WSL
```PowerShell
wsl install -d Ubuntu-22.04
```

##### Apres installation, exécuter la cmd 'wsl' pour accéder à la session Ubuntu

## Installation d'un environnement de travail Python Django sur Ubuntu

#### Mise à jour du système
```bash
sudo apt-get update && sudo apt-get upgrade -y
```

#### Installation de Python et des outils nécessaires
```bash
sudo apt install python3 python3-pip python3-venv -y
```

#### Créer un dossier qui contiendra ce tutoriel
```bash
mkdir <folderName>
```

#### Aller à la racine de ce projet
```bash
cd <folderName>
```

#### Création d'un environnement virtuel et activation de celui-ci
```bash
python3 -m venv .venv
source .venv/bin/activate
```

Assurez vous de bien être dans un environnemnt virtuel :
```bash
(.venv)user@hostname:~/home/...
```

#### Installation de Django et des outils nécessaires 
```bash
pip install django djangorestframework pygments
```
##### pygments is used for the code highlitghting

#### Vérification de l'installation
```bash
django-admin --version
```

#### Création d'un projet Django
```bash
django-admin startproject monprojet
cd monprojet
```

#### Lancement du serveur de développement
```bash
python manage.py runserver
```

##### Note : N'oubliez pas d'activer votre environnement virtuel à chaque utilisation

# Ajout manuel de datas
```bash
http -a user:password POST htto://127.0.0.1:8000/snippets/ code="print(message)"
```

