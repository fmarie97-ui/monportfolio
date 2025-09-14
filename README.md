# monportfolio
ajout de mon site @
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marie F. - Créatrice de Sites Web</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
        }

        /* Header */
        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .header h1 {
            font-size: 3rem;
            margin-bottom: 0.5rem;
            animation: fadeInUp 1s ease;
        }

        .header p {
            font-size: 1.2rem;
            opacity: 0.9;
            animation: fadeInUp 1s ease 0.2s both;
        }

        /* Navigation */
        .nav {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .nav-container {
            display: flex;
            justify-content: center;
            gap: 2rem;
        }

        .nav a {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 25px;
            transition: all 0.3s ease;
        }

        .nav a:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-2px);
        }

        /* Sections */
        .section {
            padding: 4rem 0;
        }

        .section:nth-child(even) {
            background: #f8f9fa;
        }

        .section h2 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 2rem;
            color: #667eea;
        }

        /* Services Grid */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .service-card {
            background: white;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .service-card h3 {
            color: #667eea;
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }

        .price {
            font-size: 1.8rem;
            color: #764ba2;
            font-weight: bold;
            margin-top: 1rem;
        }

        .price-detail {
            font-size: 0.9rem;
            color: #666;
            margin-top: 0.5rem;
        }

        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 3rem;
            align-items: center;
            margin-top: 2rem;
        }

        .profile-img {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea, #764ba2);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 4rem;
            margin: 0 auto;
        }

        .about-text {
            font-size: 1.1rem;
            line-height: 1.8;
        }

        /* Process Steps */
        .process-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .step {
            text-align: center;
            position: relative;
        }

        .step-number {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            font-weight: bold;
            margin: 0 auto 1rem;
        }

        /* Contact Section */
        .contact {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            text-align: center;
        }

        .contact-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .contact-item {
            padding: 1.5rem;
            border-radius: 10px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
        }

        .contact-item h3 {
            margin-bottom: 0.5rem;
            font-size: 1.2rem;
        }

        /* CTA Button */
        .cta-button {
            display: inline-block;
            background: #ff6b6b;
            color: white;
            padding: 1rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1rem;
            margin-top: 2rem;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(255, 107, 107, 0.4);
        }

        .cta-button:hover {
            background: #ff5252;
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(255, 107, 107, 0.6);
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

        /* Responsive */
        @media (max-width: 768px) {
            .header h1 {
                font-size: 2rem;
            }
            
            .about-content {
                grid-template-columns: 1fr;
                text-align: center;
            }
            
            .nav-container {
                flex-direction: column;
                gap: 1rem;
            }
            
            .section {
                padding: 2rem 0;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <h1>Marie F.</h1>
            <p>Créatrice de Sites Web Professionnels | Tarifs Débutant Accessibles</p>
        </div>
        <nav class="nav">
            <div class="nav-container">
                <a href="#services">Services</a>
                <a href="#about">À propos</a>
                <a href="#process">Processus</a>
                <a href="#contact">Contact</a>
            </div>
        </nav>
    </header>

    <!-- Services Section -->
    <section id="services" class="section">
        <div class="container">
            <h2>Mes Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">🌐</div>
                    <h3>Site Vitrine</h3>
                    <p>Site professionnel pour présenter votre activité. Design moderne, responsive et optimisé pour Google.</p>
                    <div class="price">400€</div>
                    <div class="price-detail">Tarif spécial débutant • Livraison 7-10 jours</div>
                </div>
                <div class="service-card">
                    <div class="service-icon">🛒</div>
                    <h3>Site E-commerce</h3>
                    <p>Boutique en ligne simple avec paiement sécurisé et gestion des produits. Idéal pour débuter la vente en ligne.</p>
                    <div class="price">800€</div>
                    <div class="price-detail">Configuration complète • Formation incluse</div>
                </div>
                <div class="service-card">
                    <div class="service-icon">🔧</div>
                    <h3>Maintenance</h3>
                    <p>Mises à jour de sécurité, sauvegardes automatiques et modifications mineures de contenu.</p>
                    <div class="price">50€/mois</div>
                    <div class="price-detail">Sans engagement • Support par email</div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section">
        <div class="container">
            <h2>À Propos</h2>
            <div class="about-content">
                <div class="profile-img">MF</div>
                <div class="about-text">
                    <p><strong>Développeuse web débutante passionnée</strong>, je me lance dans l'aventure de la création de sites internet avec des tarifs adaptés aux petites entreprises et entrepreneurs.</p>
                    
                    <p>Mon objectif ? Vous accompagner dans votre transformation digitale sans vous ruiner. Je propose des <strong>tarifs accessibles</strong> car je débute dans le métier, tout en garantissant un travail professionnel et soigné.</p>
                    
                    <p>Que vous soyez artisan, commerçant, thérapeute ou entrepreneur, je mets toute ma motivation à votre service pour créer le site web qui vous ressemble. <strong>Qualité professionnelle à prix débutant !</strong></p>
                    
                    <p><em>Idéal pour les petits budgets qui veulent un vrai site professionnel.</em></p>
                </div>
            </div>
        </div>
    </section>

    <!-- Process Section -->
    <section id="process" class="section">
        <div class="container">
            <h2>Mon Processus</h2>
            <div class="process-steps">
                <div class="step">
                    <div class="step-number">1</div>
                    <h3>Consultation Gratuite</h3>
                    <p>Échange de 30 minutes sur vos besoins et objectifs</p>
                </div>
                <div class="step">
                    <div class="step-number">2</div>
                    <h3>Devis Transparent</h3>
                    <p>Proposition claire avec tarifs fixes, pas de surprises</p>
                </div>
                <div class="step">
                    <div class="step-number">3</div>
                    <h3>Création</h3>
                    <p>Développement avec aperçus réguliers pour validation</p>
                </div>
                <div class="step">
                    <div class="step-number">4</div>
                    <h3>Formation</h3>
                    <p>Je vous explique comment gérer votre site facilement</p>
                </div>
                <div class="step">
                    <div class="step-number">5</div>
                    <h3>Suivi</h3>
                    <p>Support gratuit 1 mois après livraison</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section contact">
        <div class="container">
            <h2>Contactez-moi</h2>
            <div class="contact-info">
                <div class="contact-item">
                    <h3>📧 Email</h3>
                    <p>marie.f@exemple.com</p>
                </div>
                <div class="contact-item">
                    <h3>📱 Téléphone</h3>
                    <p>06 XX XX XX XX</p>
                </div>
                <div class="contact-item">
                    <h3>💻 Portfolio</h3>
                    <p>www.marie-web.com</p>
                </div>
            </div>
            <a href="#" class="cta-button">Consultation Gratuite de 30min !</a>
            <p style="margin-top: 1rem; opacity: 0.8;">Réponse sous 24h garantie • Tarifs fixes sans surprise</p>
        </div>
    </section>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add scroll effect to service cards
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animation = 'fadeInUp 0.6s ease forwards';
                }
            });
        });

        document.querySelectorAll('.service-card, .step').forEach(card => {
            observer.observe(card);
        });
    </script>
</body>
</html>
