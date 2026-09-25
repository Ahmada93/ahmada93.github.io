```
"Excellence École" → Complexe At-Tidiani

"123 Avenue de l'Éducation" → Keur Massar Firdawsi

"+33 1 23 45 67 89" → 774814701

"contact@excellence-ecole.fr" → mouhamedpslgueye001@gmail.com

Les sections de programmes → Français et Franco-arabe 

Les actualités → journées d'inauguration le 27 septembre 2026 à Apix 
```

---

##  **Exemple: Changer la Couleur Principale**

Trouvez cette ligne au début du CSS:
```css
--primary: #667eea;  /* Vert */
```

Changez-la par:
```css
--primary: #ff6b6b;  /* Rouge */
--primary: #1dd1a1;  /* Vert */
--primary: #feca57;  /* Jaune */
```

---

##  **Points Forts du Design:**

 **Couleurs modernes** - Bleu + violet + blanc  
 **Animations fluides** - Transitions douces  
 **Mobile-first** - Parfait sur téléphone  
 **Accessible** - Lisible pour tous  
 **SEO-friendly** - Bien classé Google  
 **Formulaire** - Validation des données  

---

##  **Prochaines Étapes:**

1. **Téléchargez** le fichier
2. **Ouvrez-le** dans votre navigateur pour le tester
3. **Modifiez** le contenu avec vos informations
4. **Uploadez** sur GitHub Pages (gratuit & permanent)
5. **Partagez** le lien avec votre école!

**Votre site est déjà prêt à l'emploi!** Vous pouvez l'ouvrir directement dans votre navigateur. Si vous avez besoin de modifications ou d'ajouts, dites-moi!  
[24/09, 23:10] Sen Carrefour d'affaires At-tidiani: <!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Collège & Lycée - Excellence Académique</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #667eea;
            --secondary: #764ba2;
            --accent: #f093fb;
            --dark: #2d3436;
            --light: #f5f6fa;
            --success: #00b894;
            --danger: #d63031;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: var(--dark);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* =====================
           HEADER & NAVIGATION
           ===================== */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8em;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo-icon {
            font-size: 2em;
        }

        nav {
            display: flex;
            gap: 30px;
            align-items: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
            font-weight: 500;
        }

        nav a:hover {
            opacity: 0.8;
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5em;
            cursor: pointer;
        }

        /* =====================
           HERO SECTION
           ===================== */
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 150px 20px 100px;
            text-align: center;
            margin-top: 60px;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="%23ffffff" fill-opacity="0.1" d="M0,96L48,112C96,128,192,160,288,160C384,160,480,128,576,122.7C672,117,768,139,864,144C960,149,1056,139,1152,128C1248,117,1344,107,1392,101.3L1440,96L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>');
            background-repeat: no-repeat;
            background-position: bottom;
            background-size: cover;
            opacity: 0.5;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
            animation: slideInDown 0.8s ease;
        }

        .hero h1 {
            font-size: 3.5em;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .hero p {
            font-size: 1.3em;
            margin-bottom: 30px;
            opacity: 0.95;
        }

        .hero-buttons {
            display: flex;
            gap: 20px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 12px 30px;
            border: none;
            border-radius: 50px;
            font-size: 1em;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
            display: inline-block;
        }

        .btn-primary {
            background: white;
            color: var(--primary);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        .btn-secondary {
            background: rgba(255,255,255,0.2);
            color: white;
            border: 2px solid white;
        }

        .btn-secondary:hover {
            background: rgba(255,255,255,0.3);
            transform: translateY(-3px);
        }

        /* =====================
           SECTIONS
           ===================== */
        section {
            padding: 80px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 2.5em;
            margin-bottom: 50px;
            color: var(--dark);
            position: relative;
            padding-bottom: 20px;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            border-radius: 2px;
        }

        /* =====================
           À PROPOS
           ===================== */
        .about {
            background: var(--light);
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-text h3 {
            color: var(--primary);
            font-size: 1.5em;
            margin-bottom: 15px;
        }

        .about-text p {
            margin-bottom: 15px;
            color: #555;
            font-size: 1.05em;
        }

        .about-image {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border-radius: 10px;
            padding: 40px;
            text-align: center;
            color: white;
            font-size: 4em;
            min-height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        /* =====================
           PROGRAMMES
           ===================== */
        .programs {
            background: white;
        }

        .programs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .program-card {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s;
            border-top: 4px solid var(--primary);
        }

        .program-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }

        .program-icon {
            font-size: 2.5em;
            margin-bottom: 15px;
        }

        .program-card h3 {
            color: var(--primary);
            margin-bottom: 15px;
            font-size: 1.3em;
        }

        .program-card p {
            color: #666;
            margin-bottom: 15px;
        }

        .program-card ul {
            list-style: none;
            color: #666;
        }

        .program-card ul li {
            padding: 5px 0;
            padding-left: 25px;
            position: relative;
        }

        .program-card ul li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--success);
            font-weight: bold;
        }

        /* =====================
           GALERIE
           ===================== */
        .gallery {
            background: var(--light);
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            aspect-ratio: 1;
            cursor: pointer;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3em;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .gallery-item:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .gallery-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0,0,0,0.7);
            display: flex;
            align-items: flex-end;
            padding: 20px;
            color: white;
            opacity: 0;
            transition: opacity 0.3s;
        }

        .gallery-item:hover .gallery-overlay {
            opacity: 1;
        }

        /* =====================
           ACTUALITÉS
           ===================== */
        .news {
            background: white;
        }

        .news-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .news-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s;
        }

        .news-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .news-image {
            width: 100%;
            height: 200px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2em;
        }

        .news-content {
            padding: 25px;
        }

        .news-date {
            color: var(--primary);
            font-weight: 600;
            font-size: 0.9em;
            margin-bottom: 10px;
        }

        .news-card h3 {
            color: var(--dark);
            margin-bottom: 10px;
            font-size: 1.2em;
        }

        .news-card p {
            color: #666;
            margin-bottom: 15px;
        }

        .read-more {
            color: var(--primary);
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
        }

        .read-more:hover {
            color: var(--secondary);
        }

        /* =====================
           CONTACT FORM
           ===================== */
        .contact {
            background: var(--light);
        }

        .contact-wrapper {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
        }

        .contact-info h3 {
            color: var(--primary);
            font-size: 1.3em;
            margin-bottom: 20px;
        }

        .contact-item {
            margin-bottom: 30px;
            display: flex;
            gap: 15px;
        }

        .contact-icon {
            font-size: 1.5em;
            color: var(--primary);
            min-width: 30px;
        }

        .contact-item p {
            color: #666;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: var(--dark);
            font-weight: 600;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px 15px;
            border: 2px solid #ddd;
            border-radius: 5px;
            font-family: inherit;
            font-size: 1em;
            transition: border-color 0.3s;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--primary);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }

        .form-submit {
            width: 100%;
            padding: 12px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1em;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
        }

        .form-submit:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(102, 126, 234, 0.3);
        }

        .form-message {
            margin-top: 15px;
            padding: 15px;
            border-radius: 5px;
            text-align: center;
            font-weight: 600;
            display: none;
        }

        .form-message.success {
            background: #d4edda;
            color: #155724;
            display: block;
        }

        .form-message.error {
            background: #f8d7da;
            color: #721c24;
            display: block;
        }

        /* =====================
           FOOTER
           ===================== */
        footer {
            background: var(--dark);
            color: white;
            padding: 40px 20px 20px;
            margin-top: 50px;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-section h4 {
            margin-bottom: 15px;
            color: var(--primary);
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section ul li {
            margin-bottom: 10px;
        }

        .footer-section a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-section a:hover {
            color: white;
        }

        .footer-bottom {
            text-align: center;
            border-top: 1px solid #444;
            padding-top: 20px;
            color: #999;
        }

        /* =====================
           ANIMATIONS
           ===================== */
        @keyframes slideInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

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

        /* =====================
           RESPONSIVE
           ===================== */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2em;
            }

            .hero p {
                font-size: 1.05em;
            }

            .mobile-menu-btn {
                display: block;
            }

            nav {
                position: absolute;
                top: 100%;
                left: 0;
                right: 0;
                background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
                flex-direction: column;
                gap: 10px;
                padding: 20px;
                display: none;
                gap: 0;
            }

            nav.active {
                display: flex;
            }

            nav a {
                padding: 10px 0;
                border-bottom: 1px solid rgba(255,255,255,0.1);
            }

            .about-content {
                grid-template-columns: 1fr;
                gap: 30px;
            }

            .contact-wrapper {
                grid-template-columns: 1fr;
                gap: 30px;
            }

            .section-title {
                font-size: 1.8em;
            }

            .hero {
                padding: 100px 20px 60px;
                margin-top: 50px;
            }

            section {
                padding: 50px 20px;
            }
        }

        /* =====================
           SCROLL ANIMATIONS
           ===================== */
        .fade-in {
            animation: fadeInUp 0.8s ease forwards;
            opacity: 0;
        }

        .fade-in.visible {
            opacity: 1;
        }
    </style>
</head>
<body>
    <!-- =====================
         HEADER
         ===================== -->
    <header>
        <div class="nav-container">
            <div class="logo">
                <span class="logo-icon"> </span>
                <span>Excellence École</span>
            </div>
            <nav id="nav-menu">
                <a href="#accueil">Accueil</a>
                <a href="#about">À Propos</a>
                <a href="#programs">Programmes</a>
                <a href="#gallery">Galerie</a>
                <a href="#news">Actualités</a>
                <a href="#contact">Contact</a>
            </nav>
            <button class="mobile-menu-btn" onclick="toggleMenu()">☰</button>
        </div>
    </header>

    <!-- =====================
         HERO SECTION
         ===================== -->
    <section class="hero" id="accueil">
        <div class="hero-content">
            <h1>Bienvenue dans notre Établissement</h1>
            <p>Excellence académique, développement personnel et innovation pédagogique</p>
            <div class="hero-buttons">
                <button class="btn btn-primary" onclick="document.getElementById('contact').scrollIntoView()">Nous Contacter</button>
                <button class="btn btn-secondary" onclick="document.getElementById('programs').scrollIntoView()">Découvrir</button>
            </div>
        </div>
    </section>

    <!-- =====================
         À PROPOS
         ===================== -->
    <section class="about" id="about">
        <h2 class="section-title">À Propos de Notre École</h2>
        <div class="about-content">
            <div class="about-text">
                <h3>Notre Engagement</h3>
                <p>
                    Depuis plus de 20 ans, notre établissement s'engage à offrir une éducation de qualité à nos étudiants. Nous croyons en l'importance de combiner l'excellence académique avec le développement personnel.
                </p>
                <p>
                    Notre équipe pédagogique dévouée travaille chaque jour pour créer un environnement propice à l'apprentissage, où chaque étudiant peut s'épanouir et atteindre son plein potentiel.
                </p>
                <h3 style="margin-top: 30px;">Nos Valeurs</h3>
                <p>✓ Excellence académique</p>
                <p>✓ Respect et tolérance</p>
                <p>✓ Innovation pédagogique</p>
                <p>✓ Développement personnel</p>
            </div>
            <div class="about-image">
                 
            </div>
        </div>
    </section>

    <!-- =====================
         PROGRAMMES
         ===================== -->
    <section class="programs" id="programs">
        <h2 class="section-title">Nos Programmes</h2>
        <div class="programs-grid">
            <div class="program-card">
                <div class="program-icon"> </div>
                <h3>Sciences & Technologie</h3>
                <p>Un programme complet en sciences naturelles et technologie avec laboratoires modernes.</p>
                <ul>
                    <li>Physique-Chimie</li>
                    <li>Sciences de la Vie</li>
                    <li>Informatique</li>
                    <li>Robotique</li>
                </ul>
            </div>

            <div class="program-card">
                <div class="program-icon"> </div>
                <h3>Littérature & Humanités</h3>
                <p>Développez votre esprit critique et vos compétences en communication.</p>
                <ul>
                    <li>Français</li>
                    <li>Philosophie</li>
                    <li>Histoire-Géographie</li>
                    <li>Langues Étrangères</li>
                </ul>
            </div>

            <div class="program-card">
                <div class="program-icon"> </div>
                <h3>Arts & Culture</h3>
                <p>Explorez votre créativité à travers les arts, la musique et la culture.</p>
                <ul>
                    <li>Arts Plastiques</li>
                    <li>Musique</li>
                    <li>Théâtre</li>
                    <li>Cinéma</li>
                </ul>
            </div>

            <div class="program-card">
                <div class="program-icon"> </div>
                <h3>Sports & Bien-être</h3>
                <p>Activités sportives variées pour une bonne santé physique et mentale.</p>
                <ul>
                    <li>Éducation Physique</li>
                    <li>Football & Volley</li>
                    <li>Tennis</li>
                    <li>Yoga & Fitness</li>
                </ul>
            </div>

            <div class="program-card">
                <div class="program-icon"> </div>
                <h3>Préparation Professionnelle</h3>
                <p>Préparez votre avenir avec des stages et des modules professionnels.</p>
                <ul>
                    <li>Stages d'entreprise</li>
                    <li>Conseils d'orientation</li>
                    <li>CV & Entretiens</li>
                    <li>Networking</li>
                </ul>
            </div>

            <div class="program-card">
                <div class="program-icon"> </div>
                <h3>Programmes Internationaux</h3>
                <p>Échanges et programmes d'immersion dans d'autres pays.</p>
                <ul>
                    <li>Échanges Erasmus</li>
                    <li>Voyages Pédagogiques</li>
                    <li>Partenariats Internationaux</li>
                    <li>Certifications Langues</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- =====================
         GALERIE
         ===================== -->
    <section class="gallery" id="gallery">
        <h2 class="section-title">Notre Galerie</h2>
        <div class="gallery-grid">
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Campus Moderne</div>
            </div>
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Laboratoires</div>
            </div>
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Bibliothèque</div>
            </div>
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Salle des Arts</div>
            </div>
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Centre Sportif</div>
            </div>
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Espace Vert</div>
            </div>
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Salle Informatique</div>
            </div>
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Restaurant Scolaire</div>
            </div>
            <div class="gallery-item">
                 
                <div class="gallery-overlay">Amphithéâtre</div>
            </div>
        </div>
    </section>

    <!-- =====================
         ACTUALITÉS
         ===================== -->
    <section class="news" id="news">
        <h2 class="section-title">Actualités & Événements</h2>
        <div class="news-grid">
            <div class="news-card">
                <div class="news-image"> </div>
                <div class="news-content">
                    <div class="news-date">25 Janvier 2024</div>
                    <h3>Journée Portes Ouvertes</h3>
                    <p>Venez découvrir nos installations et rencontrer notre équipe pédagogique. Une occasion de explorer tous nos programmes et infrastructures.</p>
                    <a href="#" class="read-more">En savoir plus →</a>
                </div>
            </div>

            <div class="news-card">
                <div class="news-image"> </div>
                <div class="news-content">
                    <div class="news-date">15 Janvier 2024</div>
                    <h3>Succès aux Examens</h3>
                    <p>Nos élèves brillent aux examens nationaux avec un taux de réussite exceptionnel. Félicitations à tous nos étudiants!</p>
                    <a href="#" class="read-more">En savoir plus →</a>
                </div>
            </div>

            <div class="news-card">
                <div class="news-image"> </div>
                <div class="news-content">
                    <div class="news-date">5 Janvier 2024</div>
                    <h3>Échange International</h3>
                    <p>Nos étudiants participent à un programme d'échange de 3 mois avec nos partenaires allemands pour une immersion culturelle riche.</p>
                    <a href="#" class="read-more">En savoir plus →</a>
                </div>
            </div>
        </div>
    </section>

    <!-- =====================
         CONTACT
         ===================== -->
    <section class="contact" id="contact">
        <h2 class="section-title">Nous Contacter</h2>
        <div class="contact-wrapper">
            <div class="contact-info">
                <h3>Coordonnées</h3>
                
                <div class="contact-item">
                    <div class="contact-icon"> </div>
                    <p><strong>Adresse</strong><br>123 Avenue de l'Éducation<br>75000 Paris, France</p>
                </div>

                <div class="contact-item">
                    <div class="contact-icon"> </div>
                    <p><strong>Téléphone</strong><br>+33 1 23 45 67 89<br>+33 1 98 76 54 32</p>
                </div>

                <div class="contact-item">
                    <div class="contact-icon"> </div>
                    <p><strong>Email</strong><br>contact@excellence-ecole.fr<br>info@excellence-ecole.fr</p>
                </div>

                <div class="contact-item">
                    <div class="contact-icon"> </div>
                    <p><strong>Horaires</strong><br>Lundi - Vendredi: 8h - 18h<br>Samedi: 9h - 14h</p>
                </div>
            </div>

            <form onsubmit="handleSubmit(event)">
                <div class="form-group">
                    <label for="name">Nom Complet</label>
                    <input type="text" id="name" name="name" required>
                </div>

                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" name="email" required>
                </div>

                <div class="form-group">
                    <label for="phone">Téléphone</label>
                    <input type="tel" id="phone" name="phone">
                </div>

                <div class="form-group">
                    <label for="subject">Sujet</label>
                    <input type="text" id="subject" name="subject" required>
                </div>

                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea id="message" name="message" required></textarea>
                </div>

                <button type="submit" class="form-submit">Envoyer le Message</button>
                <div id="form-message" class="form-message"></div>
            </form>
        </div>
    </section>

    <!-- =====================
         FOOTER
         ===================== -->
    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h4>À Propos</h4>
                <ul>
                    <li><a href="#about">Notre École</a></li>
                    <li><a href="#programs">Nos Programmes</a></li>
                    <li><a href="#gallery">Nos Installations</a></li>
                    <li><a href="#news">Actualités</a></li>
                </ul>
            </div>

            <div class="footer-section">
                <h4>Programmes</h4>
                <ul>
                    <li><a href="#">Sciences & Technologie</a></li>
                    <li><a href="#">Littérature & Humanités</a></li>
                    <li><a href="#">Arts & Culture</a></li>
                    <li><a href="#">Sports & Bien-être</a></li>
                </ul>
            </div>

            <div class="footer-section">
                <h4>Ressources</h4>
                <ul>
                    <li><a href="#">Calendrier Scolaire</a></li>
                    <li><a href="#">Inscription</a></li>
                    <li><a href="#">Emploi du Temps</a></li>
                    <li><a href="#">Portail Élèves</a></li>
                </ul>
            </div>

            <div class="footer-section">
                <h4>Suivez-nous</h4>
                <ul>
                    <li><a href="#">Facebook</a></li>
                    <li><a href="#">Twitter</a></li>
                    <li><a href="#">Instagram</a></li>
                    <li><a href="#">LinkedIn</a></li>
                </ul>
            </div>
        </div>

        <div class="footer-bottom">
            <p>&copy; 2024 Excellence École - Tous droits réservés | <a href="#" style="color: #bbb;">Mentions Légales</a> | <a href="#" style="color: #bbb;">Politique de Confidentialité</a></p>
        </div>
    </footer>

    <script>
        // =====================
        // MENU MOBILE
        // =====================
        function toggleMenu() {
            const nav = document.getElementById('nav-menu');
            nav.classList.toggle('active');
        }

        // Fermer le menu au clic sur un lien
        document.querySelectorAll('#nav-menu a').forEach(link => {
            link.addEventListener('click', () => {
                document.getElementById('nav-menu').classList.remove('active');
            });
        });

        // =====================
        // FORMULAIRE DE CONTACT
        // =====================
        function handleSubmit(event) {
            event.preventDefault();

            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const phone = document.getElementById('phone').value;
            const subject = document.getElementById('subject').value;
            const message = document.getElementById('message').value;

            // Validation simple
            if (!name || !email || !subject || !message) {
                showMessage('  Veuillez remplir tous les champs obligatoires.', 'error');
                return;
            }

            if (!email.includes('@')) {
                showMessage('  Veuillez entrer une adresse email valide.', 'error');
                return;
            }

            // Simuler l'envoi
            const btn = event.target.querySelector('button[type="submit"]');
            btn.disabled = true;
            btn.textContent = 'Envoi en cours...';

            setTimeout(() => {
                showMessage('✓ Message envoyé avec succès! Nous vous répondrons bientôt.', 'success');
                document.querySelector('form').reset();
                btn.disabled = false;
                btn.textContent = 'Envoyer le Message';
            }, 1500);
        }

        function showMessage(text, type) {
            const messageDiv = document.getElementById('form-message');
            messageDiv.textContent = text;
            messageDiv.className = 'form-message ' + type;

            setTimeout(() => {
                messageDiv.style.display = 'none';
            }, 5000);
        }

        // =====================
        // ANIMATIONS AU SCROLL
        // =====================
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -100px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        // Observer les éléments
        document.querySelectorAll('.program-card, .news-card, .gallery-item').forEach(el => {
            el.classList.add('fade-in');
            observer.observe(el);
        });

        // =====================
        // SMOOTH SCROLL SUPPLÉMENTAIRE
        // =====================
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                const href = this.getAttribute('href');
                if (href !== '#' && document.querySelector(href)) {
                    e.preventDefault();
                }
            });
        });
    </script>
</body>
</html>
# ahmada93.github.io
