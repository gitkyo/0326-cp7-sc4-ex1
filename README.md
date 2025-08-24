# 📸 Exercice Pratique de 5h : "Le Portfolio d'Éléonore, Photographe d'Art"

**Mission** : Créer la page d'accueil du portfolio en ligne d'Éléonore, une photographe d'art contemporain.

## 🎯 Contexte de l'Exercice

Vous êtes un(e) **Concepteur Designer UI** et votre cliente Éléonore souhaite mettre en ligne son portfolio artistique. Elle vous a fourni :

- ✅ Un moodboard visuel de ce qu'elle souhaite
- ✅ Ses plus belles photographies en haute résolution
- ✅ Une vidéo de présentation de son atelier

**Votre mission** : Transformer sa vision artistique en une vitrine numérique professionnelle, responsive et optimisée pour le web.

💡 **Pourquoi cet exercice ?** Vous n'êtes pas juste en train de "coder", vous créez une expérience qui va permettre à une artiste de partager son travail avec le monde entier !

## 🛠️ Outils et Technologies

- **HTML5** : Structure sémantique
- **CSS3** : Styles et animations
- **Responsive Design** : Media queries
- **Optimisation** : Formats d'images modernes

## 🎓 Philosophie d'Apprentissage

**⚠️ IMPORTANT** : Ce n'est PAS un exercice de copier-coller !

**Votre approche doit être** :

1. **LIRE** le code avant de le copier
2. **COMPRENDRE** ce que fait chaque partie
3. **TESTER** chaque étape dans votre navigateur
4. **EXPÉRIMENTER** en modifiant des valeurs
5. **QUESTIONNER** tout ce qui n'est pas clair
6. **PARTAGER** vos découvertes avec les autres

🤝 **Règle d'or** : Si vous ne comprenez pas une ligne de code, demandez ! Il n'y a aucune question stupide en programmation.

## 🚀 Mindset du Développeur

- **Curiosité** : "Pourquoi ça marche ?"
- **Expérimentation** : "Que se passe-t-il si je change ça ?"
- **Collaboration** : "J'explique à mon binôme pour mieux comprendre"
- **Persévérance** : "Un bug est un puzzle à résoudre"
- **Créativité** : "Comment puis-je personnaliser cela ?"

## 📋 Progression Détaillée de l'Exercice (5h)

⏰ **Gestion du temps** : Chaque étape a un timing indicatif, mais l'important est de COMPRENDRE, pas de finir vite !

👥 **Travail en binôme recommandé** : Un qui code, un qui observe et questionne. Alternez les rôles !

### ⚡ Étape 1 : La Fondation (1h)

**Objectif** : Créer la structure de base de la page d'accueil

🏗️ **Concept architectural** : Comme un bâtiment, un site web a besoin de fondations solides. La structure HTML est votre béton armé !

#### 1.1 Structure HTML de base

🤔 **Avant de commencer** : Prenez 2 minutes pour observer la structure ci-dessous. Pouvez-vous identifier les différentes parties d'une page web ?

Créez un fichier `index.html` et copiez cette structure :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Éléonore - Photographe d'Art</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="header">
        <div class="container">
            <div class="logo">
                <h1>Éléonore</h1>
                <span>Photographe d'Art</span>
            </div>
            <nav class="nav">
                <ul>
                    <li><a href="#accueil">Accueil</a></li>
                    <li><a href="#portfolio">Portfolio</a></li>
                    <li><a href="#about">À propos</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <section id="accueil" class="hero">
            <div class="hero-content">
                <h2>Capturer l'émotion dans chaque instant</h2>
                <p>Découvrez l'univers photographique d'Éléonore, où l'art rencontre la réalité.</p>
                <a href="#portfolio" class="btn-primary">Voir le Portfolio</a>
            </div>
        </section>

        <section id="portfolio" class="portfolio">
            <div class="container">
                <h2>Mes Œuvres</h2>
                <!-- Le carrousel sera ajouté ici -->
                <div class="carousel-container">
                    <!-- Contenu à venir -->
                </div>
            </div>
        </section>

        <section id="about" class="about">
            <div class="container">
                <h2>À propos</h2>
                <p>Passionnée par la photographie depuis plus de 10 ans...</p>
            </div>
        </section>
    </main>

    <footer class="footer">
        <div class="container">
            <p>&copy; 2024 Éléonore - Tous droits réservés</p>
        </div>
    </footer>
</body>
</html>
```

🔍 **TEST & COMPRÉHENSION** :

1. **Testez** : Ouvrez votre fichier `index.html` dans le navigateur. Que voyez-vous ?
2. **Analysez** : Trouvez dans le code les balises `<header>`, `<main>`, `<section>`. À quoi servent-elles ?
3. **Réflexion** : Pourquoi utilise-t-on `<nav>` plutôt qu'une simple `<div>` pour la navigation ?
4. **Question groupe** : Discutez en binôme : que signifie "structure sémantique" ?

#### 1.2 Styles CSS de base

💡 **Avant de coder** : Ce CSS va transformer votre page HTML basique en quelque chose de beau. Observez les sélecteurs utilisés.

Créez un fichier `styles.css` et ajoutez ces styles :

```css
/* Reset et styles généraux */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    color: #333;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header */
.header {
    background: rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(10px);
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
    padding: 1rem 0;
}

.header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo h1 {
    font-size: 1.8rem;
    color: #2c3e50;
}

.logo span {
    font-size: 0.9rem;
    color: #7f8c8d;
}

.nav ul {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav a {
    text-decoration: none;
    color: #2c3e50;
    font-weight: 500;
    transition: color 0.3s ease;
}

.nav a:hover {
    color: #e74c3c;
}

/* Section Hero */
.hero {
    height: 100vh;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
    margin-top: 100px;
}

.hero-content h2 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.hero-content p {
    font-size: 1.2rem;
    margin-bottom: 2rem;    
}

.btn-primary {
    display: inline-block;
    padding: 1rem 2rem;
    background: #e74c3c;
    color: white;
    text-decoration: none;
    border-radius: 50px;
    transition: transform 0.3s ease;
}

.btn-primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 25px rgba(231, 76, 60, 0.3);
}

/* Sections */
.portfolio, .about {
    padding: 4rem 0;
}

.portfolio h2, .about h2 {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 3rem;
    color: #2c3e50;
}

/* Footer */
.footer {
    background: #2c3e50;
    color: white;
    text-align: center;
    padding: 2rem 0;
}
```

**✅ Résultat attendu** : Une page avec un header fixe, une section hero attractive et une structure de base.

🧪 **EXPÉRIMENTATION & APPRENTISSAGE** :

1. **Test visuel** : Rechargez votre page. La transformation est-elle spectaculaire ?
2. **Décortiquage CSS** : A l'aide de l'inspecteur d'élément du navigateur (F12), onglet "Élements", vous trouverez sur la droite de cette fenêtre le CSS de l'élément HTML selectionné dans la partie à gauche.
   - Supprimez temporairement `position: fixed` du header. Que se passe-t-il ?
   - Changez la couleur `#e74c3c` du bouton par `#3498db`. Aimez-vous mieux ?
3. **Questions importantes** :
   - Sur le bouton, pourquoi utilise-t-on `border-radius: 50px;` ?
   - Sur la section de class hero, monter le gradient CSS à votre voisin, essayer de modifier des valeurs et tester.
4. **Défi** : Modifiez les couleurs du gradient pour créer votre propre ambiance, vous pouvez utiliser des générateurs de code gradient css comme : <https://cssgradient.io/>
5. **Discussion** : En groupe, identifiez 3 propriétés CSS que vous ne connaissiez pas

💭 **Piste de réflexion** : Ce CSS utilise des techniques modernes (flexbox, gradients). Pourquoi est-ce important de les maîtriser aujourd'hui ?

### 📱 Étape 2 : La Réactivité (1h)

**Objectif** : Rendre le site adaptatif sur tous les écrans

🤓 **Concept clé** : Le responsive design n'est pas juste une option, c'est une NÉCESSITÉ ! Plus de 50% du trafic web vient du mobile.

#### 2.1 Ajoutez les Media Queries

🎯 **Stratégie** : Nous allons utiliser l'approche "Mobile First" - d'abord le mobile, puis on adapte pour les écrans plus grands.

Ajoutez ce code à la fin de votre fichier `styles.css` :

```css
/* ======= RESPONSIVE DESIGN ======= */

/* Mobile First - Styles par défaut déjà optimisés pour mobile */

/* Navigation mobile */
@media (max-width: 768px) {
    .header .container {
        flex-direction: column;
        gap: 1rem;
    }
    
    .nav ul {
        flex-direction: column;
        text-align: center;
        gap: 1rem;
    }
    
    .hero-content h2 {
        font-size: 2rem;
    }
    
    .hero-content p {
        font-size: 1rem;
        padding: 0 1rem;
    }
}

/* Tablettes */
@media (min-width: 768px) {
    .hero-content h2 {
        font-size: 3.5rem;
    }
    
    .container {
        padding: 0 40px;
    }
}

/* Ordinateurs de bureau */
@media (min-width: 1024px) {
    .hero-content h2 {
        font-size: 4rem;
    }
    
    .nav ul {
        gap: 3rem;
    }
    
    .container {
        padding: 0 60px;
    }
}
```

**🔍 Test** : Redimensionnez votre navigateur pour voir les changements !

🚀 **TESTS & DÉCOUVERTE** :

1. **Test multi-écrans** :
   - Ouvrez les outils de développement (F12)
   - Cliquez sur l'icône mobile/tablette
   - Testez : iPhone SE (375px), iPad (768px), Desktop (1200px)
2. **Expérimentation** :
   - Pour la zone CSS de la media queries pour tablettes, changez le breackpoint (points de ruptures) `768px` par `600px`. Que remarquez-vous ?
   - Ajoutez `border: 2px solid red;` à `.container` temporairement pour voir les zones. Changez la taille de la fenêtre pour observer les changements sur la zone rouge.
3. **Questions cruciales** :
   - Pourquoi commence-t-on par mobile (Mobile First) ?
   - Que signifie `min-width` vs `max-width` ?
   - À votre avis, quels sont les breakpoints les plus importants ?
4. **Challenge** : Créez un breakpoint pour très grands écrans (min-width: 1440px)
5. **Partage** : Montrez à votre binôme comment votre site s'adapte

💡 **Concept important** : Un bon responsive ne cache pas de contenu, il le réorganise intelligemment !

---

## 🔄 Pause Réflexion 1 (5 min)

**Temps de digestion** : Vous venez de créer les bases et le responsive. Avant de continuer :

**En binôme, discutez :**

- Qu'est-ce qui vous a le plus surpris jusqu'ici ?
- Quelle différence voyez-vous entre votre site et un site "amateur" ?
- Si un client vous demandait d'expliquer pourquoi le responsive est important, que diriez-vous ?

**Test rapide :**
Changeons le gradient CSS de la zone hero par une image en fond d'écran. Pour cela, rechercher dans le fichier CSS ou se situe la zone hero (/*Section Hero*/ ligne 64) et ajouter ces propriétés :

```css
background-image: url('https://images.unsplash.com/photo-1584513707958-07bf650b9026?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
background-size: cover;
background-position: center;
```

Montrez votre site à quelqu'un d'autre. Comprend-il immédiatement que c'est un portfolio de photographe ?
Si vous le souhaitez, vous pouvez changer l'image depuis une banque d'images libres comme unsplash ou vous copier coller l'adresse de l'image dans la valeur de la prorpriété background-image.

---

### 🎬 Étape 3 : La Vidéo et les Micro-Animations (1h)

**Objectif** : Ajouter une vidéo de fond et des animations

🎨 **Pourquoi des animations ?** Les micro-animations guident l'utilisateur et rendent l'expérience plus agréable. Mais attention : trop d'animations tuent l'animation !

#### 3.1 Ajout de la vidéo de fond

⚠️ **Note importante** : Une vidéo en arrière-plan peut être lourde. Nous allons voir comment bien l'optimiser.

- Vérifier que vous avez le dossier "ressources" dans votre projet web (à côté du fichier index.htlm et styles.css) avec la vidéo "video-libre1920_1080_30fps.mp4" transmit par le formateur.
- Modifiez la section hero dans votre `index.html` :

```html
<section id="accueil" class="hero">
    <video class="hero-video" autoplay muted loop>
        <source src="ressources/video-libre1920_1080_30fps.mp4" type="video/mp4">
        <!-- Fallback si la vidéo ne se charge pas -->
    </video>
    <div class="hero-overlay"></div>
    <div class="hero-content">
        <h2>Capturer l'émotion dans chaque instant</h2>
        <p>Découvrez l'univers photographique d'Éléonore, où l'art rencontre la réalité.</p>
        <a href="#portfolio" class="btn-primary">Voir le Portfolio</a>
    </div>
</section>
```

#### 3.2 Styles pour la vidéo et animations

Ajoutez ces styles à votre `styles.css` :

```css
/* Vidéo de fond */
.hero {
    position: relative;
    overflow: hidden;
}

.hero-video {
    position: absolute;
    top: 50%;
    left: 50%;
    min-width: 100%;
    min-height: 100%;
    width: auto;
    height: auto;
    transform: translateX(-50%) translateY(-50%);    
}

.hero-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.4);
    z-index: -1;
}

/* Animations */
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.hero-content {
    animation: fadeInUp 1s ease-out;
}

.hero-content h2 {
    animation: fadeInUp 1s ease-out 0.2s both;
}

.hero-content p {
    animation: fadeInUp 1s ease-out 0.4s both;
}

.btn-primary {
    animation: fadeInUp 1s ease-out 0.6s both;
}

/* Micro-animations sur les boutons */
.btn-primary {
    position: relative;
    overflow: hidden;
}

.btn-primary::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
    transition: left 0.5s;
}

.btn-primary:hover::before {
    left: 100%;
}
```

**💡 Note** : Si la vidéo ne peux pas se charger, l'image sera affiché et si celle ci rencontre des soucis, ce sera le gradient CSS qui sera affiché.

Hésitez pas à changer de vidéos ! Exemple des ressources videos gratuites et libres : <https://www.pexels.com/fr-fr/chercher/videos/photographe/>

🎭 **ANIMATION & EXPÉRIENCE** :

1. **Test des animations** :
   - Rechargez la page et observez l'effet d'apparition
   - Survolez le bouton pour voir l'effet de brillance
   - Testez la navigation au clavier (Tab pour parcourir)
2. **Expérimentation créative** :
   - Dans la zone CSS que vous venez de copier coller, une partie concerne l'animation du bouton. Modifiez la durée d'animation de `1s` à `2s`. Préférez-vous ?
   - Changez `ease-out` par `ease-in-out`. Ressentez-vous la différence ?
3. **Questions de groupe** :
   - Pourquoi utilise-t-on `autoplay muted` pour la vidéo ?
   - Quand faut-il éviter les animations ?
4. **Défi UX** : Proposez 2 autres micro-animations (sans impléter le code ^^) qui amélioreraient l'expérience

🧠 **Réflexion UX** : Une bonne animation raconte une histoire et guide l'œil. Elle ne doit jamais être gratuite !

---

## 🔄 Pause Réflexion 2 (5 min)

**Checkpoint créatif** : Votre site commence à avoir du caractère !

**Questions individuelles :**

- Votre site vous fait-il envie ? Pourquoi ?
- Quelles animations vous plaisent le plus ?
- Comment pourriez-vous adapter ce design pour un autre métier (architecte, chef cuisinier, musicien) ?

**Défi créatif :** En 30 secondes, proposez une couleur de thème différente et justifiez votre choix avec votre voisin !

---

### 🎠 Étape 4 : Le Carrousel et la Galerie Avancée (1h30)

**Objectif** : Créer un carrousel interactif et une galerie avec effets

🚨 **Attention** : Cette étape est la plus complexe ! Nous entrons dans le JavaScript. Prenez votre temps et n'hésitez pas à poser des questions.

🤝 **Conseil** : Travaillez en binôme pour cette partie. L'un code, l'autre observe et pose des questions !

#### 4.1 Structure HTML du carrousel

🏗️ **Architecture** : Avant de coder, observez bien la structure. Un carrousel = container + slides + contrôles + indicateurs.

- Vérifiez que vous avez bien le dossier ressources avec les images : "slide-1.jpg, slide-2.jpg et slide-3.jpg, thumb-1.jpg, thumb-2.jpg, thumb-3.jpg et thumb-4.jpg"
- Remplacez le contenu de la section portfolio :

```html
<section id="portfolio" class="portfolio">
    <div class="container">
        <h2>Mes Œuvres</h2>
        
        <!-- Carrousel principal -->
        <div class="carousel">
            <div class="carousel-container">
                <div class="carousel-slide active">
                    <img src="ressources/slide-1.jpg" alt="Œuvre 1">
                    <div class="slide-info">
                        <h3>Lumières urbaines</h3>
                        <p>Série photographique sur la ville la nuit</p>
                    </div>
                </div>
                <div class="carousel-slide">
                    <img src="ressources/slide-2.jpg" alt="Œuvre 2">
                    <div class="slide-info">
                        <h3>Portraits d'âmes</h3>
                        <p>Exploration de l'émotion humaine</p>
                    </div>
                </div>
                <div class="carousel-slide">
                    <img src="ressources/slide-3.jpg" alt="Œuvre 3">
                    <div class="slide-info">
                        <h3>Nature abstraite</h3>
                        <p>Formes et textures naturelles</p>
                    </div>
                </div>
            </div>
            
            <!-- Contrôles du carrousel -->
            <button class="carousel-btn prev" onclick="changeSlide(-1)">❮</button>
            <button class="carousel-btn next" onclick="changeSlide(1)">❯</button>
            
            <!-- Indicateurs -->
            <div class="carousel-indicators">
                <span class="indicator active" onclick="currentSlide(1)"></span>
                <span class="indicator" onclick="currentSlide(2)"></span>
                <span class="indicator" onclick="currentSlide(3)"></span>
            </div>
        </div>
        
        <!-- Galerie secondaire -->
        <div class="gallery">
            <h3>Galerie</h3>
            <div class="gallery-grid">
                <div class="gallery-item">
                    <img src="ressources/thumb-1.jpg" alt="Miniature 1">
                    <div class="gallery-overlay">
                        <span>Voir plus</span>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="ressources/thumb-2.jpg" alt="Miniature 2">
                    <div class="gallery-overlay">
                        <span>Voir plus</span>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="ressources/thumb-3.jpg" alt="Miniature 3">
                    <div class="gallery-overlay">
                        <span>Voir plus</span>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="ressources/thumb-4.jpg" alt="Miniature 4">
                    <div class="gallery-overlay">
                        <span>Voir plus</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
```

#### 4.2 Styles CSS pour le carrousel

Ajoutez ces styles à votre `styles.css` :

```css
/* ======= CARROUSEL ======= */
.carousel {
    position: relative;
    max-width: 800px;
    margin: 0 auto 4rem;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
}

.carousel-container {
    position: relative;
    width: 100%;
    height: 500px;
}

.carousel-slide {
    display: none;
    position: relative;
    width: 100%;
    height: 100%;
}

.carousel-slide.active {
    display: block;
}

.carousel-slide img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.slide-info {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background: linear-gradient(transparent, rgba(0, 0, 0, 0.8));
    color: white;
    padding: 2rem;
    transform: translateY(100%);
    transition: transform 0.3s ease;
}

.carousel-slide:hover .slide-info {
    transform: translateY(0);
}

.slide-info h3 {
    font-size: 1.5rem;
    margin-bottom: 0.5rem;
}

/* Boutons de navigation */
.carousel-btn {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background: rgba(255, 255, 255, 0.8);
    border: none;
    font-size: 1.5rem;
    padding: 1rem;
    cursor: pointer;
    border-radius: 50%;
    transition: all 0.3s ease;
    z-index: 10;
}

.carousel-btn:hover {
    background: white;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}

.carousel-btn.prev {
    left: 20px;
}

.carousel-btn.next {
    right: 20px;
}

/* Indicateurs */
.carousel-indicators {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    gap: 10px;
}

.indicator {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.5);
    cursor: pointer;
    transition: background 0.3s ease;
}

.indicator.active {
    background: white;
}

/* ======= GALERIE ======= */
.gallery h3 {
    text-align: center;
    font-size: 2rem;
    margin-bottom: 2rem;
    color: #2c3e50;
}

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    margin-top: 2rem;
}

.gallery-item {
    position: relative;
    border-radius: 10px;
    overflow: hidden;
    transition: transform 0.3s ease;
}

.gallery-item:hover {
    transform: scale(1.05);
}

.gallery-item img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    transition: transform 0.3s ease;
}

.gallery-overlay {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(231, 76, 60, 0.8);
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-weight: bold;
    opacity: 0;
    transition: opacity 0.3s ease;
}

.gallery-item:hover .gallery-overlay {
    opacity: 1;
}

.gallery-item:hover img {
    transform: scale(1.1);
}
```

#### 4.3 JavaScript pour le carrousel

Créez un fichier `script.js` à coté du fichier index.html et styles.css et ajoutez ce code :

```javascript
// Variables globales
let currentSlideIndex = 0;
const slides = document.querySelectorAll('.carousel-slide');
const indicators = document.querySelectorAll('.indicator');

// Fonction pour changer de slide
function changeSlide(direction) {
    // Retirer la classe active de la slide actuelle
    slides[currentSlideIndex].classList.remove('active');
    indicators[currentSlideIndex].classList.remove('active');
    
    // Calculer le nouvel index
    currentSlideIndex += direction;
    
    // Gérer le bouclage
    if (currentSlideIndex >= slides.length) {
        currentSlideIndex = 0;
    }
    if (currentSlideIndex < 0) {
        currentSlideIndex = slides.length - 1;
    }
    
    // Ajouter la classe active à la nouvelle slide
    slides[currentSlideIndex].classList.add('active');
    indicators[currentSlideIndex].classList.add('active');
}

// Fonction pour aller à une slide spécifique
function currentSlide(n) {
    slides[currentSlideIndex].classList.remove('active');
    indicators[currentSlideIndex].classList.remove('active');
    
    currentSlideIndex = n - 1;
    
    slides[currentSlideIndex].classList.add('active');
    indicators[currentSlideIndex].classList.add('active');
}

// Défilement automatique (optionnel)
function autoSlide() {
    changeSlide(1);
}

// Démarrer le défilement automatique toutes les 5 secondes
setInterval(autoSlide, 5000);

// Permettre la navigation au clavier
document.addEventListener('keydown', function(e) {
    if (e.key === 'ArrowLeft') {
        changeSlide(-1);
    } else if (e.key === 'ArrowRight') {
        changeSlide(1);
    }
});
```

N'oubliez pas d'ajouter le script à votre HTML avant la fermeture du body :

```html
<script src="script.js"></script>
</body>
</html>
```

🎯 **MAÎTRISE JAVASCRIPT & INTERACTIVITÉ** :

1. **Test complet** :
   - Cliquez sur les flèches ← →
   - Cliquez sur les points indicateurs
   - Utilisez les flèches du clavier
   - Attendez 5 secondes pour voir le défilement automatique
2. **Compréhension du code** :
   - Expliquez ce que fait la fonction `changeSlide()`
3. **Expérimentations** :
   - Changez `setInterval(autoSlide, 5000)` à `3000`. Que se passe-t-il ?
4. **Partage de groupe** : Essayer de lire le code et supposer ce que fait chaque ligne. Discutez en avec votre binôme

🧠 **Concept fondamental** : JavaScript manipule le DOM (Document Object Model). En gros n'importe quel partie HTML ou CSS de la page. C'est lui qui permet le mouvement et la plupart des animations dans les pages.

💼 **Personalisation** : Vous pouvez changer et/ou ajouter des images de slides, elles sont au format 2000*1000px et les miniatures en 500 par 300px

### 🚀 Étape 5 : Optimisation et Validation (30min)

**Objectif** : Optimiser les performances et valider le code

🏁 **Dernière ligne droite** : Vous avez un site qui fonctionne ! Maintenant, rendons-le professionnel avec les bonnes pratiques.

#### 5.1 Optimisation des médias

Convertir les images au format webp. Réfléchir aux autres optimisations possibles sur les médias.

#### 5.2 Optimisation CSS

Ajoutez ces optimisations :

```css
/* Optimisations de performance */
.carousel-slide img,
.gallery-item img {
    will-change: transform;
}

/* Réduction de motion pour l'accessibilité */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
    }
}
```

#### 5.3 Validation

1. **HTML** : Allez sur [validator.w3.org](https://validator.w3.org)
2. **CSS** : Allez sur [jigsaw.w3.org/css-validator](https://jigsaw.w3.org/css-validator/)

🎖️ **FINALISATION & QUALITÉ PRO** :

1. **Tests de validation** :
   - Validez votre HTML et corrigez les erreurs
   - Validez votre CSS et analysez les warnings
2. **Performance** :
   - Ouvrez F12 → Lighthouse → Générer un rapport
   - Analysez vos scores Performance, Accessibilité, SEO
   - Qu'est-ce qui peut être amélioré ?
3. **Questions de professionnalisation** :
   - Pourquoi valider son code est-il important ?
4. **Test utilisateur** :
   - Faites tester votre site par un autre binôme
   - Notez leurs retours UX
   - Qu'est-ce qui les a surpris positivement/négativement ?
5. **Auto-évaluation** :
   - Sur une échelle de 1 à 10, comment notez-vous votre site ?
   - Quelles sont vos 3 fiertés dans ce projet ?
   - Qu'aimeriez-vous améliorer ?
🏆 **Bravo !** Vous venez de créer un portfolio professionnel complet ! Ce type de projet vaut 500-1500€ sur le marché freelance.

---

## 🔄 Pause Réflexion Finale (10 min)

**Moment de fierté** : Regardez le chemin parcouru !

**Comparez :**

- Votre fichier HTML vide du début VS votre portfolio complet maintenant
- Votre niveau de confiance en CSS/JS avant VS maintenant
- Votre compréhension du "responsive" avant VS maintenant

**Question de projection :**
Si vous deviez vendre ce portfolio à un vrai client, quel prix demanderiez-vous et pourquoi ?

---

## 🎨 Améliorations Suggérées

1. **Lightbox** : Ajouter une lightbox pour voir les images en grand
2. **Filtres** : Système de filtres par catégorie
3. **Lazy Loading** : Chargement différé des images
4. **Mode sombre** : Toggle pour basculer entre thème clair/sombre
5. **Contact Form** : Formulaire de contact fonctionnel

## 📝 Checklist de Validation

- [ ] Page responsive sur mobile, tablette et desktop
- [ ] Carrousel fonctionnel avec navigation
- [ ] Galerie avec effets de survol
- [ ] Animations fluides
- [ ] Code HTML valide
- [ ] Code CSS valide
- [ ] Performance optimisée
- [ ] Accessibilité respectée

## 🤔 Bilan & Réflexion Collective

💬 **Session de debriefing** : Prenez 15 minutes en groupe pour échanger

### Questions de réflexion individuelle

1. **Apprentissage** : Quelle technique avez-vous trouvée la plus difficile ? La plus intéressante ?
2. **Compréhension** : Expliquez en une phrase ce qu'est le responsive design
3. **Créativité** : Si vous deviez refaire ce projet, que changeriez-vous dans le design ?

### Discussion de groupe

- **Partage d'expérience** : Quels ont été vos moments "eurêka" ?
- **Entraide** : Quelles astuces avez-vous découvertes pour déboguer ?
- **Perspectives** : Quels projets aimeriez-vous réaliser maintenant ?

### Auto-évaluation

**Je me sens capable de** :

- [ ] Créer une structure HTML sémantique
- [ ] Appliquer des styles CSS simples
- [ ] Rendre un site responsive
- [ ] Intégrer des vidéos, diaporama
- [ ] Valider et déboguer mon code

**Mes prochains objectifs** :

- [ ] Apprendre un framework CSS (Bootstrap, Tailwind)
- [ ] Approfondir JavaScript
- [ ] Optimiser un site pour la performance
- [ ] Mise en ligne

## 🏆 Résultat Final

Vous devriez avoir un portfolio élégant et moderne avec :

- ✅ Design responsive
- ✅ Carrousel interactif
- ✅ Galerie avec effets
- ✅ Animations CSS
- ✅ Code optimisé

**Bravo !** Vous avez créé une vitrine numérique professionnelle pour Éléonore ! 🎉
