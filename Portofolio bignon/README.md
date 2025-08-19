# Portfolio d'Innocent GBEDONOU - Bignon du Bénin

## Description
Site web professionnel présentant Innocent GBEDONOU, entrepreneur béninois passionné par le design et l'ameublement, et son entreprise Bignon du Bénin.

## Fonctionnalités
- **Page d'accueil** : Présentation d'Innocent GBEDONOU et de son parcours
- **Page de contact** : Formulaire de contact et informations de l'entreprise
- **Page d'événement** : Détails sur le Gala des Entrepreneurs de Porto-Novo
- **Design responsive** : Compatible mobile, tablette et desktop
- **Navigation mobile** : Barre de navigation fixe en bas d'écran (mobile-first)
- **Mode sombre/clair** : Basculement automatique entre thèmes
- **Sélecteur de couleurs** : Personnalisation de la palette de couleurs
- **Animations AOS** : Effets de défilement élégants
- **Carrousel de témoignages** : Présentation des avis clients
- **PWA (Progressive Web App)** : Installation sur l'écran d'accueil, mode hors ligne

## Structure des fichiers
```
├── index.html              # Page d'accueil
├── about.html              # Page À propos détaillée
├── contact.html            # Page de contact
├── blog_details.html       # Détails de l'événement
├── privacy-policy.html     # Politique de confidentialité
├── terms-of-service.html   # Conditions d'utilisation
├── 404.html               # Page d'erreur 404
├── 500.html               # Page d'erreur 500
├── assets/                 # Ressources (CSS, JS, images)
│   ├── css/
│   │   ├── style.css      # Styles principaux
│   │   └── mobile-nav.css # Navigation mobile
│   ├── js/                # Scripts JavaScript
│   └── images/            # Images et logos
├── manifest.json           # Manifeste PWA
├── sitemap.xml            # Sitemap pour le SEO
├── robots.txt             # Configuration des robots
├── .htaccess              # Configuration serveur
├── analytics.html          # Configuration Google Analytics
├── cookie-banner.html      # Bannière de cookies RGPD
└── README.md              # Documentation
```

## Technologies utilisées
- HTML5 sémantique
- CSS3 avec variables personnalisées
- JavaScript vanilla
- AOS (Animate On Scroll)
- Swiper.js pour les carrousels
- Phosphor Icons
- EmailJS pour le formulaire de contact

## Installation et utilisation

### 1. Cloner le projet
```bash
git clone [URL_DU_REPO]
cd portfolio-bignon
```

### 2. Ouvrir dans un navigateur
Ouvrez simplement `index.html` dans votre navigateur web préféré.

### 3. Configuration EmailJS (optionnel)
Pour activer le formulaire de contact :
1. Créez un compte sur [EmailJS](https://www.emailjs.com/)
2. Remplacez `YOUR_USER_ID` dans `contact.html` par votre User ID
3. Configurez votre service d'email

## Personnalisation

### Couleurs
Le site utilise un système de variables CSS pour les couleurs. Modifiez les valeurs dans `assets/css/style.css` :
```css
:root {
  --p1: 120, 171, 168;  /* Couleur principale */
  --n1: 255, 255, 255;  /* Blanc */
  --n5: 51, 51, 51;     /* Texte principal */
  /* ... autres couleurs */
}
```

### Contenu
- Modifiez les textes directement dans les fichiers HTML
- Remplacez les images dans le dossier `assets/images/`
- Ajustez les liens sociaux dans la sidebar

## SEO et Performance

### Optimisations incluses
- Balises meta optimisées
- Balises Open Graph pour les réseaux sociaux
- Sitemap XML
- Robots.txt
- Attributs alt descriptifs pour les images
- Structure HTML sémantique

### Améliorations recommandées
- Compresser les images
- Minifier CSS et JavaScript
- Utiliser un CDN pour les ressources externes
- Implémenter la mise en cache

## Compatibilité
- ✅ Chrome (dernière version)
- ✅ Firefox (dernière version)
- ✅ Safari (dernière version)
- ✅ Edge (dernière version)
- ✅ Mobile (iOS/Android)

## Navigation Mobile

### Caractéristiques
- **Design mobile-first** : Optimisé pour les petits écrans
- **Barre fixe en bas** : Navigation accessible en permanence
- **3 éléments principaux** : Accueil, À propos, Contact
- **Indicateur visuel** : Page active clairement identifiée
- **Animations fluides** : Effets de survol et de pression
- **Conformité totale** : Structure identique sur toutes les pages

### Structure
```
[🏠 Accueil] [👤 À Propos] [✉️ Contact]
```

### Responsive
- **Mobile (≤480px)** : Icônes grandes, texte visible
- **Tablette (481-768px)** : Icônes moyennes, texte visible
- **Desktop (>768px)** : Navigation masquée (sidebar utilisée)

### Icônes utilisées
- 🏠 **Accueil** : `ph-house` (maison)
- 👤 **À Propos** : `ph-user` (utilisateur)
- ✉️ **Contact** : `ph-envelope` (enveloppe)

### Conformité du Menu

#### **Structure uniforme sur toutes les pages :**
- **Sidebar Desktop** : 3 éléments avec indicateur de page active
- **Navigation Mobile** : Barre fixe en bas avec 3 éléments
- **Ordre cohérent** : Accueil → À Propos → Contact

#### **Pages et leurs états actifs :**
- **`index.html`** : Accueil actif (sidebar + mobile)
- **`about.html`** : À Propos actif (sidebar + mobile)
- **`contact.html`** : Contact actif (sidebar + mobile)
- **`blog_details.html`** : Accueil actif (sidebar + mobile)

#### **Classes CSS utilisées :**
- **Page active** : `bg1-color` + `n11-color`
- **Pages inactives** : `n5-color` (couleur normale)
- **Structure** : `rounded-3` pour tous les éléments

#### **Conformité totale garantie :**
- **Sidebar Desktop** : 3 éléments avec indicateur de page active
- **Navigation Mobile** : 3 éléments avec indicateur de page active
- **Classes CSS** : Identiques sur toutes les pages
- **Ordre des éléments** : Accueil → À Propos → Contact (constant)

## Configuration PWA (Progressive Web App)

### Fonctionnalités activées
- **Installation sur l'écran d'accueil** : Compatible iOS et Android
- **Mode hors ligne** : Service Worker pour la mise en cache
- **Apparence native** : Interface similaire à une application mobile
- **Icônes adaptatives** : Support des différentes tailles d'écran

### Configuration incluse
- **Manifeste PWA** : `manifest.json` avec métadonnées complètes
- **Meta tags** : Configuration pour tous les navigateurs
- **Icônes** : Support iOS (Apple Touch Icons) et Android
- **Thème** : Couleurs cohérentes avec la charte graphique

### Meta tags PWA ajoutés
```html
<link rel="manifest" href="manifest.json" />
<meta name="theme-color" content="#78aba8" />
<meta name="apple-mobile-web-app-capable" content="yes" />
<meta name="apple-mobile-web-app-title" content="Bignon du Bénin" />
```

### Icônes supportées
- **iOS** : 152x152, 180x180, 167x167 pixels
- **Android** : 32x32, 16x16 pixels
- **Favicon** : 16x16 pixels pour les navigateurs

## Support
Pour toute question ou suggestion, contactez l'équipe de développement.

## Licence
© 2024 BIGNON DU BENIN. Tous droits réservés.

---

**Développé par** [Génération Impact 3.0](https://generationimpact3.0.com)
