# 💪 EXERCICES PRATIQUES

## 🎯 Objectif
Maintenant que tu as suivi le guide, c'est à toi de coder !

---

## 📋 EXERCICE 1 : Code ton HTML de A à Z (30 min)

### Instructions :
1. **Supprime** (ou renomme) ton fichier `index.html` actuel
2. **Crée un nouveau** `index.html` vide
3. **Code TOUT le HTML sans regarder** le guide :
   - La structure de base
   - Le header avec menu
   - Les 3 sections
   - Le footer

### ✅ Auto-correction :
Compare avec le fichier `index-solution.html` (fourni)

---

## 🎨 EXERCICE 2 : Code ton CSS de A à Z (30 min)

### Instructions :
1. **Supprime** ton `style.css`
2. **Crée un nouveau** `style.css` vide
3. **Code le CSS sans regarder** :
   - Style du body
   - Style du header
   - Style du menu
   - Style des sections
   - Style du footer

### ✅ Auto-correction :
Compare avec `style-solution.css`

---

## 🚀 EXERCICE 3 : Personnalisation (45 min)

### Mission :
Transforme le site pour qu'il reflète **TA personnalité** !

### À faire :
1. **Contenu** :
   - [ ] Remplace par ton vrai nom
   - [ ] Écris ta vraie présentation
   - [ ] Ajoute tes vraies compétences
   - [ ] Mets ton vrai email/LinkedIn

2. **Design** :
   - [ ] Change les couleurs principales
   - [ ] Change la police de caractères
   - [ ] Modifie les espacements
   - [ ] Expérimente avec les tailles de texte

3. **Structure** :
   - [ ] Ajoute une 4ème section "Projets"
   - [ ] Ajoute une 5ème section "Expérience"

---

## 🎓 EXERCICE 4 : Comprendre les erreurs (20 min)

### Trouve et corrige les erreurs :

#### Code avec erreurs :

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mon Site
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Bonjour</h1>
    <p>Ceci est un paragraphe
    <a href="#contact">Contact
</body>
```

### Questions :
1. Combien d'erreurs y a-t-il ?
2. Quelles sont-elles ?
3. Comment les corriger ?

<details>
<summary>💡 Voir les réponses</summary>

**Erreurs trouvées :**
1. `<title>` pas fermé (manque `</title>`)
2. `<p>` pas fermé (manque `</p>`)
3. `<a>` pas fermé (manque `</a>`)
4. `</html>` manquant à la fin

**Code corrigé :**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Mon Site</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Bonjour</h1>
    <p>Ceci est un paragraphe</p>
    <a href="#contact">Contact</a>
</body>
</html>
```
</details>

---

## 🌈 EXERCICE 5 : Expérimente avec les couleurs (15 min)

### Crée 3 thèmes de couleurs différents :

#### Thème 1 : Professionnel Bleu
```css
header { background-color: #2c3e50; }
h2 { color: #3498db; }
```

#### Thème 2 : Créatif Violet
```css
header { background-color: #8e44ad; }
h2 { color: #9b59b6; }
```

#### Thème 3 : Énergique Rouge
```css
header { background-color: #c0392b; }
h2 { color: #e74c3c; }
```

### Mission :
1. Teste chaque thème
2. Crée TON propre thème avec tes couleurs préférées
3. Cherche sur Google "color palette generator" pour t'inspirer

---

## 📱 EXERCICE 6 : Ajouter une image (20 min)

### Instructions :

1. **Télécharge une photo** (de toi ou d'illustration)
2. **Mets-la dans** le dossier `images/`
3. **Ajoute dans le HTML** (section accueil) :

```html
<section id="accueil">
    <img src="images/photo.jpg" alt="Ma photo">
    <h2>Bienvenue sur mon portfolio</h2>
    <p>Étudiant en Business & Économie...</p>
</section>
```

4. **Style dans le CSS** :

```css
section img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
}
```

### 🧠 Comprendre :
- `border-radius: 50%` = Image ronde
- `object-fit: cover` = L'image remplit l'espace sans déformation

---

## 🎯 EXERCICE 7 : Créer un effet hover (15 min)

### Mission :
Quand on passe la souris sur les liens du menu, ils changent de couleur !

### Code à ajouter dans `style.css` :

```css
nav ul li a:hover {
    color: #3498db;
    border-bottom: 2px solid #3498db;
}
```

### Expérimente :
- Change la couleur du hover
- Ajoute une transition douce : `transition: all 0.3s;`
- Essaie d'autres effets (background, font-size...)

---

## 🏆 EXERCICE BONUS : Formulaire de contact (30 min)

### Remplace la section contact par :

```html
<section id="contact">
    <h2>Contactez-moi</h2>
    <form>
        <input type="text" placeholder="Votre nom" required>
        <input type="email" placeholder="Votre email" required>
        <textarea placeholder="Votre message" rows="5"></textarea>
        <button type="submit">Envoyer</button>
    </form>
</section>
```

### Style le formulaire :

```css
form {
    max-width: 500px;
    margin: 0 auto;
}

input, textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ddd;
    border-radius: 5px;
}

button {
    background-color: #1e2a38;
    color: white;
    padding: 10px 30px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
}

button:hover {
    background-color: #3498db;
}
```

---

## 📝 EXERCICE FINAL : Documentation (15 min)

### Ajoute des commentaires dans ton code :

#### Dans HTML :
```html
<!-- En-tête de la page -->
<header>
    <h1>Mon Nom</h1>
    
    <!-- Menu de navigation -->
    <nav>
        ...
    </nav>
</header>
```

#### Dans CSS :
```css
/* Style général de la page */
body {
    font-family: Arial, sans-serif;
    margin: 0;
}

/* En-tête avec fond sombre */
header {
    background-color: #1e2a38;
}
```

---

## ✅ Checklist de progression

- [ ] J'ai codé le HTML entier sans aide
- [ ] J'ai codé le CSS entier sans aide
- [ ] J'ai personnalisé le contenu avec mes infos
- [ ] J'ai créé mon propre thème de couleurs
- [ ] J'ai ajouté une photo
- [ ] J'ai créé une 4ème section
- [ ] J'ai ajouté des effets hover
- [ ] J'ai ajouté un formulaire de contact
- [ ] J'ai commenté mon code
- [ ] J'ai publié sur GitHub

---

## 🎉 Bravo !

Si tu as coché toutes les cases, tu maîtrises les bases du HTML/CSS !

**Prochaine étape :** Apprends le responsive design pour que ton site s'affiche bien sur mobile ! 📱
