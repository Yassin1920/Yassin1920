<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Abed Mouhamed Yassin - Full Stack Developer</title>
    <!-- Font Awesome 6 -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet" />
    <style>
        /* --- RESET & BASE --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Inter', sans-serif;
            background: #f8f8f8;
            color: #010112;
            line-height: 1.6;
            padding: 2rem 1.5rem;
        }
        .container {
            max-width: 1100px;
            margin: 0 auto;
            background: #ffffff;
            border-radius: 2rem;
            box-shadow: 0 20px 40px -12px rgba(0, 0, 0, 0.12);
            padding: 2.5rem 2.8rem;
            transition: all 0.2s ease;
        }
        @media (max-width: 640px) {
            body {
                padding: 1rem 0.8rem;
            }
            .container {
                padding: 1.8rem 1.2rem;
                border-radius: 1.5rem;
            }
        }

        /* --- TYPOGRAPHY --- */
        h1, h2, h3 {
            font-weight: 700;
            letter-spacing: -0.02em;
        }
        h1 {
            font-size: 2.8rem;
            background: linear-gradient(145deg, #0b1120, #1e293b);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: inline-block;
        }
        h2 {
            font-size: 1.8rem;
            margin-top: 2.8rem;
            margin-bottom: 1.2rem;
            display: flex;
            align-items: center;
            gap: 0.6rem;
            border-bottom: 3px solid #e9edf2;
            padding-bottom: 0.6rem;
        }
        h2 i {
            color: #2563eb;
            font-size: 1.6rem;
            -webkit-text-fill-color: #2563eb;
        }
        h3 {
            font-size: 1.25rem;
            margin: 1.5rem 0 0.6rem;
            color: #0b1120;
        }
        .badge-role {
            display: inline-block;
            background: #bfeafc;
            color: #1e4f8a;
            font-weight: 600;
            font-size: 1.2rem;
            padding: 0.3rem 1.2rem;
            border-radius: 40px;
            letter-spacing: 0.3px;
            margin-top: 0.2rem;
        }
        .tagline {
            font-size: 1.1rem;
            color: #334155;
            max-width: 650px;
            margin: 0.8rem auto 0;
            font-weight: 400;
        }

        /* --- HEADER / PROFILE --- */
        .profile-header {
            text-align: center;
            margin-bottom: 2rem;
        }
        .profile-header .avatar-icon {
            font-size: 4.2rem;
            color: #2563eb;
            background: #e2f1ff;
            width: 90px;
            height: 90px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            margin: 0 auto 0.8rem;
            box-shadow: 0 8px 20px rgba(37, 99, 235, 0.1);
        }
        .divider {
            width: 70px;
            height: 4px;
            background: linear-gradient(90deg, #2563eb, #7c8cff);
            border-radius: 4px;
            margin: 1.2rem auto 1rem;
        }

        /* --- ABOUT --- */
        .about-text {
            background: #f1f5f9;
            padding: 1.5rem 2rem;
            border-radius: 1.5rem;
            border-left: 6px solid #2563eb;
            font-size: 1.2rem;
            color: #1e293b;
            margin: 1rem 0 0.2rem;
        }

        /* --- SKILLS GRID --- */
        .skills-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem 1.8rem;
            align-items: center;
            justify-content: center;
            margin: 0.8rem 0 1rem;
        }
        .skills-grid img {
            height: 48px;
            width: auto;
            transition: transform 0.2s ease;
            filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.02));
        }
        .skills-grid img:hover {
            transform: scale(1.08);
        }
        .skill-label {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem 1.2rem;
            justify-content: center;
            font-weight: 500;
            color: #1e293b;
            font-size: 0.95rem;
            margin-top: 0.2rem;
        }
        .skill-label span {
            background: #f1f5f9;
            padding: 0.2rem 1.5rem;
            border-radius: 30px;
            font-size: 0.85rem;
            font-weight: 500;
            color: #1e293b;
        }
        .tech-category {
            background: #fafcff;
            border-radius: 1.4rem;
            padding: 1.2rem 1.5rem 0.8rem;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.02);
            border: 1px solid #eef2f6;
            margin: 1.2rem 0 0.2rem;
        }
        .tech-category p {
            font-weight: 600;
            color: #0b1120;
            margin-bottom: 0.6rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        .tech-category p i {
            color: #2563eb;
            width: 1.4rem;
        }

        /* --- PROJECT CARDS --- */
        .project-card {
            background: #fafcff;
            border: 1px solid #e9edf2;
            border-radius: 1.6rem;
            padding: 1.8rem 2rem;
            margin: 1.6rem 0;
            transition: box-shadow 0.25s ease, transform 0.15s ease;
        }
        .project-card:hover {
            box-shadow: 0 12px 30px -10px rgba(0, 0, 0, 0.06);
            transform: translateY(-4px);
            border-color: #2563eb;
        }
        .project-card h3 {
            font-size: 1.5rem;
            margin-top: 0;
            display: flex;
            align-items: center;
            gap: 0.6rem;
        }
        .project-card h3 i {
            color: #2563eb;
            font-size: 1.7rem;
        }
        .project-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem 0.8rem;
            margin: 0.6rem 0 0.8rem;
        }
        .project-stack span {
            background: #eef2ff;
            padding: 0.15rem 0.9rem;
            border-radius: 40px;
            font-size: 0.75rem;
            font-weight: 600;
            color: #1e4f8a;
            letter-spacing: 0.3px;
        }
        .project-features {
            list-style: none;
            margin-top: 0.6rem;
            display: flex;
            flex-wrap: wrap;
            gap: 0.3rem 1.2rem;
        }
        .project-features li {
            font-size: 0.95rem;
            display: flex;
            align-items: center;
            gap: 0.4rem;
            color: #1e293b;
        }
        .project-features li i {
            color: #2563eb;
            font-size: 0.8rem;
            opacity: 0.8;
        }

        /* --- CONTACT --- */
        .contact-links {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem 1.8rem;
            justify-content: center;
            margin: 2rem 0 1rem;
        }
        .contact-links a {
            display: inline-flex;
            align-items: center;
            gap: 0.6rem;
            background: #f1f5f9;
            padding: 0.6rem 1.6rem;
            border-radius: 60px;
            font-weight: 600;
            text-decoration: none;
            color: #0b1120;
            font-size: 0.95rem;
            transition: background 0.2s, transform 0.1s;
            border: 1px solid transparent;
        }
        .contact-links a i {
            font-size: 1.2rem;
        }
        .contact-links a:hover {
            background: #e2e8f0;
            transform: scale(1.02);
            border-color: #cbd5e1;
        }
        .contact-links a.email i {
            color: #dc2626;
        }
        .contact-links a.whatsapp i {
            color: #22c55e;
        }
        .contact-links a.linkedin i {
            color: #0a66c2;
        }

        /* --- FOOTER --- */
        .footer-note {
            text-align: center;
            margin-top: 2.8rem;
            font-size: 0.95rem;
            color: #475569;
            border-top: 2px solid #eef2f6;
            padding-top: 1.8rem;
            letter-spacing: 0.2px;
        }
        .footer-note i {
            color: #2563eb;
            margin: 0 0.2rem;
        }

        /* --- RESPONSIVE --- */
        @media (max-width: 480px) {
            h1 {
                font-size: 2rem;
            }
            .project-card {
                padding: 1.2rem;
            }
            .contact-links a {
                padding: 0.5rem 1.2rem;
                font-size: 0.85rem;
            }
        }
    </style>
</head>
<body>

    <div class="container">

        <!-- ========== HEADER ========== -->
        <div class="profile-header">
            <div class="avatar-icon">
                <i class="fas fa-user-astronaut"></i>
            </div>
            <h1>Abed Mouhamed Yassin</h1>
            <div class="badge-role">
                <i class="fas fa-code" style="margin-right: 6px;"></i> Full Stack Developer
            </div>
            <p class="tagline">
                <i class="fas fa-rocket" style="color: #2563eb; margin-right: 6px;"></i>
                Designing scalable web applications · Reliable backend · Modern interfaces
            </p>
            <div class="divider"></div>
        </div>

        <!-- ========== ABOUT ========== -->
        <section>
            <h2><i class="fas fa-user-circle"></i> About Me</h2>
            <div class="about-text">
                <p style="margin-bottom: 0.3rem;">
                    <i class="fas fa-quote-left" style="color: #2563eb; opacity: 0.5; margin-right: 6px;"></i>
                    I am a Full Stack Developer passionate about building robust and scalable web applications.
                    My focus is combining solid backend architecture with modern frontend technologies to deliver efficient
                    and maintainable software solutions.
                </p>
                <p style="margin-top: 0.6rem;">
                    I enjoy solving complex technical problems, designing structured systems, and continuously learning
                    new technologies to improve my engineering skills.
                </p>
            </div>
        </section>

        <!-- ========== CORE SKILLS ========== -->
        <section>
            <h2><i class="fas fa-cogs"></i> Core Technical Skills</h2>

            <!-- Frontend -->
            <div class="tech-category">
                <p><i class="fas fa-paint-brush"></i> Frontend Development</p>
                <div class="skills-grid">
                    <img src="https://skillicons.dev/icons?i=html,css,js,react,bootstrap" alt="Frontend stack" />
                </div>
                <div class="skill-label">
                    <span>HTML5</span> <span>CSS3</span> <span>JavaScript</span>
                    <span>React</span> <span>Bootstrap</span>
                </div>
            </div>

            <!-- Backend -->
            <div class="tech-category">
                <p><i class="fas fa-server"></i> Backend Development</p>
                <div class="skills-grid">
                    <img src="https://skillicons.dev/icons?i=php,laravel,symfony" alt="Backend stack" />
                </div>
                <div class="skill-label">
                    <span>PHP</span> <span>Laravel</span> <span>Symfony</span>
                </div>
            </div>

            <!-- Databases -->
            <div class="tech-category">
                <p><i class="fas fa-database"></i> Database Systems</p>
                <div class="skills-grid">
                    <img src="https://skillicons.dev/icons?i=mysql,postgresql,mongodb,oracle" alt="Databases" />
                </div>
                <div class="skill-label">
                    <span>MySQL</span> <span>PostgreSQL</span>
                    <span>Oracle</span> <span>MongoDB</span>
                </div>
            </div>

            <!-- Tools -->
            <div class="tech-category">
                <p><i class="fas fa-tools"></i> Development Tools &amp; Environment</p>
                <div class="skills-grid">
                    <img src="https://skillicons.dev/icons?i=git,docker,vscode,postman" alt="Tools" />
                </div>
                <div class="skill-label">
                    <span>Git</span> <span>Docker</span>
                    <span>VS Code</span> <span>Postman</span>
                    <span>WAMP</span> <span>StarUML</span>
                </div>
            </div>
        </section>

        <!-- ========== FEATURED PROJECTS ========== -->
        <section>
            <h2><i class="fas fa-folder-open"></i> Featured Projects</h2>

            <!-- Project 1 -->
            <div class="project-card">
                <h3><i class="fas fa-atom"></i> React Web Application – API Integration</h3>
                <p style="color: #334155; margin-top: 0.2rem;">
                    Modern web application using <strong>React</strong> that consumes external APIs and integrates
                    cloud-based services for a dynamic, scalable user experience.
                </p>
                <div class="project-stack">
                    <span>React</span> <span>JavaScript</span> <span>REST API</span>
                </div>
                <ul class="project-features">
                    <li><i class="fas fa-check-circle"></i> API data consumption</li>
                    <li><i class="fas fa-check-circle"></i> Dynamic React components</li>
                    <li><i class="fas fa-check-circle"></i> Modern responsive UI</li>
                    <li><i class="fas fa-check-circle"></i> Scalable architecture</li>
                </ul>
            </div>

            <!-- Project 2 -->
            <div class="project-card">
                <h3><i class="fas fa-store"></i> E‑commerce Platform</h3>
                <p style="color: #334155; margin-top: 0.2rem;">
                    Full‑stack web application with structured backend logic and responsive frontend interfaces.
                </p>
                <div class="project-stack">
                    <span>HTML</span> <span>CSS</span> <span>JavaScript</span>
                    <span>Bootstrap</span> <span>PHP</span> <span>MySQL</span>
                </div>
                <ul class="project-features">
                    <li><i class="fas fa-check-circle"></i> CRUD operations</li>
                    <li><i class="fas fa-check-circle"></i> Responsive design</li>
                    <li><i class="fas fa-check-circle"></i> Server‑side processing</li>
                    <li><i class="fas fa-check-circle"></i> MySQL management</li>
                </ul>
            </div>

            <!-- Project 3 -->
            <div class="project-card">
                <h3><i class="fas fa-hotel"></i> Hotel Management System</h3>
                <p style="color: #334155; margin-top: 0.2rem;">
                    Web‑based system handling reservations, customer management, and administrative tasks.
                </p>
                <div class="project-stack">
                    <span>HTML</span> <span>CSS</span> <span>JavaScript</span>
                    <span>Bootstrap</span> <span>PHP</span> <span>MySQL</span>
                </div>
                <ul class="project-features">
                    <li><i class="fas fa-check-circle"></i> Reservation management</li>
                    <li><i class="fas fa-check-circle"></i> Customer data handling</li>
                    <li><i class="fas fa-check-circle"></i> Admin dashboard</li>
                    <li><i class="fas fa-check-circle"></i> Secure backend logic</li>
                </ul>
            </div>
        </section>

        <!-- ========== CONTACT ========== -->
        <section>
            <h2><i class="fas fa-paper-plane"></i> Contact</h2>
            <div class="contact-links">
                <a href="mailto:mouhamedyassin6@gmail.com" class="email">
                    <i class="fas fa-envelope"></i> Email
                </a>
                <a href="https://wa.me/21622314826" class="whatsapp">
                    <i class="fab fa-whatsapp"></i> WhatsApp
                </a>
                <a href="https://www.linkedin.com/in/abed-mouhamed-yassin-81ab54212/" class="linkedin">
                    <i class="fab fa-linkedin-in"></i> LinkedIn
                </a>
            </div>
        </section>

        <!-- ========== FOOTER ========== -->
        <div class="footer-note">
            <i class="fas fa-cube" style="margin-right: 6px;"></i>
            Building reliable software solutions through clean architecture, modern technologies, and continuous learning.
        </div>

    </div>
    <!-- /container -->

</body>
</html>
