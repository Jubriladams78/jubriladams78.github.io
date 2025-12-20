
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jubril Adams - Cloud Support Engineer</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/feather-icons/4.29.0/feather.min.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 50%, #0f172a 100%);
            color: #ffffff;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 24px;
        }

        header {
            background: rgba(15, 23, 42, 0.5);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(59, 130, 246, 0.2);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 16px 0;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            background: linear-gradient(to right, #60a5fa, #22d3ee);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .nav-links {
            display: flex;
            gap: 24px;
            list-style: none;
        }

        .nav-links a {
            color: #d1d5db;
            text-decoration: none;
            text-transform: capitalize;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #22d3ee;
        }

        .hero {
            text-align: center;
            padding: 80px 0;
        }

        .hero-icon {
            width: 128px;
            height: 128px;
            margin: 0 auto 24px;
            background: linear-gradient(135deg, #3b82f6, #22d3ee);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 16px;
        }

        .hero h2 {
            font-size: 28px;
            color: #22d3ee;
            margin-bottom: 24px;
        }

        .hero p {
            font-size: 18px;
            color: #d1d5db;
            max-width: 700px;
            margin: 0 auto 16px;
        }

        .hero .location {
            font-size: 16px;
            color: #9ca3af;
        }

        .btn-group {
            display: flex;
            gap: 16px;
            justify-content: center;
            margin-top: 32px;
        }

        .btn {
            padding: 12px 32px;
            border-radius: 8px;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s;
            cursor: pointer;
            border: none;
            font-size: 16px;
        }

        .btn-primary {
            background: #22d3ee;
            color: #0f172a;
        }

        .btn-primary:hover {
            background: #06b6d4;
        }

        .btn-secondary {
            background: transparent;
            color: #22d3ee;
            border: 2px solid #22d3ee;
        }

        .btn-secondary:hover {
            background: rgba(34, 211, 238, 0.1);
        }

        section {
            padding: 64px 0;
        }

        .section-bg {
            background: rgba(30, 41, 59, 0.3);
        }

        .section-title {
            font-size: 32px;
            text-align: center;
            margin-bottom: 48px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
        }

        .section-title i {
            color: #22d3ee;
        }

        .experience-item {
            background: rgba(30, 41, 59, 0.5);
            border: 1px solid rgba(59, 130, 246, 0.2);
            border-radius: 8px;
            padding: 24px;
            margin-bottom: 32px;
        }

        .experience-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 16px;
            flex-wrap: wrap;
            gap: 16px;
        }

        .experience-title h3 {
            font-size: 24px;
            color: #22d3ee;
            margin-bottom: 8px;
        }

        .experience-title h4 {
            font-size: 20px;
            color: #d1d5db;
        }

        .experience-date {
            text-align: right;
            color: #9ca3af;
        }

        .experience-description {
            color: #9ca3af;
            font-style: italic;
            margin-bottom: 16px;
        }

        .experience-item ul {
            list-style: none;
        }

        .experience-item li {
            color: #d1d5db;
            margin-bottom: 8px;
            display: flex;
            gap: 8px;
        }

        .experience-item li::before {
            content: "▸";
            color: #22d3ee;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 24px;
        }

        .project-card {
            background: rgba(30, 41, 59, 0.5);
            border: 1px solid rgba(59, 130, 246, 0.2);
            border-radius: 8px;
            padding: 24px;
            transition: all 0.3s;
        }

        .project-card:hover {
            border-color: rgba(34, 211, 238, 0.5);
            transform: scale(1.05);
        }

        .project-header {
            display: flex;
            gap: 16px;
            margin-bottom: 16px;
            align-items: flex-start;
        }

        .project-icon {
            background: rgba(34, 211, 238, 0.2);
            padding: 12px;
            border-radius: 8px;
            flex-shrink: 0;
        }

        .project-icon i {
            color: #22d3ee;
        }

        .project-card h4 {
            font-size: 18px;
            margin-bottom: 8px;
        }

        .project-card p {
            color: #d1d5db;
            margin-bottom: 16px;
        }

        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .tech-tag {
            background: rgba(59, 130, 246, 0.2);
            color: #22d3ee;
            padding: 4px 12px;
            border-radius: 16px;
            font-size: 14px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 24px;
        }

        .skill-category {
            background: rgba(30, 41, 59, 0.5);
            border: 1px solid rgba(59, 130, 246, 0.2);
            border-radius: 8px;
            padding: 24px;
        }

        .skill-category h4 {
            font-size: 20px;
            color: #22d3ee;
            margin-bottom: 16px;
        }

        .skill-category ul {
            list-style: none;
        }

        .skill-category li {
            color: #d1d5db;
            margin-bottom: 8px;
            display: flex;
            gap: 8px;
        }

        .skill-category li::before {
            content: "▸";
            color: #22d3ee;
            margin-top: 2px;
        }

        .cert-list {
            max-width: 800px;
            margin: 0 auto;
        }

        .cert-item {
            background: rgba(30, 41, 59, 0.5);
            border: 1px solid rgba(59, 130, 246, 0.2);
            border-radius: 8px;
            padding: 24px;
            margin-bottom: 16px;
            transition: border-color 0.3s;
        }

        .cert-item:hover {
            border-color: rgba(34, 211, 238, 0.5);
        }

        .cert-content {
            display: flex;
            gap: 16px;
            align-items: flex-start;
        }

        .cert-icon {
            color: #22d3ee;
            flex-shrink: 0;
        }

        .cert-details h4 {
            font-size: 18px;
            margin-bottom: 4px;
        }

        .cert-issuer {
            color: #22d3ee;
            font-size: 14px;
            margin-bottom: 4px;
        }

        .cert-date {
            color: #9ca3af;
            font-size: 14px;
        }

        .education-item {
            background: rgba(30, 41, 59, 0.5);
            border: 1px solid rgba(59, 130, 246, 0.2);
            border-radius: 8px;
            padding: 24px;
            max-width: 800px;
            margin: 0 auto;
        }

        .education-content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 16px;
        }

        .education-content h3 {
            font-size: 24px;
            color: #22d3ee;
            margin-bottom: 8px;
        }

        .education-content h4 {
            font-size: 20px;
            color: #d1d5db;
        }

        .education-location {
            color: #9ca3af;
            margin-top: 8px;
        }

        .contact-box {
            background: rgba(30, 41, 59, 0.5);
            border: 1px solid rgba(59, 130, 246, 0.2);
            border-radius: 8px;
            padding: 32px;
            max-width: 700px;
            margin: 0 auto;
            text-align: center;
        }

        .contact-box p {
            color: #d1d5db;
            margin-bottom: 32px;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 24px;
        }

        .social-link {
            padding: 16px;
            border-radius: 8px;
            transition: all 0.3s;
            display: inline-block;
        }

        .social-link:hover {
            transform: translateY(-4px);
        }

        .social-link.email {
            background: #22d3ee;
        }

        .social-link.email:hover {
            background: #06b6d4;
        }

        .social-link.phone {
            background: #10b981;
        }

        .social-link.phone:hover {
            background: #059669;
        }

        .social-link.linkedin {
            background: #2563eb;
        }

        .social-link.linkedin:hover {
            background: #1d4ed8;
        }

        .social-link.github {
            background: #374151;
        }

        .social-link.github:hover {
            background: #1f2937;
        }

        .contact-info {
            color: #d1d5db;
        }

        .contact-info p {
            margin-bottom: 8px;
        }

        .contact-info span {
            color: #22d3ee;
            font-weight: 600;
        }

        footer {
            background: #0f172a;
            border-top: 1px solid rgba(59, 130, 246, 0.2);
            padding: 32px 0;
            text-align: center;
            color: #9ca3af;
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero h1 {
                font-size: 32px;
            }

            .hero h2 {
                font-size: 20px;
            }

            .btn-group {
                flex-direction: column;
            }

            .experience-header {
                flex-direction: column;
            }

            .experience-date {
                text-align: left;
            }

            .social-links {
                flex-wrap: wrap;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav class="container">
            <div class="logo">Jubril Adams</div>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#certifications">Certifications</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="about" class="hero">
        <div class="container">
            <div class="hero-icon">
                <i data-feather="server" width="64" height="64"></i>
            </div>
            <h1>Jubril Adams</h1>
            <h2>Cloud Support Engineer · System Administrator</h2>
            <p>
                Cloud Support Engineer and System Administrator with hands-on experience supporting users, managing Windows and Linux servers, and building cloud lab environments on AWS. Currently pursuing a B.S. in Cloud Computing at Western Governors University and applying IT support and healthcare experience to reliable, secure, and well-documented infrastructure.
            </p>
            <p class="location">📍 Palatine, IL, USA</p>
            <div class="btn-group">
                <a href="#contact" class="btn btn-primary">Download Resume</a>
                <a href="#projects" class="btn btn-secondary">View Projects</a>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="section-bg">
        <div class="container">
            <h2 class="section-title">
                <i data-feather="briefcase"></i>
                Professional Experience
            </h2>

            <div class="experience-item">
                <div class="experience-header">
                    <div class="experience-title">
                        <h3>IT Support Specialist</h3>
                        <h4>Aurora Home Care</h4>
                    </div>
                    <div class="experience-date">
                        <p>September 2025 - Present</p>
                        <p>Illinois, USA</p>
                    </div>
                </div>
                <ul>
                    <li>Provide front-line IT support for clinicians and staff, resolving issues with laptops, desktops, printers, and mobile devices.</li>
                    <li>Support users in healthcare environments, including EMR access, account issues, and secure remote connectivity.</li>
                    <li>Troubleshoot Windows and basic network problems (Wi‑Fi, VPN, printers) and document resolutions in tickets.</li>
                    <li>Assist with onboarding and offboarding, account setup, and permissions following company policies.</li>
                    <li>Escalate complex issues to senior admins while maintaining clear, empathetic communication with end users.</li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="experience-header">
                    <div class="experience-title">
                        <h3>Systems Administrator (Linux/Windows)</h3>
                        <h4>Clearbrook</h4>
                    </div>
                    <div class="experience-date">
                        <p>2014 - Present</p>
                        <p>Arlington Heights, IL</p>
                    </div>
                </div>
                <p class="experience-description">
                    Non-profit empowering children and adults with disabilities, serving thousands of individuals annually across multiple Chicagoland locations.
                </p>
                <ul>
                    <li>Provide on-site and remote support for servers, network devices, and user endpoints across branch offices and the main campus.</li>
                    <li>Manage network connectivity and basic security between branch offices and head office, coordinating with vendors as needed.</li>
                    <li>Support VoIP infrastructure using Cisco Unified Communications Manager and network printers, helping ensure minimal downtime.</li>
                    <li>Assist with routine maintenance, patching, and backups for Windows and Linux servers in collaboration with senior staff.</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <div class="container">
            <h2 class="section-title">
                <i data-feather="briefcase"></i>
                Featured Labs & Projects
            </h2>
            <div class="projects-grid">
                <div class="project-card">
