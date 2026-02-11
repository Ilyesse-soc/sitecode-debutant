# 🎓 GUIDE COMPLET - Apprendre à coder son Portfolio

## 👋 Bienvenue !

Ce guide va t'apprendre à créer ton **portfolio professionnel** en HTML et CSS, **ligne par ligne**.

Tu vas **VRAIMENT** apprendre à coder, pas juste copier-coller ! 💪

---

## 📚 Comment utiliser ce guide ?

1. **Lis chaque étape** attentivement
2. **Tape le code toi-même** dans VS Code (ne copie pas !)
3. **Teste dans ton navigateur** après chaque étape
4. **Expérimente** : change les couleurs, les textes, etc.

---

## 🗂️ ÉTAPE 0 : Préparation

### Crée la structure de dossiers :

```
portfolio-business/
├── index.html       ← Ta page web (à créer)
├── style.css        ← Ton design (à créer)
└── images/          ← Tes photos (optionnel)
```

### Ouvre VS Code :
1. Clique droit dans le dossier `portfolio-business`
2. Choisis "Ouvrir avec Code" (ou ouvre VS Code et fais File > Open Folder)
3. Crée un nouveau fichier : `index.html`

✅ **Prêt ?** Continue à l'étape 1 !

---

## 🏗️ ÉTAPE 1 : La base HTML (5 minutes)

### 📝 Ton premier code

Ouvre `index.html` et tape **ligne par ligne** :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Mon Portfolio</title>
</head>
<body>
    <h1>Bonjour, je suis [Ton Nom]</h1>
</body>
</html>
```

### 🧠 Comprendre ce que tu as tapé :

| Code | Signification |
|------|---------------|
| `<!DOCTYPE html>` | "Hé navigateur, c'est du HTML5 !" |
| `<html lang="fr">` | Début du document, langue française |
| `<head>` | Informations invisibles (paramètres) |
| `<meta charset="UTF-8">` | Accepte les accents (é, à, ç...) |
| `<title>` | Titre dans l'onglet du navigateur |
| `<body>` | Contenu visible de ta page |
| `<h1>` | Titre principal (Heading 1) |

### ✅ Teste ton code :
1. **Sauvegarde** (Ctrl + S)
2. **Fais un clic droit** sur `index.html`
3. Choisis **"Ouvrir avec le navigateur par défaut"**

**Tu dois voir** ton nom en gros titre !

---

## 🧭 ÉTAPE 2 : Ajouter la navigation (10 minutes)

### 📝 Ajoute le menu

Juste **après** `<body>`, ajoute :

```html
<body>
    <header>
        <h1>[Ton Nom]</h1>
        <nav>
            <ul>
                <li><a href="#accueil">Accueil</a></li>
                <li><a href="#apropos">À propos</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
```

### 🧠 Nouvelles balises :

| Balise | Signification |
|--------|---------------|
| `<header>` | En-tête de la page |
| `<nav>` | Zone de navigation |
| `<ul>` | Liste à puces (Unordered List) |
| `<li>` | Élément de liste (List Item) |
| `<a href="">` | Lien hypertexte |
| `#accueil` | Ancre interne (va vers une section) |

### ✅ Teste :
Recharge ta page → Tu dois voir 3 liens (pas encore stylés)

---

## 📄 ÉTAPE 3 : Créer les sections (15 minutes)

### 📝 Ajoute les 3 sections

**Après** `</header>`, ajoute :

```html
    <section id="accueil">
        <h2>Bienvenue sur mon portfolio</h2>
        <p>Étudiant en Business & Économie, passionné par l'entrepreneuriat.</p>
    </section>

    <section id="apropos">
        <h2>À propos de moi</h2>
        <p>Je développe des compétences en gestion et finance.</p>
        <ul>
            <li>Analyse financière</li>
            <li>Marketing stratégique</li>
            <li>Entrepreneuriat</li>
        </ul>
    </section>

    <section id="contact">
        <h2>Contact</h2>
        <p>Email : ton.email@exemple.com</p>
        <p>LinkedIn : linkedin.com/in/ton-profil</p>
    </section>
```

### 🧠 Nouvelles balises :

| Balise | Signification |
|--------|---------------|
| `<section>` | Section de contenu |
| `id="accueil"` | Identifiant unique (pour les liens) |
| `<h2>` | Sous-titre (Heading 2) |
| `<p>` | Paragraphe de texte |

### ✅ Teste :
Clique sur les liens du menu → La page doit défiler vers chaque section !

---

## 🦶 ÉTAPE 4 : Ajouter le pied de page (5 minutes)

### 📝 Tout en bas, avant `</body>`

```html
    <footer>
        <p>© 2026 - Mon Portfolio Business</p>
    </footer>

</body>
</html>
```

### 🧠 Comprendre :

- `<footer>` = Pied de page
- `©` = Symbole copyright

### ✅ Ton HTML est complet !

À ce stade, tu as :
- ✅ Une structure HTML valide
- ✅ Un menu de navigation
- ✅ 3 sections de contenu
- ✅ Un pied de page

**MAIS** c'est moche ! 😅 On va corriger ça avec le CSS →

---

## 🎨 ÉTAPE 5 : Créer le fichier CSS (5 minutes)

### 📝 Crée `style.css`

1. **Crée un nouveau fichier** : `style.css`
2. **Lie-le au HTML** : dans `index.html`, dans la section `<head>`, ajoute :

```html
<head>
    <meta charset="UTF-8">
    <title>Mon Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
```

### 🧠 Comprendre :

- `<link>` = Lien vers un fichier externe
- `rel="stylesheet"` = C'est une feuille de style
- `href="style.css"` = Le nom du fichier CSS

---

## 🖌️ ÉTAPE 6 : Styliser le BODY (5 minutes)

### 📝 Dans `style.css`, tape :

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background-color: #f4f6f9;
    color: #333;
}
```

### 🧠 Comprendre :

| Propriété | Signification |
|-----------|---------------|
| `font-family` | Police de caractères |
| `margin: 0` | Enlève les marges par défaut |
| `background-color` | Couleur de fond (gris clair) |
| `color` | Couleur du texte (gris foncé) |
| `#f4f6f9` | Code hexadécimal d'une couleur |

### ✅ Teste :
Recharge → Le fond doit être gris clair !

---

## 🎯 ÉTAPE 7 : Styliser le HEADER (10 minutes)

### 📝 Ajoute dans `style.css` :

```css
header {
    background-color: #1e2a38;
    color: white;
    padding: 20px;
    text-align: center;
}
```

### 🧠 Comprendre :

- `padding: 20px` = Espace intérieur de 20 pixels
- `text-align: center` = Texte centré
- `#1e2a38` = Bleu foncé professionnel

### ✅ Teste :
Le header doit être bleu foncé avec texte blanc !

---

## 🧭 ÉTAPE 8 : Styliser le MENU (10 minutes)

### 📝 Ajoute :

```css
nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}
```

### 🧠 Comprendre :

| Propriété | Signification |
|-----------|---------------|
| `list-style: none` | Enlève les puces |
| `display: inline` | Affiche en ligne (horizontal) |
| `margin: 0 15px` | Espace entre les liens |
| `text-decoration: none` | Enlève le soulignement |
| `font-weight: bold` | Texte en gras |

### ✅ Teste :
Les liens doivent être côte à côte, en blanc, sans soulignement !

---

## 📄 ÉTAPE 9 : Styliser les SECTIONS (10 minutes)

### 📝 Ajoute :

```css
section {
    padding: 60px 20px;
    text-align: center;
}

section:nth-child(even) {
    background-color: white;
}

h2 {
    color: #1e2a38;
}
```

### 🧠 Comprendre :

- `padding: 60px 20px` = 60px en haut/bas, 20px à gauche/droite
- `:nth-child(even)` = Cible les sections paires (2, 4, 6...)
- Effet : alternance de couleurs entre sections

### ✅ Teste :
Les sections doivent alterner entre gris clair et blanc !

---

## 🦶 ÉTAPE 10 : Styliser le FOOTER (5 minutes)

### 📝 Ajoute :

```css
footer {
    background-color: #1e2a38;
    color: white;
    text-align: center;
    padding: 20px;
}
```

### ✅ Teste :
Le footer doit avoir le même style que le header !

---

## 🎉 ÉTAPE 11 : Personnalisation (À TOI DE JOUER !)

### ✏️ Exercices :

1. **Change ton nom** dans le HTML
2. **Modifie les couleurs** :
   - Essaie `background-color: #2c3e50;` (bleu différent)
   - Essaie `color: #e74c3c;` (rouge)
3. **Ajoute une section "Projets"** :
   - Copie une section existante
   - Change l'id et le contenu
   - Ajoute le lien dans le menu
4. **Change la police** :
   - Essaie `font-family: 'Georgia', serif;`
   - Ou `font-family: 'Courier New', monospace;`

---

## 🚀 ÉTAPE 12 : Publier sur GitHub

### 📝 Dans le terminal VS Code :

```bash
git add .
git commit -m "Mon portfolio terminé"
git push
```

---

## 📊 Ce que tu as appris

### HTML :
- ✅ Structure d'une page (`<!DOCTYPE>`, `<html>`, `<head>`, `<body>`)
- ✅ Balises de contenu (`<h1>`, `<p>`, `<ul>`, `<li>`)
- ✅ Balises sémantiques (`<header>`, `<nav>`, `<section>`, `<footer>`)
- ✅ Liens internes (`<a href="#section">`)
- ✅ Lien vers CSS (`<link>`)

### CSS :
- ✅ Sélecteurs (balise, class, id)
- ✅ Couleurs (hexadécimal)
- ✅ Mise en page (padding, margin)
- ✅ Typographie (font, color, text-align)
- ✅ Pseudo-classes (`:nth-child`)

---

## 🏆 Prochaines étapes (niveau avancé)

1. **Ajouter une photo de profil**
2. **Créer un formulaire de contact**
3. **Rendre le site responsive** (mobile)
4. **Ajouter des animations CSS**
5. **Utiliser Flexbox ou Grid**

---

## ❓ En cas de problème

### Le style ne s'applique pas ?
- Vérifie que `<link rel="stylesheet" href="style.css">` est dans le `<head>`
- Vérifie que `style.css` est bien dans le même dossier que `index.html`
- Recharge la page avec Ctrl + F5 (vide le cache)

### Les liens ne fonctionnent pas ?
- Vérifie que les `id=""` dans les sections correspondent aux `href="#"` dans les liens

### Le code ne s'affiche pas ?
- Vérifie les balises fermantes (chaque `<balise>` doit avoir son `</balise>`)
- Utilise l'extension "Live Server" dans VS Code pour voir les changements en direct

---

**Bravo ! Tu as codé ton premier site web professionnel ! 🎉**
