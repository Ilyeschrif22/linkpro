# Linkpro Dashboard

Interface de tableau de bord pour Linkpro créée avec HTML, CSS et Tailwind CSS.

## Structure du projet

```
linkpro-dashboard/
├── index.html      # Fichier HTML principal
├── styles.css      # Styles CSS personnalisés
└── README.md       # Ce fichier
```

## Technologies utilisées

- **HTML5** : Structure de la page
- **Tailwind CSS** : Framework CSS via CDN (chargé automatiquement)
- **CSS personnalisé** : Styles additionnels dans `styles.css`

## Comment exécuter le code

### Méthode 1 : Ouvrir directement dans le navigateur (le plus simple)

1. Double-clique sur le fichier `idnex.html`
2. Il s'ouvrira automatiquement dans ton navigateur par défaut

### Méthode 2 : Via un serveur local (recommandé pour le développement)

#### Option A : Avec Python (si installé)
```bash
# Python 3
python -m http.server 8000

# Puis ouvre ton navigateur sur : http://localhost:8000/idnex.html
```

#### Option B : Avec Node.js (si installé)
```bash
# Installe http-server globalement
npm install -g http-server

# Lance le serveur
http-server

# Puis ouvre ton navigateur sur l'URL affichée (généralement http://localhost:8080)
```

#### Option C : Avec VS Code
1. Installe l'extension "Live Server" dans VS Code
2. Clic droit sur `idnex.html` → "Open with Live Server"

## Où est Tailwind CSS ?

Tailwind CSS est chargé automatiquement via **CDN** (Content Delivery Network) dans le fichier HTML à la ligne 7 :

```html
<script src="https://cdn.tailwindcss.com"></script>
```

Cela signifie que :
- ✅ Pas besoin d'installation
- ✅ Pas besoin de compilation
- ✅ Fonctionne directement dans le navigateur
- ✅ Tu peux utiliser toutes les classes Tailwind directement

## Personnalisation

### Remplacer les images

Les placeholders d'images sont marqués avec des commentaires HTML. Remplace-les par :

```html
<!-- Pour les projets -->
<img src="chemin/vers/image.png" alt="Description" class="w-full h-full object-cover">

<!-- Pour les badges -->
<img src="chemin/vers/badge.png" alt="Badge" class="w-full h-full object-cover">

<!-- Pour la photo de profil -->
<img src="chemin/vers/profile.jpg" alt="Profile" class="w-full h-full object-cover">
```

### Modifier les styles

- **Classes Tailwind** : Modifie directement les classes dans le HTML
- **Styles personnalisés** : Modifie le fichier `styles.css`

## Notes

- Le fichier fonctionne sans serveur web, mais certains navigateurs peuvent bloquer les requêtes locales
- Pour un environnement de production, considère installer Tailwind CSS localement pour de meilleures performances

