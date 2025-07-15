# 🎯 Mes Starter Kits

Ce repo contient plusieurs variantes de starters Symfony et autres frameworks.

## ⚠️ Pré-Requis pour mes starter kits
- PHP v8.4
- WampServer 3.3
  
## ⚙️ Configuration

### php.ini

Télécharger et copier le fichier _cacert.pem_ dans le dossier de PHP et ajouter les lignes suivante :

>  curl.cainfo = "C:/wamp64/bin/php/php8.4.10/extras/ssl/cacert.pem"
>  openssl.cafile="C:/wamp64/bin/php/php8.4.10/extras/ssl/cacert.pem"

Modifier la taille limite :
>memory_limit = 512M

## 📦 Liste des starters

- [`symfony-tailwind`](./symfony-tailwind/) — Symfony + Tailwind CSS v4


## 🧰 Utilisation

### 1. Cloner un seul starter

```bash
git clone --filter=blob:none --sparse https://github.com/AubourgA/starter_kit.git
cd starter_kit
git sparse-checkout set nom_starter_kit
````

### 2. Copier le starter dans un nouveau dossier

````bash
cp -R starter_kit/nom_starter_kit nouveau_dossier
````

# Type Starter kit : Symfony

### 1. Installer le dossier vendor

Se rendre dans le nouveau_dossier

````bash
composer install
`````

### 2. Initier git [facultatif]

Préparer un repo github sur github.com

taper la commande suivante :
````bash
git init
````

suiver les étapes :
````bash
git add .
git commit -m "first commit"
git branch -M main
git add remote origin [nom_du_repo.git]
git push -u origin main
````

### 3. Télécharger et mettre le fichier tailwind

Telecharger le fichier executalbe de tailwind :


[`https://github.com/tailwindlabs/tailwindcss/releases/download/v4.1.11/tailwindcss-windows-x64.exe`](https://github.com/tailwindlabs/tailwindcss/releases/download/v4.1.11/tailwindcss-windows-x64.exe)

### 4. Initialiser le dossier de reception
Avec la commande suivante, cela va créer le dossier pour tailwind
````bash
symfony console tailwind:build -w
````

Copier le fichier **tailwindcss-windows-x64.exe**
````
var/tailwind/v4.1.11/tailwindcss-windowsx64.exe
````

### 5. Lancer le projet

```bash
symfony serve
symfony console tailwind:build -w
````

Le projet est disponible [127.0.0.1:8000](127.0.0.1:8000)
