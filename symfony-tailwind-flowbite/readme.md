# 🎨 Symfony 7.3 + Tailwind CSS 4 + Flowbite

Ce projet utilise Tailwind CSS v4 avec AssetMapper (pas de Node.js) et intègre la bibliothèque d'UI Flowbite.

---

## ✅ Prérequis

- PHP ≥ 8.2

## 🛠️ Setup

Pour que les animation fonctionnent, dans le fichier _app.js_, il est necessaire d'avoir :
````bash
import 'flowbite';
````

## 📝 Customisez les couleurs ou autres

### Configuration

Dans le dossier _assets/styles/app.css_

````css
@theme {
  --color-primary-100: #e0e7ff;
  --color-primary-200: #c7d2fe;
  --color-primary-300: #a5b4fc;
  --color-primary-400: #818cf8;
  --color-primary-500: #6366f1;
  --color-primary-600: #5850ec;
  --color-primary-700: #5145cd;
  --color-primary-800: #4f46e5;
}
````

### Application

Dans un fichier twig :

````twig
<div class="bg-primary-300">...</div>
````




