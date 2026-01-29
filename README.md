# Orlando-digital-marketing-
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Orlando Tech | Orlando Digital X Marketing</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;600;800&family=Fira+Code:wght@400;500&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg: #050608;
            --card: #111522;
            --primary: #00f5a2;
            --accent: #00e5ff;
            --text: #f5f5f7;
            --muted: #a4afc4;
        }

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg);
            background: radial-gradient(circle at top, #1b2646, #050608 60%);
            color: var(--text);
            scroll-behavior: smooth;
        }

        .glass {
            background: rgba(17, 21, 34, 0.8);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 24px;
        }

        .gradient-text {
            background: linear-gradient(135deg, var(--accent), var(--primary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .nav-link {
            position: relative;
            transition: color 0.3s;
        }

        .nav-link::after {
            content: '';
            position: absolute;
            width: 0; height: 2px;
            bottom: -4px; left: 0;
            background: var(--primary);
            transition: width 0.3s;
        }

        .nav-link:hover::after { width: 100%; }

        /* Animation simple pour le terminal */
        @keyframes blink { 50% { opacity: 0; } }
        .cursor { animation: blink 1s infinite; }

        .mobile-menu {
            transform: translateY(-100%);
            transition: transform 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .mobile-menu.active { transform: translateY(0); }
    </style>
</head>
<body class="overflow-x-hidden">

    <header class="fixed w-full z-50 top-0 left-0 bg-black/50 backdrop-blur-xl border-b border-white/5">
        <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 rounded-full bg-gradient-to-tr from-cyan-500 to-emerald-400 flex items-center justify-center font-bold text-black text-xl shadow-[0_0_20px_rgba(0,245,162,0.4)]">
                    O
                </div>
                <div class="flex flex-col leading-none">
                    <span class="font-extrabold text-sm tracking-widest uppercase">Orlando Tech</span>
                    <span class="text-[10px] text-muted uppercase tracking-[0.2em]">Digital X Marketing</span>
                </div>
            </div>

            <nav class="hidden lg:flex items-center gap-8 text-[11px] font-bold uppercase tracking-widest text-muted">
                <a href="#accueil" class="nav-link hover:text-white">Accueil</a>
                <a href="#services" class="nav-link hover:text-white">Services</a>
                <a href="#portfolio" class="nav-link hover:text-white">Portfolio</a>
                <a href="#competences" class="nav-link hover:text-white">Compétences</a>
                <a href="#propos" class="nav-link hover:text-white">À propos</a>
                <a href="#contact" class="bg-primary text-black px-5 py-2 rounded-full hover:scale-105 transition active:scale-95">Me Contacter</a>
            </nav>

            <button id="menu-btn" class="lg:hidden flex flex-col gap-1.5">
                <span class="w-6 h-0.5 bg-white"></span>
                <span class="w-6 h-0.5 bg-white"></span>
                <span class="w-6 h-0.5 bg-white"></span>
            </button>
        </div>
    </header>

    <div id="mobile-menu" class="fixed inset-0 bg-black z-40 mobile-menu lg:hidden flex flex-col items-center justify-center gap-8 text-xl font-bold uppercase tracking-widest">
        <a href="#accueil" class="m-link">Accueil</a>
        <a href="#services" class="m-link">Services</a>
        <a href="#portfolio" class="m-link">Portfolio</a>
        <a href="#competences" class="m-link">Compétences</a>
        <a href="#propos" class="m-link">À propos</a>
        <a href="#contact" class="m-link text-primary border border-primary px-8 py-2 rounded-full">Contact</a>
    </div>

    <main>
        <section id="accueil" class="pt-40 pb-24 px-6 max-w-7xl mx-auto">
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div>
                    <div class="inline-block px-4 py-1 rounded-full border border-emerald-500/30 bg-emerald-500/5 text-primary text-[10px] font-bold uppercase tracking-widest mb-6">
                        ORLANDO TECH – Développeur web & marketing digital
                    </div>
                    <h1 class="text-5xl lg:text-7xl font-black leading-tight mb-8">
                        Je construis des solutions web <span class="gradient-text italic">modernes & sécurisées</span>
                    </h1>
                    <p class="text-muted text-lg leading-relaxed mb-10 max-w-xl">
                        Je suis Orlando Tech, passionné de cybersécurité et programmeur aguerri. Je maîtrise HTML, CSS, JavaScript, Python et Golang pour offrir aux entreprises une présence digitale d'élite.
                    </p>
                    <div class="flex flex-wrap gap-4 mb-12">
                        <a href="#services" class="bg-primary text-black font-extrabold px-8 py-4 rounded-2xl hover:shadow-[0_0_30px_rgba(0,245,162,0.3)] transition">Voir mes services</a>
                        <a href="#portfolio" class="border border-white/10 bg-white/5 font-extrabold px-8 py-4 rounded-2xl hover:bg-white/10 transition">Voir mon portfolio</a>
                    </div>
                    <div class="grid grid-cols-3 gap-8 pt-8 border-t border-white/5">
                        <div><strong class="text-3xl font-black block">3+</strong><span class="text-[10px] text-muted uppercase font-bold">Projets Web</span></div>
                        <div><strong class="text-3xl font-black block">100%</strong><span class="text-[10px] text-muted uppercase font-bold">Marketing Digital</span></div>
                        <div><strong class="text-3xl font-black block">PRO</strong><span class="text-[10px] text-muted uppercase font-bold">Cybersécurité</span></div>
                    </div>
                </div>

                <div class="relative">
                    <div class="glass p-8 relative z-10">
                        <div class="flex items-center gap-4 mb-8">
                            <div class="w-14 h-14 rounded-2xl bg-white/5 flex items-center justify-center text-3xl">👨‍💻</div>
                            <div>
                                <h3 class="font-bold text-xl leading-none mb-1">Freelance Tech</h3>
                                <p class="text-xs text-primary font-mono uppercase tracking-widest">Available for Hire</p>
                            </div>
                        </div>
                        <p class="text-sm text-muted leading-relaxed mb-8">
                            En tant que professionnel de la tech, je conçois vos sites, gère votre marketing digital, et j'optimise votre infrastructure avec les meilleures pratiques de cybersécurité.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-8">
                            <span class="text-[10px] font-bold px-3 py-1 rounded-md bg-white/5 border border-white/10 uppercase">Développeur Web</span>
                            <span class="text-[10px] font-bold px-3 py-1 rounded-md bg-white/5 border border-white/10 uppercase">Marketing Digital</span>
                            <span class="text-[10px] font-bold px-3 py-1 rounded-md bg-white/5 border border-white/10 uppercase">Cybersécurité</span>
                        </div>
                        <div class="rounded-xl overflow-hidden border border-white/10">
                            <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&q=80" alt="Tech Dashboard" class="w-full opacity-60">
                        </div>
                    </div>
                    <div class="absolute -top-10 -right-10 w-64 h-64 bg-accent/20 rounded-full blur-[100px]"></div>
                </div>
            </div>
        </section>

        <section id="services" class="py-24 px-6 max-w-7xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-black uppercase mb-4 tracking-tighter">Mes Services <span class="gradient-text italic">Premium</span></h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="glass p-8 group hover:border-primary/50 transition">
                    <div class="text-3xl mb-6">💻</div>
                    <h3 class="text-xl font-bold mb-4 uppercase">Développeur Web</h3>
                    <p class="text-sm text-muted mb-6">Création de sites vitrines, landing pages et sites responsives modernes.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="text-[10px] font-mono text-primary">#HTML</span>
                        <span class="text-[10px] font-mono text-primary">#CSS</span>
                        <span class="text-[10px] font-mono text-primary">#JavaScript</span>
                    </div>
                </div>
                <div class="glass p-8 group hover:border-primary/50 transition">
                    <div class="text-3xl mb-6">📈</div>
                    <h3 class="text-xl font-bold mb-4 uppercase">Marketing Digital</h3>
                    <p class="text-sm text-muted mb-6">Gestion de présence sur réseaux sociaux, branding et stratégie de croissance.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="text-[10px] font-mono text-primary">#TikTok</span>
                        <span class="text-[10px] font-mono text-primary">#Branding</span>
                        <span class="text-[10px] font-mono text-primary">#Instagram</span>
                    </div>
                </div>
                <div class="glass p-8 group hover:border-primary/50 transition">
                    <div class="text-3xl mb-6">🛡️</div>
                    <h3 class="text-xl font-bold mb-4 uppercase">Cybersécurité</h3>
                    <p class="text-sm text-muted mb-6">Sensibilisation, audit basique et mise en place de bonnes habitudes de sécurité.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="text-[10px] font-mono text-primary">#Protection</span>
                        <span class="text-[10px] font-mono text-primary">#Audit</span>
                        <span class="text-[10px] font-mono text-primary">#Sécurité</span>
                    </div>
                </div>
                <div class="glass p-8 group hover:border-primary/50 transition">
                    <div class="text-3xl mb-6">🎨</div>
                    <h3 class="text-xl font-bold mb-4 uppercase">Branding & Contenu</h3>
                    <p class="text-sm text-muted mb-6">Identité visuelle, logos et création de contenus percutants.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="text-[10px] font-mono text-primary">#Logo</span>
                        <span class="text-[10px] font-mono text-primary">#Design</span>
                    </div>
                </div>
                <div class="glass p-8 group hover:border-primary/50 transition">
                    <div class="text-3xl mb-6">🚀</div>
                    <h3 class="text-xl font-bold mb-4 uppercase">Optimisation SEO</h3>
                    <p class="text-sm text-muted mb-6">Vitesse de chargement et structure technique pour le référencement.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="text-[10px] font-mono text-primary">#SEO</span>
                        <span class="text-[10px] font-mono text-primary">#Performance</span>
                    </div>
                </div>
                <div class="glass p-8 group hover:border-primary/50 transition">
                    <div class="text-3xl mb-6">🤝</div>
                    <h3 class="text-xl font-bold mb-4 uppercase">Conseil & Accompagnement</h3>
                    <p class="text-sm text-muted mb-6">De l'idée au lancement : je vous coache pour votre réussite digitale.</p>
                    <div class="flex flex-wrap gap-2">
                        <span class="text-[10px] font-mono text-primary">#Stratégie</span>
                        <span class="text-[10px] font-mono text-primary">#Coaching</span>
                    </div>
                </div>
            </div>
        </section>

        <section id="competences" class="py-24 px-6 bg-white/5">
            <div class="max-w-7xl mx-auto">
                <div class="text-center mb-16">
                    <h2 class="text-4xl font-black uppercase tracking-tighter italic">Compétences <span class="text-primary tracking-normal">Techniques</span></h2>
                </div>
                <div class="grid grid-cols-2 lg:grid-cols-5 gap-4 text-center">
                    <div class="glass p-6">
                        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" class="w-12 h-12 mx-auto mb-4" alt="HTML">
                        <h4 class="font-bold">HTML5</h4>
                        <p class="text-[10px] text-muted mt-2 uppercase">Structure moderne</p>
                    </div>
                    <div class="glass p-6 border-b-2 border-b-primary">
                        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" class="w-12 h-12 mx-auto mb-4" alt="CSS">
                        <h4 class="font-bold">CSS3</h4>
                        <p class="text-[10px] text-muted mt-2 uppercase">Design Responsive</p>
                    </div>
                    <div class="glass p-6">
                        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" class="w-12 h-12 mx-auto mb-4" alt="JS">
                        <h4 class="font-bold">JavaScript</h4>
                        <p class="text-[10px] text-muted mt-2 uppercase">Interactions</p>
                    </div>
                    <div class="glass p-6 border-b-2 border-b-primary">
                        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" class="w-12 h-12 mx-auto mb-4" alt="Python">
                        <h4 class="font-bold">Python</h4>
                        <p class="text-[10px] text-muted mt-2 uppercase">Automatisation</p>
                    </div>
                    <div class="glass p-6">
                        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/go/go-original-wordmark.svg" class="w-12 h-12 mx-auto mb-4" alt="Golang">
                        <h4 class="font-bold">Golang</h4>
                        <p class="text-[10px] text-muted mt-2 uppercase">Backend Haute Performance</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="portfolio" class="py-24 px-6 max-w-7xl mx-auto">
            <div class="text-center max-w-2xl mx-auto mb-16">
                <h2 class="text-4xl font-black uppercase mb-4 tracking-tighter italic">Portfolio</h2>
                <p class="text-muted text-sm">Découvrez comment j'allie programmation et marketing digital pour créer des expériences uniques.</p>
                    </div>
                </div>
                <div class="glass overflow-hidden group">
                    <div class="h-40 bg-gray-900">
                        <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&q=80" alt="Projet" class="w-full h-full object-cover group-hover:scale-110 transition duration-500 opacity-60">
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold uppercase text-sm mb-1">Dashboard Marketing</h4>
                        <p class="text-[10px] text-muted">Analyse de données en temps réel.</p>
                    </div>
                </div>
                <div class="glass overflow-hidden group">
                    <div class="h-40 bg-gray-900">
                        <img src="https://images.unsplash.com/photo-1563986768609-322da13575f3?auto="format"&fit=crop&q=80" alt="Projet" class="w-full h-full object-cover group-hover:scale-110 transition duration-500 opacity-60">
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold uppercase text-sm mb-1">Portfolio Design</h4>
                        <p class="text-[10px] text-muted">Structure épurée et responsive.</p>
                    </div>
                </div>
                <div class="glass overflow-hidden group">
                    <div class="h-40 bg-gray-900">
                        <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?auto=format&fit=crop&q=80" alt="Projet" class="w-full h-full object-cover group-hover:scale-110 transition duration-500 opacity-60">
                    </div>
                    <div class="p-4">
                        <h4 class="font-bold uppercase text-sm mb-1">Audit Sécurité API</h4>
                        <p class="text-[10px] text-muted">Sécurisation de flux de données.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="propos" class="py-24 px-6 max-w-7xl mx-auto border-t border-white/5">
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div class="glass p-10">
                    <h2 class="text-3xl font-black mb-8 uppercase italic">À propos de <span class="text-primary italic">moi</span></h2>
                    <p class="text-muted leading-relaxed mb-6">
                        Orlando Tech n'est pas qu'une marque, c'est une expertise. Passionné par le code et la protection des données, j'aide les entrepreneurs à bâtir une présence digitale forte et cohérente.
                    </p>
                    <ul class="space-y-4 text-sm font-semibold italic">
                        <li class="flex items-center gap-3 text-primary"><span class="text-white">▹</span> Conception de sites modernes</li>
                        <li class="flex items-center gap-3 text-primary"><span class="text-white">▹</span> Intégration responsive multi-langages</li>
                        <li class="flex items-center gap-3 text-primary"><span class="text-white">▹</span> Stratégie marketing TikTok/Insta</li>
                        <li class="flex items-center gap-3 text-primary"><span class="text-white">▹</span> Bases de cybersécurité industrielle</li>
                    </ul>
                </div>
                <div class="rounded-[40px] overflow-hidden border border-white/10 shadow-2xl rotate-2 hover:rotate-0 transition duration-700">
                    <img src="https://images.unsplash.com/photo-1550439062-609e1531270e?auto=format&fit=crop&q=80" alt="Orlando Tech" class="w-full h-full object-cover">
                </div>
            </div>
        </section>

        <section id="contact" class="py-24 px-6 max-w-7xl mx-auto">
            <div class="grid lg:grid-cols-2 gap-16">
                <div>
                    <h2 class="text-4xl font-black mb-6 uppercase tracking-tighter italic">On travaille <br> <span class="text-primary italic">ensemble ?</span></h2>
                    <p class="text-muted mb-12">Ouvert aux projets web, marketing et collaborations techniques.</p>
                    
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div class="glass p-6">
                            <span class="text-[10px] uppercase font-bold text-muted block mb-2 tracking-[0.2em]">Email</span>
                            <a href="mailto:orlandodigitalmarketing01@gmail.com" class="font-bold text-xs break-all">orlandodigitalmarketing01@gmail.com</a>
                        </div>
                        <div class="glass p-6">
                            <span class="text-[10px] uppercase font-bold text-muted block mb-2 tracking-[0.2em]">WhatsApp</span>
                            <a href="https://wa.me/50935443504" class="font-bold text-sm tracking-widest">+509 3544-3504</a>
                        </div>
                        <div class="glass p-6">
                            <span class="text-[10px] uppercase font-bold text-muted block mb-2 tracking-[0.2em]">Instagram</span>
                            <a href="https://www.instagram.com/orlando_digital_x_marketing" class="font-bold text-xs">@orlando_digital</a>
                        </div>
                        <div class="glass p-6">
                            <span class="text-[10px] uppercase font-bold text-muted block mb-2 tracking-[0.2em]">TikTok</span>
                            <a href="https://www.tiktok.com/@orlando_digital_" class="font-bold text-xs">@orlando_digital_</a>
                        </div>
                    </div>
                </div>

                <div class="glass p-10">
                    <form class="flex flex-col gap-6">
                        <div class="flex flex-col gap-2">
                            <label class="text-[10px] font-bold uppercase tracking-widest text-muted">Nom complet</label>
                            <input type="text" placeholder="Orlando-tech" class="bg-white/5 border border-white/10 p-4 rounded-xl focus:outline-none focus:border-primary transition">
                        </div>
                        <div class="flex flex-col gap-2">
                            <label class="text-[10px] font-bold uppercase tracking-widest text-muted">Email</label>
                            <input type="email" placeholder="orlandomarketing01@gmail.com" class="bg-white/5 border border-white/10 p-4 rounded-xl focus:outline-none focus:border-primary transition">
                        </div>
                        <div class="flex flex-col gap-2">
                            <label class="text-[10px] font-bold uppercase tracking-widest text-muted">Message pas encore prêt</label>
                            <textarea rows="4" placeholder="Votre projet..." class="bg-white/5 border border-white/10 p-4 rounded-xl focus:outline-none focus:border-primary transition"></textarea>
                        </div>
                        <button type="button" class="bg-primary text-black font-black p-4 rounded-xl hover:shadow-[0_0_30px_rgba(0,245,162,0.3)] transition">Envoyer un message a Orlando-tech</button>
                    </form>
                </div>
            </div>
        </section>
    </main>

    <footer class="py-12 border-t border-white/5 px-6">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-6">
            <div>
                <span class="font-black text-xl italic uppercase">Orlando <span class="text-primary">Digital X</span></span>
            </div>
            <p class="text-muted text-[10px] uppercase tracking-widest font-bold">Transforme tes idées en solutions digitales modernes.</p>
            <p class="text-muted text-[10px] uppercase font-bold">© 2026 Tous droits réservés.</p>
        </div>
    </footer>

    <script>
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const mLinks = document.querySelectorAll('.m-link');

        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('active');
        });

        mLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.remove('active');
            });
        });

        // Smooth Scroll pour tous les liens
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
