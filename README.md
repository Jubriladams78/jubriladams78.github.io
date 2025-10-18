<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JUBRIL J ADAMS - Cloud Engineer Portfolio</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
    <style>
        /* Font Awesome Icons as Unicode */
        .fa-github:before { content: "\f09b"; }
        .fa-linkedin:before { content: "\f0e1"; }
        .fa-phone:before { content: "\f095"; }
        .fa-envelope:before { content: "\f0e0"; }
        .fa-aws:before { content: "\f375"; }
        .fa-microsoft:before { content: "\f3ca"; }
        .fa-docker:before { content: "\f395"; }
        .fa-cloud:before { content: "\f0c2"; }
        .fa-server:before { content: "\f233"; }
        .fa-rocket:before { content: "\f135"; }
        .fa-code-branch:before { content: "\f126"; }
        .fa-code:before { content: "\f121"; }
        .fa-dharmachakra:before { content: "\f655"; }
        .fa-arrow-right:before { content: "\f061"; }
        .fa-shield-alt:before { content: "\f3ed"; }
        .fa-database:before { content: "\f1c0"; }
        .fa-linux:before { content: "\f17c"; }
        .fa-network-wired:before { content: "\f6ff"; }
        .fa-shopping-cart:before { content: "\f07a"; }
        .fa-cloud-upload-alt:before { content: "\f382"; }
        .fa-dollar-sign:before { content: "\f155"; }
        .fa-robot:before { content: "\f544"; }
        .fa-certificate:before { content: "\f0a3"; }
        .fa-download:before { content: "\f019"; }
        .fa-times:before { content: "\f00d"; }
        .fa-chevron-down:before { content: "\f078"; }
        
        .fab, .fas, .fa {
            font-family: "Font Awesome 6 Free", "Font Awesome 6 Brands";
            font-weight: 900;
            font-style: normal;
            display: inline-block;
        }
        
        .fab {
            font-family: "Font Awesome 6 Brands";
        }
        
        @font-face {
            font-family: "Font Awesome 6 Free";
            font-style: normal;
            font-weight: 900;
            font-display: block;
            src: url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/webfonts/fa-solid-900.woff2) format("woff2");
        }
        
        @font-face {
            font-family: "Font Awesome 6 Brands";
            font-style: normal;
            font-weight: 400;
            font-display: block;
            src: url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/webfonts/fa-brands-400.woff2) format("woff2");
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --bg-dark: #0a0a0a;
            --bg-card: #111111;
            --accent-cyan: #00fff7;
            --accent-purple: #a855f7;
            --accent-pink: #ec4899;
            --text-primary: #ffffff;
            --text-secondary: #a1a1aa;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', sans-serif;
            background: var(--bg-dark);
            color: var(--text-primary);
            line-height: 1.6;
            min-height: 100vh;
            overflow-x: hidden;
        }

        /* Animated background */
        .bg-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            opacity: 0.4;
        }

        .bg-gradient {
            position: absolute;
            width: 600px;
            height: 600px;
            border-radius: 50%;
            filter: blur(120px);
            animation: float 20s infinite ease-in-out;
        }

        .gradient-1 {
            background: var(--accent-cyan);
            top: -200px;
            left: -200px;
            animation-delay: 0s;
        }

        .gradient-2 {
            background: var(--accent-purple);
            bottom: -200px;
            right: -200px;
            animation-delay: 7s;
        }

        .gradient-3 {
            background: var(--accent-pink);
            top: 50%;
            left: 50%;
            animation-delay: 14s;
        }

        @keyframes float {
            0%, 100% { transform: translate(0, 0) scale(1); }
            33% { transform: translate(100px, -100px) scale(1.1); }
            66% { transform: translate(-100px, 100px) scale(0.9); }
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 40px;
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            backdrop-filter: blur(20px);
            background: rgba(10, 10, 10, 0.7);
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            z-index: 1000;
            padding: 20px 0;
        }

        .nav-content {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            background: linear-gradient(135deg, var(--accent-cyan), var(--accent-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .nav-links {
            display: flex;
            gap: 40px;
            list-style: none;
        }

        .nav-links a {
            color: var(--text-secondary);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: linear-gradient(90deg, var(--accent-cyan), var(--accent-purple));
            transition: width 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--text-primary);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .nav-actions {
            display: flex;
            gap: 20px;
            align-items: center;
        }

        .download-btn {
            padding: 10px 20px;
            background: var(--accent-cyan);
            color: var(--bg-dark);
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.9rem;
        }

        .download-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(0, 255, 247, 0.3);
        }

        /* Hero Section */
        header {
            padding: 200px 0 150px;
            text-align: center;
            position: relative;
        }

        .hero-badge {
            display: inline-block;
            padding: 10px 25px;
            border: 1px solid rgba(0, 255, 247, 0.3);
            border-radius: 50px;
            color: var(--accent-cyan);
            font-size: 0.9rem;
            margin-bottom: 30px;
            animation: slideDown 1s ease;
            backdrop-filter: blur(10px);
            background: rgba(0, 255, 247, 0.05);
        }

        .hero-title {
            font-size: 5rem;
            font-weight: 900;
            margin-bottom: 20px;
            background: linear-gradient(135deg, var(--accent-cyan), var(--accent-purple), var(--accent-pink));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: slideUp 1s ease 0.2s both;
            letter-spacing: -3px;
        }

        .hero-subtitle {
            font-size: 1.5rem;
            color: var(--text-secondary);
            margin-bottom: 40px;
            animation: slideUp 1s ease 0.4s both;
            font-weight: 300;
        }

        .hero-cta {
            display: flex;
            gap: 20px;
            justify-content: center;
            animation: slideUp 1s ease 0.6s both;
        }

        .btn {
            padding: 18px 40px;
            border-radius: 50px;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            font-size: 1rem;
            border: none;
            cursor: pointer;
            display: inline-flex;
            align-items: center;
            gap: 10px;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--accent-cyan), var(--accent-purple));
            color: white;
            box-shadow: 0 20px 40px rgba(0, 255, 247, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 25px 50px rgba(0, 255, 247, 0.5);
        }

        .btn-secondary {
            border: 2px solid rgba(255, 255, 255, 0.2);
            color: var(--text-primary);
            backdrop-filter: blur(10px);
        }

        .btn-secondary:hover {
            border-color: var(--accent-cyan);
            background: rgba(0, 255, 247, 0.1);
            transform: translateY(-3px);
        }

        .social-links {
            display: flex;
            gap: 25px;
            justify-content: center;
            margin-top: 50px;
            animation: slideUp 1s ease 0.8s both;
        }

        .social-links a {
            width: 50px;
            height: 50px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--text-secondary);
            font-size: 1.2rem;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .social-links a:hover {
            border-color: var(--accent-cyan);
            color: var(--accent-cyan);
            transform: translateY(-5px) rotate(5deg);
            box-shadow: 0 10px 30px rgba(0, 255, 247, 0.3);
        }

        /* Section Styles */
        .section {
            margin-bottom: 150px;
            opacity: 0;
            transform: translateY(50px);
            animation: fadeInUp 1s ease forwards;
        }

        .section:nth-child(2) { animation-delay: 0.2s; }
        .section:nth-child(3) { animation-delay: 0.4s; }
        .section:nth-child(4) { animation-delay: 0.6s; }

        .section-header {
            text-align: center;
            margin-bottom: 80px;
        }

        .section-label {
            display: inline-block;
            padding: 8px 20px;
            border: 1px solid rgba(0, 255, 247, 0.3);
            border-radius: 50px;
            color: var(--accent-cyan);
            font-size: 0.85rem;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: 600;
        }

        .section-title {
            font-size: 3.5rem;
            font-weight: 900;
            margin-bottom: 20px;
            letter-spacing: -2px;
        }

        .section-description {
            color: var(--text-secondary);
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto;
        }

        /* About Section */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .about-text p {
            font-size: 1.2rem;
            color: var(--text-secondary);
            line-height: 2;
            margin-bottom: 30px;
        }

        .about-stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            margin-top: 40px;
        }

        .stat-card {
            text-align: center;
            padding: 30px;
            background: var(--bg-card);
            border: 1px solid rgba(255, 255, 255, 0.05);
            border-radius: 20px;
            transition: all 0.3s ease;
        }

        .stat-card:hover {
            border-color: var(--accent-cyan);
            transform: translateY(-5px);
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 900;
            background: linear-gradient(135deg, var(--accent-cyan), var(--accent-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .stat-label {
            color: var(--text-secondary);
            font-size: 0.9rem;
            margin-top: 5px;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 25px;
        }

        .skill-card {
            background: var(--bg-card);
            padding: 40px 30px;
            border-radius: 25px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .skill-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(0, 255, 247, 0.1), transparent);
            transition: left 0.5s ease;
        }

        .skill-card:hover::before {
            left: 100%;
        }

        .skill-card:hover {
            transform: translateY(-10px) scale(1.02);
            border-color: var(--accent-cyan);
            box-shadow: 0 20px 60px rgba(0, 255, 247, 0.2);
        }

        .skill-card i {
            font-size: 3.5rem;
            margin-bottom: 20px;
            background: linear-gradient(135deg, var(--accent-cyan), var(--accent-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: inline-block;
            transition: transform 0.3s ease;
        }

        .skill-card:hover i {
            transform: scale(1.1) rotateY(360deg);
        }

        .skill-card h3 {
            font-size: 1.3rem;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .skill-card p {
            color: var(--text-secondary);
            font-size: 0.9rem;
        }

        /* Projects Grid */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 35px;
        }

        .project-card {
            background: var(--bg-card);
            border-radius: 30px;
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
        }

        .project-card:hover {
            transform: translateY(-15px);
            border-color: var(--accent-cyan);
            box-shadow: 0 30px 80px rgba(0, 255, 247, 0.3);
        }

        .project-image {
            width: 100%;
            height: 250px;
            background: linear-gradient(135deg, rgba(0, 255, 247, 0.2), rgba(168, 85, 247, 0.2));
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 5rem;
            position: relative;
            overflow: hidden;
        }

        .project-image i {
            background: linear-gradient(135deg, var(--accent-cyan), var(--accent-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            transition: transform 0.4s ease;
        }

        .project-card:hover .project-image i {
            transform: scale(1.2) rotate(5deg);
        }

        .project-content {
            padding: 35px;
        }

        .project-content h3 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            font-weight: 700;
        }

        .project-content p {
            color: var(--text-secondary);
            margin-bottom: 25px;
            line-height: 1.8;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 25px;
        }

        .tag {
            background: rgba(0, 255, 247, 0.1);
            color: var(--accent-cyan);
            padding: 8px 18px;
            border-radius: 50px;
            font-size: 0.85rem;
            border: 1px solid rgba(0, 255, 247, 0.3);
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .tag:hover {
            background: rgba(0, 255, 247, 0.2);
            transform: scale(1.05);
        }

        .project-link {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            color: var(--accent-cyan);
            text-decoration: none;
            font-weight: 700;
            transition: all 0.3s ease;
            cursor: pointer;
            background: none;
            border: none;
        }

        .project-link:hover {
            gap: 15px;
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 2000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(5px);
        }

        .modal.active {
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .modal-content {
            background: var(--bg-card);
            padding: 50px;
            border-radius: 30px;
            max-width: 900px;
            width: 90%;
            max-height: 80vh;
            overflow-y: auto;
            border: 1px solid rgba(0, 255, 247, 0.3);
            position: relative;
        }

        .modal-close {
            position: absolute;
            top: 20px;
            right: 20px;
            background: none;
            border: none;
            color: var(--accent-cyan);
            font-size: 2rem;
            cursor: pointer;
            transition: transform 0.3s ease;
        }

        .modal-close:hover {
            transform: rotate(90deg);
        }

        .modal-title {
            font-size: 2.5rem;
            margin-bottom: 30px;
            background: linear-gradient(135deg, var(--accent-cyan), var(--accent-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .guide-step {
            margin-bottom: 30px;
            padding: 20px;
            background: rgba(0, 255, 247, 0.05);
            border-left: 4px solid var(--accent-cyan);
            border-radius: 10px;
        }

        .guide-step h3 {
            color: var(--accent-cyan);
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 1.3rem;
        }

        .guide-step p {
            color: var(--text-secondary);
            line-height: 1.8;
            margin-bottom: 10px;
        }

        .guide-step ul {
            color: var(--text-secondary);
            margin-left: 20px;
            line-height: 1.8;
        }

        .guide-step li {
            margin-bottom: 8px;
        }

        /* Contact Section */
        .contact-card {
            background: var(--bg-card);
            padding: 80px 60px;
            border-radius: 40px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.05);
            position: relative;
            overflow: hidden;
        }

        .contact-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(0, 255, 247, 0.1) 0%, transparent 70%);
            animation: rotate 20s linear infinite;
        }

        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        .contact-card > * {
            position: relative;
            z-index: 1;
        }

        .contact-card h2 {
            font-size: 3rem;
            margin-bottom: 20px;
            font-weight: 900;
        }

        .contact-card p {
            font-size: 1.3rem;
            color: var(--text-secondary);
            margin-bottom: 40px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 60px 0;
            color: var(--text-secondary);
            border-top: 1px solid rgba(255, 255, 255, 0.05);
            margin-top: 150px;
        }

        /* Animations */
        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Responsive */
        @media (max-width: 1024px) {
            .about-grid {
                grid-template-columns: 1fr;
            }

            .projects-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 768px) {
            .container {
                padding: 0 20px;
            }

            .nav-content {
                padding: 0 20px;
            }

            .nav-links {
                display: none;
            }

            header {
                padding: 150px 0 100px;
            }

            .hero-title {
                font-size: 3rem;
                letter-spacing: -1px;
            }

            .hero-subtitle {
                font-size: 1.2rem;
            }

            .section-title {
                font-size: 2.5rem;
            }

            .about-stats {
                grid-template-columns: 1fr;
            }

            .hero-cta {
                flex-direction: column;
                align-items: stretch;
            }

            .contact-card {
                padding: 50px 30px;
            }

            .modal-content {
                padding: 30px;
                width: 95%;
            }
        }
    </style>
</head>
<body>
    <div class="bg-animation">
        <div class="bg-gradient gradient-1"></div>
        <div class="bg-gradient gradient-2"></div>
        <div class="bg-gradient gradient-3"></div>
    </div>

    <nav>
        <div class="nav-content">
            <div class="logo">JJA</div>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#certifications">Certifications</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="nav-actions">
                <button class="download-btn" onclick="downloadResume()">
                    <i class="fas fa-download"></i> Download Resume
                </button>
            </div>
        </div>
    </nav>

    <div class="container">
        <header>
            <div class="hero-badge">💡 Available for new opportunities</div>
            <h1 class="hero-title">JUBRIL J ADAMS</h1>
            <p class="hero-subtitle">System Administrator | Multi-Cloud Engineer (AWS, Azure, GCP) | DevOps Enthusiast</p>
            <div class="hero-cta">
                <a href="#projects" class="btn btn-primary">View My Work</a>
                <a href="#contact" class="btn btn-secondary">Get In Touch</a>
            </div>
            <div class="social-links">
                <a href="#" aria-label="GitHub"><i class="fab fa-github"></i></a>
                <a href="http://www.linkedin.com/in/jubriladams" target="_blank" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
                <a href="tel:224-474-9556" aria-label="Phone"><i class="fas fa-phone"></i></a>
                <a href="mailto:Jubriladams75@gmail.com" aria-label="Email"><i class="fas fa-envelope"></i></a>
            </div>
        </header>

        <section class="section" id="about">
            <div class="section-header">
                <div class="section-label">About Me</div>
                <h2 class="section-title">Building The Cloud</h2>
                <p class="section-description">Transforming infrastructure through automation, scalability, and cutting-edge cloud technologies</p>
            </div>
            <div class="about-grid">
                <div class="about-text">
                    <p>
                        I'm a Cloud Solutions Architect at Secure&IT with over 4 years of experience designing and deploying scalable, secure, and cost-effective cloud infrastructures. My expertise spans AWS, Azure, GCP, Linux system administration, and infrastructure as code (IaC).
                    </p>
                    <p>
                        I specialize in facilitating large-scale application migrations, optimizing cloud costs, and supporting disaster recovery planning. Through containerization technologies, agile methodologies, and modern DevOps practices, I deliver efficient and reliable cloud solutions that drive organizational success.
                    </p>
                </div>
            </div>
        </section>

        <section class="section" id="skills">
            <div class="section-header">
                <div class="section-label">Expertise</div>
                <h2 class="section-title">Skills & Technologies</h2>
            </div>
            <div class="skills-grid">
                <div class="skill-card">
                    <i class="fab fa-aws"></i>
                    <h3>AWS</h3>
                    <p>EC2, S3, Lambda, ECS, RDS, VPC</p>
                </div>
                <div class="skill-card">
                    <i class="fab fa-microsoft"></i>
                    <h3>Azure & GCP</h3>
                    <p>Multi-Cloud Architecture</p>
                </div>
                <div class="skill-card">
                    <i class="fab fa-linux"></i>
                    <h3>Linux Admin</h3>
                    <p>RHEL, Ubuntu, System Config</p>
                </div>
                <div class="skill-card">
                    <i class="fab fa-docker"></i>
                    <h3>Docker</h3>
                    <p>Containerization & Deployment</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-dharmachakra"></i>
                    <h3>Kubernetes</h3>
                    <p>K8s Orchestration</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-code"></i>
                    <h3>IaC & Scripting</h3>
                    <p>Terraform, Python, Bash</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-code-branch"></i>
                    <h3>CI/CD</h3>
                    <p>Jenkins, GitLab CI, GitHub Actions</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-shield-alt"></i>
                    <h3>Security</h3>
                    <p>Compliance & Best Practices</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-network-wired"></i>
                    <h3>Networking</h3>
                    <p>VPN, Load Balancing, DNS</p>
                </div>
            </div>
        </section>

        <section class="section" id="certifications">
            <div class="section-header">
                <div class="section-label">Certifications</div>
                <h2 class="section-title">Professional Credentials</h2>
                <p class="section-description">Industry-recognized certifications validating my cloud and IT expertise</p>
            </div>
            <div class="skills-grid">
                <div class="skill-card">
                    <i class="fab fa-aws"></i>
                    <h3>AWS Solutions Architect</h3>
                    <p>Associate Level - Amazon Web Services</p>
                </div>
                <div class="skill-card">
                    <i class="fab fa-aws"></i>
                    <h3>AWS Cloud Practitioner</h3>
                    <p>Foundational - Amazon Web Services</p>
                </div>
                <div class="skill-card">
                    <i class="fab fa-linux"></i>
                    <h3>Linux Essentials</h3>
                    <p>Linux Professional Institute (LPI)</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-certificate"></i>
                    <h3>CompTIA A+ CE</h3>
                    <p>Continuing Education - CompTIA</p>
                </div>
            </div>
        </section>

        <section class="section" id="projects">
            <div class="section-header">
                <div class="section-label">Portfolio</div>
                <h2 class="section-title">Featured Projects</h2>
                <p class="section-description">A selection of my recent cloud engineering and DevOps projects</p>
            </div>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-shopping-cart"></i>
                    </div>
                    <div class="project-content">
                        <h3>E-Commerce Cloud Optimization</h3>
                        <p>Led infrastructure enhancement for e-commerce platform, implementing AWS load balancing and reducing latency. Integrated advanced analytics driving 20% sales increase during peak traffic periods.</p>
                        <div class="project-tags">
                            <span class="tag">AWS</span>
                            <span class="tag">Load Balancing</span>
                            <span class="tag">Analytics</span>
                            <span class="tag">Scalability</span>
                        </div>
                        <button class="project-link" onclick="openGuide(1)">
                            View Details <i class="fas fa-arrow-right"></i>
                        </button>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-cloud-upload-alt"></i>
                    </div>
                    <div class="project-content">
                        <h3>Large-Scale Application Migration</h3>
                        <p>Successfully led team to migrate 200+ applications to cloud infrastructure with zero downtime. Implemented comprehensive disaster recovery strategy ensuring 99.9% system uptime.</p>
                        <div class="project-tags">
                            <span class="tag">AWS</span>
                            <span class="tag">Migration</span>
                            <span class="tag">Zero Downtime</span>
                            <span class="tag">DR Planning</span>
                        </div>
                        <button class="project-link" onclick="openGuide(2)">
                            View Details <i class="fas fa-arrow-right"></i>
                        </button>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-server"></i>
                    </div>
                    <div class="project-content">
                        <h3>Web Server Performance Enhancement</h3>
                        <p>Optimized web server performance using NGINX, achieving 30% efficiency increase. Enhanced security protocols reducing vulnerabilities and improving site reliability for dynamic e-commerce platform.</p>
                        <div class="project-tags">
                            <span class="tag">NGINX</span>
                            <span class="tag">Load Balancing</span>
                            <span class="tag">Security</span>
                            <span class="tag">Performance</span>
                        </div>
                        <button class="project-link" onclick="openGuide(3)">
                            View Details <i class="fas fa-arrow-right"></i>
                        </button>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-dollar-sign"></i>
                    </div>
                    <div class="project-content">
                        <h3>Cloud Cost Optimization</h3>
                        <p>Reduced cloud infrastructure costs by 30% through strategic resource allocation and optimization. Implemented automated monitoring and right-sizing recommendations for AWS resources.</p>
                        <div class="project-tags">
                            <span class="tag">Cost Optimization</span>
                            <span class="tag">AWS</span>
                            <span class="tag">Automation</span>
                            <span class="tag">Monitoring</span>
                        </div>
                        <button class="project-link" onclick="openGuide(4)">
                            View Details <i class="fas fa-arrow-right"></i>
                        </button>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-robot"></i>
                    </div>
                    <div class="project-content">
                        <h3>Automation Through Scripting</h3>
                        <p>Developed automated Python and Bash scripts resulting in 50% reduction of manual server maintenance tasks. Streamlined deployment processes and improved operational efficiency.</p>
                        <div class="project-tags">
                            <span class="tag">Python</span>
                            <span class="tag">Bash</span>
                            <span class="tag">Automation</span>
                            <span class="tag">DevOps</span>
                        </div>
                        <button class="project-link" onclick="openGuide(5)">
                            View Details <i class="fas fa-arrow-right"></i>
                        </button>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-image">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <div class="project-content">
                        <h3>Hybrid Cloud Architecture</h3>
                        <p>Defined cloud architecture for hybrid solutions ensuring compliance with cybersecurity regulations. Identified and remediated security risks enhancing overall system reliability.</p>
                        <div class="project-tags">
                            <span class="tag">Hybrid Cloud</span>
                            <span class="tag">Security</span>
                            <span class="tag">Compliance</span>
                            <span class="tag">Multi-Cloud</span>
                        </div>
                        <button class="project-link" onclick="openGuide(6)">
                            View Details <i class="fas fa-arrow-right"></i>
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <section class="section" id="contact">
            <div class="contact-card">
                <h2>Let's Build Something Amazing</h2>
                <p>I'm always interested in hearing about innovative projects and opportunities to create exceptional cloud solutions.</p>
                <a href="mailto:Jubriladams75@gmail.com" class="btn btn-primary">Start a Conversation</a>
            </div>
        </section>

        <footer>
            <p>&copy; 2025 JUBRIL J ADAMS • Cloud Engineer • Built with passion for technology</p>
        </footer>
    </div>

    <!-- Project Guide Modal -->
    <div class="modal" id="guideModal">
        <div class="modal-content">
            <button class="modal-close" onclick="closeGuide()"><i class="fas fa-times"></i></button>
            <h2 class="modal-title" id="guideTitle"></h2>
            <div id="guideContent"></div>
        </div>
    </div>

    <!-- Hidden Resume Section (for PDF generation) -->
    <div id="resumeContent" style="display: none; background: white; color: black; padding: 40px; font-family: Arial, sans-serif;">
        <div style="text-align: center; margin-bottom: 30px; border-bottom: 3px solid #00fff7; padding-bottom: 20px;">
            <h1 style="margin: 0; font-size: 2.5em;">JUBRIL J ADAMS</h1>
            <p style="margin: 5px 0; font-size: 1.1em;">System Administrator | Multi-Cloud Engineer | DevOps Enthusiast</p>
            <p style="margin: 5px 0;">📞 224-474-9556 | 📧 Jubriladams75@gmail.com | 🔗 linkedin.com/in/jubriladams</p>
        </div>

        <div style="margin-bottom: 25px;">
            <h2 style="border-bottom: 2px solid #00fff7; padding-bottom: 10px; color: #00fff7;">PROFESSIONAL SUMMARY</h2>
            <p>Cloud Solutions Architect at Secure&IT with 4+ years of experience designing and deploying scalable, secure, and cost-effective cloud infrastructures. Expertise in AWS, Azure, GCP, Linux system administration, and Infrastructure as Code. Proven track record in large-scale application migrations, cloud cost optimization, and disaster recovery planning.</p>
        </div>

        <div style="margin-bottom: 25px;">
            <h2 style="border-bottom: 2px solid #00fff7; padding-bottom: 10px; color: #00fff7;">CORE COMPETENCIES</h2>
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">
                <div>
                    <strong>Cloud Platforms:</strong> AWS, Azure, GCP<br>
                    <strong>Containerization:</strong> Docker, Kubernetes, ECS<br>
                    <strong>Infrastructure as Code:</strong> Terraform, CloudFormation
                </div>
                <div>
                    <strong>CI/CD Tools:</strong> Jenkins, GitLab CI, GitHub Actions<br>
                    <strong>Programming:</strong> Python, Bash, YAML<br>
                    <strong>Specializations:</strong> Cost Optimization, Security, Load Balancing
                </div>
            </div>
        </div>

        <div style="margin-bottom: 25px;">
            <h2 style="border-bottom: 2px solid #00fff7; padding-bottom: 10px; color: #00fff7;">KEY ACHIEVEMENTS</h2>
            <ul style="line-height: 1.8;">
                <li>Successfully migrated 200+ applications to cloud with zero downtime</li>
                <li>Reduced cloud infrastructure costs by 30% through strategic optimization</li>
                <li>Maintained 99.9% system uptime across all managed infrastructure</li>
                <li>Achieved 30% efficiency increase in web server performance using NGINX</li>
                <li>Reduced manual server maintenance tasks by 50% through automation</li>
                <li>Designed hybrid cloud architecture ensuring compliance with cybersecurity regulations</li>
            </ul>
        </div>

        <div style="margin-bottom: 25px;">
            <h2 style="border-bottom: 2px solid #00fff7; padding-bottom: 10px; color: #00fff7;">TECHNICAL SKILLS</h2>
            <div style="line-height: 2;">
                <strong>Cloud Services:</strong> EC2, S3, Lambda, ECS, RDS, VPC, Azure VMs, App Services, GCP Compute Engine<br>
                <strong>DevOps Tools:</strong> Docker, Kubernetes, Terraform, Ansible, Jenkins<br>
                <strong>Linux/Unix:</strong> RHEL, Ubuntu, CentOS, System Administration, Shell Scripting<br>
                <strong>Networking:</strong> VPN Configuration, Load Balancing, DNS, VPC Management<br>
                <strong>Monitoring:</strong> CloudWatch, Prometheus, Grafana, ELK Stack<br>
                <strong>Security:</strong> IAM, Security Groups, Compliance, Best Practices
            </div>
        </div>

        <div style="margin-bottom: 25px;">
            <h2 style="border-bottom: 2px solid #00fff7; padding-bottom: 10px; color: #00fff7;">PROFESSIONAL EXPERIENCE</h2>
            <div style="margin-bottom: 20px;">
                <h3 style="margin: 0; color: #333;">Cloud Solutions Architect</h3>
                <p style="margin: 5px 0; font-style: italic;">Secure&IT | 4+ Years</p>
                <ul style="line-height: 1.8; margin: 10px 0;">
                    <li>Design and deploy scalable cloud infrastructures across AWS, Azure, and GCP</li>
                    <li>Lead large-scale application migrations with zero downtime strategy</li>
                    <li>Optimize cloud costs through resource allocation and automation</li>
                    <li>Implement disaster recovery and business continuity planning</li>
                    <li>Manage infrastructure security and compliance requirements</li>
                </ul>
            </div>
        </div>

        <div style="margin-bottom: 25px;">
            <h2 style="border-bottom: 2px solid #00fff7; padding-bottom: 10px; color: #00fff7;">CERTIFICATIONS</h2>
            <ul style="line-height: 1.8;">
                <li>AWS Solutions Architect Associate - Amazon Web Services</li>
                <li>AWS Cloud Practitioner - Amazon Web Services</li>
                <li>Linux Essentials - Linux Professional Institute (LPI)</li>
                <li>CompTIA A+ Continuing Education - CompTIA</li>
            </ul>
        </div>

        <div style="margin-bottom: 25px;">
            <h2 style="border-bottom: 2px solid #00fff7; padding-bottom: 10px; color: #00fff7;">PROJECTS & NOTABLE WORK</h2>
            <div style="line-height: 1.8;">
                <strong>E-Commerce Cloud Optimization:</strong> Implemented AWS load balancing, reduced latency, integrated analytics driving 20% sales increase<br><br>
                <strong>Large-Scale Migration:</strong> Led migration of 200+ applications with zero downtime, established 99.9% uptime SLA<br><br>
                <strong>Web Server Optimization:</strong> Implemented NGINX configuration achieving 30% performance improvement<br><br>
                <strong>Hybrid Cloud Architecture:</strong> Designed compliant hybrid solutions with security hardening and risk remediation
            </div>
        </div>
    </div>

    <script>
        const guides = {
            1: {
                title: "E-Commerce Cloud Optimization Guide",
                content: `
                    <div class="guide-step">
                        <h3><i class="fas fa-rocket"></i> Step 1: Infrastructure Assessment</h3>
                        <p>Begin by analyzing the current e-commerce platform infrastructure:</p>
                        <ul>
                            <li>Evaluate existing server configurations and capacity</li>
                            <li>Identify performance bottlenecks and latency issues</li>
                            <li>Document current traffic patterns and peak loads</li>
                            <li>Review security posture and compliance requirements</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-code"></i> Step 2: AWS Load Balancer Setup</h3>
                        <p>Configure Application Load Balancer (ALB) for optimal distribution:</p>
                        <ul>
                            <li>Create target groups for backend EC2 instances</li>
                            <li>Configure listener rules for path-based routing</li>
                            <li>Enable sticky sessions for session persistence</li>
                            <li>Set up health checks with appropriate thresholds</li>
                            <li>Configure SSL/TLS certificates for secure communication</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-database"></i> Step 3: Database Optimization</h3>
                        <p>Optimize database performance and scalability:</p>
                        <ul>
                            <li>Migrate to Amazon RDS with Multi-AZ deployment</li>
                            <li>Implement read replicas for read-heavy operations</li>
                            <li>Configure automated backups and point-in-time recovery</li>
                            <li>Implement caching strategies using ElastiCache</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-chart-line"></i> Step 4: Analytics Integration</h3>
                        <p>Implement analytics to drive business insights:</p>
                        <ul>
                            <li>Set up Amazon Kinesis for real-time data streaming</li>
                            <li>Integrate AWS Analytics services for customer behavior analysis</li>
                            <li>Create CloudWatch dashboards for performance monitoring</li>
                            <li>Configure alerts for critical metrics and thresholds</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-check-circle"></i> Step 5: Testing & Validation</h3>
                        <p>Ensure reliability before production deployment:</p>
                        <ul>
                            <li>Conduct load testing using Apache JMeter or similar tools</li>
                            <li>Verify latency improvements and response times</li>
                            <li>Test failover mechanisms and redundancy</li>
                            <li>Validate analytics data accuracy</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-deploy"></i> Step 6: Deployment & Monitoring</h3>
                        <p>Deploy to production with continuous monitoring:</p>
                        <ul>
                            <li>Execute blue-green deployment strategy</li>
                            <li>Monitor real-time performance metrics</li>
                            <li>Track sales conversion and revenue impact</li>
                            <li>Prepare rollback procedures if needed</li>
                        </ul>
                    </div>
                `
            },
            2: {
                title: "Large-Scale Application Migration Guide",
                content: `
                    <div class="guide-step">
                        <h3><i class="fas fa-list-check"></i> Step 1: Migration Planning & Assessment</h3>
                        <p>Develop comprehensive migration strategy:</p>
                        <ul>
                            <li>Catalog all 200+ applications and dependencies</li>
                            <li>Classify applications (6Rs: Rehost, Replatform, Refactor, Repurchase, Retire, Retain)</li>
                            <li>Create migration wave timeline</li>
                            <li>Establish success criteria and KPIs</li>
                            <li>Document all risks and mitigation strategies</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-network-wired"></i> Step 2: AWS Environment Preparation</h3>
                        <p>Set up cloud infrastructure foundation:</p>
                        <ul>
                            <li>Design VPC architecture with multi-AZ deployment</li>
                            <li>Configure subnets, route tables, and NAT gateways</li>
                            <li>Set up VPN/Direct Connect for on-premises connectivity</li>
                            <li>Configure security groups and NACLs</li>
                            <li>Set up IAM roles and policies</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-server"></i> Step 3: Database Migration Strategy</h3>
                        <p>Execute database migration with minimal downtime:</p>
                        <ul>
                            <li>Use AWS Database Migration Service (DMS)</li>
                            <li>Set up continuous replication for near-zero downtime</li>
                            <li>Perform data validation and reconciliation</li>
                            <li>Configure read replicas for high availability</li>
                            <li>Implement backup and recovery procedures</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-boxes"></i> Step 4: Application Wave Migration</h3>
                        <p>Execute wave-based migration approach:</p>
                        <ul>
                            <li>Wave 1: Non-critical applications (pilot phase)</li>
                            <li>Wave 2: Supporting applications</li>
                            <li>Wave 3: Critical business applications</li>
                            <li>Monitor each wave before proceeding to next</li>
                            <li>Document lessons learned from each wave</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-shield-alt"></i> Step 5: Zero-Downtime Implementation</h3>
                        <p>Ensure business continuity during migration:</p>
                        <ul>
                            <li>Use DNS failover and Route 53 health checks</li>
                            <li>Implement load balancing across on-premises and cloud</li>
                            <li>Set up automated rollback procedures</li>
                            <li>Maintain parallel systems during transition period</li>
                            <li>Monitor performance metrics continuously</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-backup"></i> Step 6: Disaster Recovery Setup</h3>
                        <p>Establish comprehensive DR strategy:</p>
                        <ul>
                            <li>Configure cross-region replication</li>
                            <li>Set up automated backup schedules</li>
                            <li>Create disaster recovery runbooks</li>
                            <li>Conduct DR drills and testing</li>
                            <li>Document RTO and RPO targets</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-chart-line"></i> Step 7: Post-Migration Optimization</h3>
                        <p>Optimize and validate cloud infrastructure:</p>
                        <ul>
                            <li>Monitor performance against SLAs</li>
                            <li>Optimize resource allocation and costs</li>
                            <li>Implement auto-scaling policies</li>
                            <li>Review and optimize security posture</li>
                            <li>Plan decommissioning of on-premises resources</li>
                        </ul>
                    </div>
                `
            },
            3: {
                title: "Web Server Performance Enhancement Guide",
                content: `
                    <div class="guide-step">
                        <h3><i class="fas fa-server"></i> Step 1: Current Performance Baseline</h3>
                        <p>Establish baseline metrics before optimization:</p>
                        <ul>
                            <li>Measure current response times and throughput</li>
                            <li>Identify slow endpoints and bottlenecks</li>
                            <li>Document current CPU, memory, and disk usage</li>
                            <li>Analyze web server logs for patterns</li>
                            <li>Set up monitoring dashboards</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-download"></i> Step 2: NGINX Installation & Configuration</h3>
                        <p>Deploy and configure NGINX web server:</p>
                        <ul>
                            <li>Install NGINX on Linux (RHEL/Ubuntu)</li>
                            <li>Configure worker processes and connections</li>
                            <li>Enable gzip compression for static content</li>
                            <li>Set up SSL/TLS with HTTP/2 support</li>
                            <li>Configure caching headers for browser caching</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-balance-scale"></i> Step 3: Load Balancing Setup</h3>
                        <p>Distribute traffic across multiple backend servers:</p>
                        <ul>
                            <li>Configure upstream backend servers</li>
                            <li>Set up load balancing algorithms (round-robin, least connections)</li>
                            <li>Enable session persistence if required</li>
                            <li>Configure health checks for backend monitoring</li>
                            <li>Implement connection pooling</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-tachometer-alt"></i> Step 4: Performance Tuning</h3>
                        <p>Optimize NGINX configuration:</p>
                        <ul>
                            <li>Increase worker_connections for better concurrency</li>
                            <li>Configure buffer sizes for large uploads/downloads</li>
                            <li>Enable keep-alive connections</li>
                            <li>Optimize TCP settings and timeouts</li>
                            <li>Configure request throttling and rate limiting</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-lock"></i> Step 5: Security Hardening</h3>
                        <p>Strengthen security posture:</p>
                        <ul>
                            <li>Configure WAF (Web Application Firewall) rules</li>
                            <li>Implement rate limiting and DDoS protection</li>
                            <li>Set up security headers (HSTS, X-Frame-Options, CSP)</li>
                            <li>Configure SSL/TLS best practices</li>
                            <li>Enable logging and monitoring for security events</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-caching"></i> Step 6: Caching Strategy</h3>
                        <p>Implement multi-layer caching:</p>
                        <ul>
                            <li>Set up Redis/Memcached for application caching</li>
                            <li>Configure NGINX reverse proxy caching</li>
                            <li>Implement cache invalidation strategies</li>
                            <li>Set up CDN integration for static content</li>
                            <li>Monitor cache hit ratios</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-chart-bar"></i> Step 7: Testing & Validation</h3>
                        <p>Verify performance improvements:</p>
                        <ul>
                            <li>Conduct load testing with Apache JMeter</li>
                            <li>Compare response times to baseline</li>
                            <li>Verify 30% efficiency improvement target</li>
                            <li>Test failover and high availability</li>
                            <li>Validate security configurations</li>
                        </ul>
                    </div>
                `
            },
            4: {
                title: "Cloud Cost Optimization Guide",
                content: `
                    <div class="guide-step">
                        <h3><i class="fas fa-chart-pie"></i> Step 1: Cost Analysis & Assessment</h3>
                        <p>Understand current spending patterns:</p>
                        <ul>
                            <li>Analyze AWS Cost Explorer reports</li>
                            <li>Identify spending by service and account</li>
                            <li>Spot unused or underutilized resources</li>
                            <li>Review cost trends over time</li>
                            <li>Establish baseline and optimization targets</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-recycle"></i> Step 2: Resource Right-Sizing</h3>
                        <p>Match resources to actual needs:</p>
                        <ul>
                            <li>Review EC2 instance utilization metrics</li>
                            <li>Downsize over-provisioned instances</li>
                            <li>Identify idle resources for termination</li>
                            <li>Convert on-demand to reserved instances</li>
                            <li>Use Compute Optimizer recommendations</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-ticket-alt"></i> Step 3: Reserved Instances & Savings Plans</h3>
                        <p>Leverage commitment discounts:</p>
                        <ul>
                            <li>Analyze usage patterns to determine RI eligibility</li>
                            <li>Purchase 1-year or 3-year reserved instances</li>
                            <li>Consider Savings Plans for flexible coverage</li>
                            <li>Blend on-demand with reserved instances</li>
                            <li>Save 30-70% on compute costs</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-storage"></i> Step 4: Storage Optimization</h3>
                        <p>Reduce storage costs:</p>
                        <ul>
                            <li>Implement S3 lifecycle policies for archival</li>
                            <li>Move infrequent data to Glacier/Glacier Deep Archive</li>
                            <li>Delete unused snapshots and volumes</li>
                            <li>Compress and deduplicate data</li>
                            <li>Monitor storage growth trends</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-cloud-download-alt"></i> Step 5: Data Transfer Optimization</h3>
                        <p>Minimize data transfer costs:</p>
                        <ul>
                            <li>Use VPC endpoints to avoid NAT gateway charges</li>
                            <li>Configure CloudFront for content distribution</li>
                            <li>Optimize inter-AZ data transfer</li>
                            <li>Implement efficient caching strategies</li>
                            <li>Monitor data transfer metrics</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-robot"></i> Step 6: Automation & Scheduling</h3>
                        <p>Implement automated cost controls:</p>
                        <ul>
                            <li>Create Lambda functions for resource scheduling</li>
                            <li>Auto-shutdown non-production environments after hours</li>
                            <li>Implement auto-scaling policies</li>
                            <li>Use Systems Manager for patch management</li>
                            <li>Configure CloudWatch alerts for budget thresholds</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-monitor"></i> Step 7: Monitoring & Continuous Optimization</h3>
                        <p>Maintain ongoing cost efficiency:</p>
                        <ul>
                            <li>Set up Cost Anomaly Detection</li>
                            <li>Create monthly cost reports</li>
                            <li>Schedule regular cost reviews</li>
                            <li>Track savings against 30% target</li>
                            <li>Identify emerging optimization opportunities</li>
                        </ul>
                    </div>
                `
            },
            5: {
                title: "Automation Through Scripting Guide",
                content: `
                    <div class="guide-step">
                        <h3><i class="fas fa-file-code"></i> Step 1: Identify Automation Opportunities</h3>
                        <p>Determine which tasks can be automated:</p>
                        <ul>
                            <li>Audit manual server maintenance tasks</li>
                            <li>Document repetitive processes and workflows</li>
                            <li>Identify time-consuming administrative tasks</li>
                            <li>Prioritize by frequency and time impact</li>
                            <li>Establish ROI for automation efforts</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-python"></i> Step 2: Python Script Development</h3>
                        <p>Create Python scripts for complex automation:</p>
                        <ul>
                            <li>Set up Python development environment</li>
                            <li>Develop scripts for AWS API interactions</li>
                            <li>Create system monitoring and alerting scripts</li>
                            <li>Build automated backup and recovery scripts</li>
                            <li>Implement error handling and logging</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-terminal"></i> Step 3: Bash Script Creation</h3>
                        <p>Develop bash scripts for shell-level automation:</p>
                        <ul>
                            <li>Create startup/shutdown automation scripts</li>
                            <li>Develop server configuration scripts</li>
                            <li>Build log rotation and cleanup scripts</li>
                            <li>Create deployment and update scripts</li>
                            <li>Implement performance monitoring scripts</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-tasks"></i> Step 4: Cron Job Scheduling</h3>
                        <p>Schedule automated task execution:</p>
                        <ul>
                            <li>Configure cron jobs for regular execution</li>
                            <li>Set up proper logging for cron tasks</li>
                            <li>Implement email notifications for failures</li>
                            <li>Create backup and archival schedules</li>
                            <li>Monitor cron execution and performance</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-ship"></i> Step 5: CI/CD Pipeline Integration</h3>
                        <p>Integrate automation into deployment pipeline:</p>
                        <ul>
                            <li>Set up Jenkins or GitHub Actions workflows</li>
                            <li>Create automated build and test pipelines</li>
                            <li>Implement automated deployment scripts</li>
                            <li>Configure automated rollback procedures</li>
                            <li>Enable continuous monitoring and notifications</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-code-review"></i> Step 6: Code Quality & Testing</h3>
                        <p>Ensure script reliability:</p>
                        <ul>
                            <li>Implement unit testing for Python scripts</li>
                            <li>Use ShellCheck for Bash script validation</li>
                            <li>Create test automation frameworks</li>
                            <li>Document script functionality and usage</li>
                            <li>Perform peer code reviews</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-chart-line"></i> Step 7: Measurement & Optimization</h3>
                        <p>Track automation impact:</p>
                        <ul>
                            <li>Measure time savings from automation</li>
                            <li>Track manual task reduction (50% target)</li>
                            <li>Monitor error rates and incidents</li>
                            <li>Calculate cost savings</li>
                            <li>Plan additional automation opportunities</li>
                        </ul>
                    </div>
                `
            },
            6: {
                title: "Hybrid Cloud Architecture Guide",
                content: `
                    <div class="guide-step">
                        <h3><i class="fas fa-building"></i> Step 1: Architecture Planning</h3>
                        <p>Design hybrid cloud infrastructure:</p>
                        <ul>
                            <li>Define workload placement strategy</li>
                            <li>Identify applications for on-premises vs cloud</li>
                            <li>Design data residency and compliance requirements</li>
                            <li>Plan network connectivity architecture</li>
                            <li>Document service integration points</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-network-wired"></i> Step 2: Connectivity Setup</h3>
                        <p>Establish secure connection between environments:</p>
                        <ul>
                            <li>Implement AWS Direct Connect or VPN</li>
                            <li>Configure site-to-site VPN with redundancy</li>
                            <li>Set up BGP routing for failover</li>
                            <li>Implement QoS for traffic prioritization</li>
                            <li>Monitor network latency and throughput</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-shield-alt"></i> Step 3: Security & Compliance</h3>
                        <p>Ensure compliance with security requirements:</p>
                        <ul>
                            <li>Implement encryption for data in transit</li>
                            <li>Configure encryption for data at rest</li>
                            <li>Set up identity federation with AD/LDAP</li>
                            <li>Implement security monitoring and logging</li>
                            <li>Conduct security compliance audit</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-key"></i> Step 4: Identity & Access Management</h3>
                        <p>Manage identities across hybrid environment:</p>
                        <ul>
                            <li>Configure AWS IAM with federated identities</li>
                            <li>Set up single sign-on (SSO) integration</li>
                            <li>Implement role-based access control (RBAC)</li>
                            <li>Configure multi-factor authentication (MFA)</li>
                            <li>Monitor access and audit logs</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-database"></i> Step 5: Data Management</h3>
                        <p>Synchronize data across environments:</p>
                        <ul>
                            <li>Implement data replication strategies</li>
                            <li>Configure backup and recovery procedures</li>
                            <li>Set up data synchronization services</li>
                            <li>Implement data residency policies</li>
                            <li>Monitor data consistency and integrity</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-exclamation-triangle"></i> Step 6: Risk Identification & Remediation</h3>
                        <p>Address security vulnerabilities:</p>
                        <ul>
                            <li>Conduct security vulnerability assessment</li>
                            <li>Identify compliance gaps</li>
                            <li>Develop remediation plans</li>
                            <li>Implement security patches and updates</li>
                            <li>Configure security groups and NACLs</li>
                        </ul>
                    </div>

                    <div class="guide-step">
                        <h3><i class="fas fa-check-double"></i> Step 7: Validation & Testing</h3>
                        <p>Verify architecture reliability:</p>
                        <ul>
                            <li>Test failover scenarios</li>
                            <li>Validate compliance requirements</li>
                            <li>Conduct security penetration testing</li>
                            <li>Verify data consistency</li>
                            <li>Document lessons learned and best practices</li>
                        </ul>
                    </div>
                `
            }
        };

        function openGuide(projectId) {
            const guide = guides[projectId];
            if (guide) {
                document.getElementById('guideTitle').textContent = guide.title;
                document.getElementById('guideContent').innerHTML = guide.content;
                document.getElementById('guideModal').classList.add('active');
                document.body.style.overflow = 'hidden';
            }
        }

        function closeGuide() {
            document.getElementById('guideModal').classList.remove('active');
            document.body.style.overflow = 'auto';
        }

        function downloadResume() {
            const element = document.getElementById('resumeContent');
            const opt = {
                margin: 10,
                filename: 'JUBRIL_J_ADAMS_Resume.pdf',
                image: { type: 'jpeg', quality: 0.98 },
                html2canvas: { scale: 2 },
                jsPDF: { unit: 'mm', format: 'a4', orientation: 'portrait' }
            };
            html2pdf().set(opt).from(element).save();
        }

        // Close modal when clicking outside
        window.onclick = function(event) {
            const modal = document.getElementById('guideModal');
            if (event.target == modal) {
                closeGuide();
            }
        }

        // Smooth scroll for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });
    </script>
</body>
</html>    <div class="about-stats">
                    <div class="stat-card">
                        <div class="stat-number">4+</div>
                        <div class="stat-label">Years Experience</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">200+</div>
                        <div class="stat-label">Apps Migrated</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">99.9%</div>
                        <div class="stat-label">System Uptime</div>
                    </div>
                </div>
