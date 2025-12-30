# 🎨 Portfolio Créatif - Template Premium

Un template de portfolio moderne et élégant pour photographes, designers et créatifs.

---

## ✨ CARACTÉRISTIQUES

### Design & Interface
- ✅ Design moderne et épuré
- ✅ Mode clair/sombre avec sauvegarde des préférences
- ✅ Animations smooth et fluides
- ✅ 100% responsive (mobile, tablette, desktop)
- ✅ Lightbox pour galerie photos

### Pages Incluses
1. **index.html** - Page d'accueil avec hero
2. **gallery.html** - Galerie avec filtres
3. **about.html** - À propos
4. **contact.html** - Contact avec formulaire

### Fonctionnalités
- 🎯 Filtres de galerie (Photographie, Design, Art)
- 🖼️ Lightbox avec navigation clavier
- 🌙 Toggle thème clair/sombre
- 📱 Menu mobile responsive
- 💬 Formulaire de contact
- ⚡ Animations au scroll
- 🎨 Facilement personnalisable

---

## 📦 FICHIERS INCLUS

```
portfolio-creatif/
├── index.html              # Page d'accueil
├── gallery.html            # Galerie
├── about.html              # À propos
├── contact.html            # Contact
├── style.css               # Styles complets
├── script.js               # JavaScript
└── README.md               # Documentation
```

---

## 🚀 INSTALLATION

### Méthode 1 : Local (pour tester)

1. **Télécharge tous les fichiers**
2. **Ouvre `index.html` dans un navigateur**
3. C'est tout ! Le site fonctionne localement.

### Méthode 2 : Hébergement en ligne (GitHub Pages)

1. **Crée un repo GitHub**
```bash
git init
git add .
git commit -m "Premier commit"
git remote add origin https://github.com/TON-USERNAME/portfolio.git
git push -u origin main
```

2. **Active GitHub Pages**
   - Va dans Settings > Pages
   - Source : main branch
   - Ton site sera sur : `https://TON-USERNAME.github.io/portfolio/`

### Méthode 3 : Autres hébergeurs

- **Netlify** : Drag & drop le dossier sur netlify.com
- **Vercel** : Import depuis GitHub
- **OVH/O2switch** : Upload via FTP

---

## 🎨 PERSONNALISATION

### Changer les couleurs

Ouvre `style.css` et modifie les variables CSS (ligne 2) :

```css
:root {
    --primary: #2563eb;        /* Couleur principale */
    --secondary: #10b981;      /* Couleur secondaire */
    --accent: #f59e0b;         /* Couleur d'accent */
}
```

### Variantes de couleurs suggérées :

**Option 1 - Bleu/Vert (par défaut)**
```css
--primary: #2563eb;
--secondary: #10b981;
```

**Option 2 - Violet/Rose**
```css
--primary: #8b5cf6;
--secondary: #ec4899;
```

**Option 3 - Orange/Rouge**
```css
--primary: #f97316;
--secondary: #ef4444;
```

**Option 4 - Noir/Or**
```css
--primary: #1f2937;
--secondary: #f59e0b;
```

### Remplacer les images

1. **Images de galerie** : Remplace les URLs Unsplash par tes propres images
   - Dans `gallery.html`, trouve les balises `<img src="https://images.unsplash.com/..."`
   - Remplace par `<img src="images/ton-image.jpg"`

2. **Crée un dossier `images/`** dans ton projet

3. **Ajoute tes photos** avec des noms clairs (ex: `photo1.jpg`, `design1.jpg`)

### Modifier les textes

**Page d'accueil** (`index.html`) :
- Ligne 61 : Titre hero ("Créateur Visuel")
- Ligne 62 : Sous-titre ("Photographie • Design • Art")
- Ligne 86+ : Projets en vedette

**À propos** (`about.html`) :
- Ligne 38+ : Photo de profil
- Ligne 42+ : Texte de présentation
- Ligne 66+ : Compétences
- Ligne 98+ : Expérience/Timeline
- Ligne 146+ : Distinctions

**Contact** (`contact.html`) :
- Ligne 112+ : Email, téléphone, localisation

### Ajouter un projet dans la galerie

Dans `gallery.html`, ajoute ce code dans la section `.gallery-grid` :

```html
<div class="gallery-item" data-category="photography">
    <img src="images/ton-image.jpg" alt="Titre du projet" loading="lazy">
    <div class="gallery-overlay">
        <h3>Nom du Projet</h3>
        <p>Catégorie</p>
    </div>
</div>
```

**Catégories disponibles** : `photography`, `design`, `art`

---

## 📧 INTÉGRATION FORMULAIRE DE CONTACT

### Option 1 : Web3Forms (Recommandé - Gratuit)

1. **Va sur** [web3forms.com](https://web3forms.com)
2. **Crée un compte** et obtiens une access key
3. **Dans `contact.html`**, ajoute après la balise `<form>` :

```html
<form action="https://api.web3forms.com/submit" method="POST">
    <input type="hidden" name="access_key" value="TA-CLE-ICI">
    <!-- Reste du formulaire -->
</form>
```

### Option 2 : Formspree

1. **Va sur** [formspree.io](https://formspree.io)
2. **Crée un formulaire** et récupère l'URL
3. **Remplace** `<form id="contactForm">` par :

```html
<form action="https://formspree.io/f/TON-ID" method="POST">
```

### Option 3 : Backend PHP (si hébergement avec PHP)

Crée un fichier `send-email.php` :

```php
<?php
$name = $_POST['name'];
$email = $_POST['email'];
$message = $_POST['message'];

$to = "ton-email@exemple.com";
$subject = "Nouveau message du portfolio";
$body = "Nom: $name\nEmail: $email\n\n$message";

mail($to, $subject, $body);
header('Location: merci.html');
?>
```

---

## 💰 CONSEILS POUR VENDRE LE TEMPLATE

### Prix suggéré : **79€**

### Ce qu'il faut inclure dans la vente :

✅ **Tous les fichiers source** (HTML, CSS, JS)  
✅ **Documentation complète** (ce README)  
✅ **3 variantes de couleurs** (4 fichiers style.css différents)  
✅ **Support par email** (pendant 30 jours)  
✅ **Mises à jour gratuites** (pendant 1 an)  

### Plateformes de vente :

1. **Gumroad** (recommandé - facile)
   - Commission : 10% + frais
   - URL : gumroad.com

2. **Lemonsqueezy** (bon pour l'Europe)
   - Commission : 5% + frais
   - URL : lemonsqueezy.com

3. **ThemeForest** (gros trafic mais compliqué)
   - Commission : 50%
   - URL : themeforest.net

### Page de vente à créer :

**Éléments essentiels :**
- 🖼️ Screenshots de toutes les pages
- 🎥 Vidéo démo (2 minutes)
- ✨ Liste des fonctionnalités
- 📊 Tableau comparatif (avec/sans template)
- ⭐ Témoignages (si possible)
- 💳 Prix et bouton d'achat
- ❓ FAQ

### Marketing :

- **Twitter/X** : Partage des screenshots
- **Dribbble** : Poste le design
- **Behance** : Publie un case study
- **ProductHunt** : Lance le produit
- **Reddit** : r/web_design, r/webdev

---

## 🎯 CRÉER LES 3 VARIANTES DE COULEURS

### Variante 1 : Bleu/Vert (par défaut)
Fichier : `style.css`
```css
--primary: #2563eb;
--secondary: #10b981;
```

### Variante 2 : Violet/Rose
Fichier : `style-purple.css` (copie de style.css)
```css
--primary: #8b5cf6;
--secondary: #ec4899;
```

### Variante 3 : Orange/Rouge
Fichier : `style-warm.css` (copie de style.css)
```css
--primary: #f97316;
--secondary: #ef4444;
```

**Pour utiliser une variante**, remplace dans les HTML :
```html
<link rel="stylesheet" href="style-purple.css">
```

---

## 📱 RESPONSIVE DESIGN

Le template s'adapte automatiquement à :
- **Mobile** : < 768px
- **Tablette** : 768px - 1024px
- **Desktop** : > 1024px

Teste sur tous les devices avec les DevTools du navigateur (F12).

---

## 🐛 DEBUGGING

### Le thème ne se sauvegarde pas
- Vérifie que le localStorage fonctionne (désactive le mode privé du navigateur)

### Les images ne s'affichent pas
- Vérifie le chemin : `images/photo.jpg` (avec `images/` au début)
- Vérifie que le dossier `images/` existe

### Le lightbox ne fonctionne pas
- Ouvre la console (F12) et vérifie les erreurs JavaScript
- Vérifie que `script.js` est bien chargé

### Le formulaire ne fonctionne pas
- Configure Web3Forms ou Formspree
- Vérifie l'attribut `action` du formulaire

---

## 📄 LICENCE

Ce template a été créé par **Olivier** ([https://olirobz31.github.io/site-freelance-premium/](https://olirobz31.github.io/site-freelance-premium/))

**Licence d'utilisation :**
- ✅ Usage personnel et commercial
- ✅ Modifications autorisées
- ✅ Utilisation pour des clients
- ❌ Revente du template tel quel
- ❌ Distribution gratuite du code source

---

## 🆘 SUPPORT

**Email** : olirobz31@gmail.com

**Questions fréquentes** :
- Réponse sous 24-48h
- Support technique inclus pendant 30 jours après l'achat
- Mises à jour gratuites pendant 1 an

---

## 🎉 C'EST PRÊT !

Ton template portfolio créatif est prêt à être utilisé et vendu !

**Prochaines étapes** :
1. Personnalise les couleurs et textes
2. Ajoute tes vraies images
3. Configure le formulaire de contact
4. Crée 3 variantes de couleurs
5. Fais des screenshots
6. Crée ta page de vente
7. Lance sur Gumroad !

**Bon succès ! 🚀**