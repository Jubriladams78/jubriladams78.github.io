<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jubril Adams - Cloud Systems Administrator</title>
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

        /* Header */
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

        /* Hero Section */
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

        /* Section Styles */
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

        /* Experience Section */
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

        /* Projects Grid */
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

        /* Skills Grid */
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

        /* Certifications */
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

        /* Education */
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

        /* Contact Section */
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
            margin-bottom: 24px;
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

        /* Footer */
        footer {
            background: #0f172a;
            border-top: 1px solid rgba(59, 130, 246, 0.2);
            padding: 32px 0;
            text-align: center;
            color: #9ca3af;
        }

        /* Responsive */
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
            <h2>Cloud Systems Administrator</h2>
            <p>
                Results-driven Cloud System Administrator with 5 years of success designing, deploying, and securing 
                enterprise cloud infrastructure across AWS, Azure, and hybrid environments. Currently pursuing B.S. in 
                Cloud Computing at Western Governors University.
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
                        <h3>Cloud Systems Administrator</h3>
                        <h4>Secure & IT</h4>
                    </div>
                    <div class="experience-date">
                        <p>2020 - Present</p>
                        <p>Madrid, Spain</p>
                    </div>
                </div>
                <ul>
                    <li>Migrated to AWS/Azure, reducing costs by 40%, uptime to 99.99%</li>
                    <li>Automated with Terraform/Ansible, cutting provisioning time 70%</li>
                    <li>Set up CI/CD with Jenkins, cutting errors 60%</li>
                    <li>Led SOC 2 compliance, reducing incidents by 60%</li>
                    <li>Responsible for servers, server room, and end users (100+ users)</li>
                    <li>Implemented new inventory management system, saving $100,000/year</li>
                    <li>Managed connectivity of 130 retail locations</li>
                    <li>Implemented WAN protocols: EIGRP, OSPF, BGP, and RIP</li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="experience-header">
                    <div class="experience-title">
                        <h3>Systems Administrator (Linux/Windows)</h3>
                        <h4>Clearbrook</h4>
                    </div>
                    <div class="experience-date">
                        <p>2014 - 2019</p>
                        <p>Arlington Heights, IL</p>
                    </div>
                </div>
                <p class="experience-description">
                    Non-profit empowering children and adults with disabilities. Illinois's largest provider, 
                    serving 8,000+ annually across 80 Chicagoland locations.
                </p>
                <ul>
                    <li>24/7/365 availability for critical restarts of infrastructure, software, and hardware</li>
                    <li>Managed network connectivity and security between 40 branch offices and head office</li>
                    <li>Designed & developed VoIP network using Cisco Unified Communications Manager for 50 users</li>
                    <li>Designed and implemented network infrastructure with 150+ network printers and registers</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <div class="container">
            <h2 class="section-title">
                <i data-feather="briefcase"></i>
                Featured Projects
            </h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="cloud"></i>
                        </div>
                        <div>
                            <h4>AWS/Azure Cloud Migration</h4>
                        </div>
                    </div>
                    <p>Migrated enterprise infrastructure to AWS/Azure, reducing operational costs by 40% and achieving 99.99% uptime</p>
                    <div class="tech-tags">
                        <span class="tech-tag">AWS</span>
                        <span class="tech-tag">Azure</span>
                        <span class="tech-tag">Terraform</span>
                        <span class="tech-tag">Ansible</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="code"></i>
                        </div>
                        <div>
                            <h4>Infrastructure Automation</h4>
                        </div>
                    </div>
                    <p>Automated systems provisioning with Terraform and Ansible, cutting deployment time by 70%</p>
                    <div class="tech-tags">
                        <span class="tech-tag">Terraform</span>
                        <span class="tech-tag">Ansible</span>
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">CloudFormation</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="server"></i>
                        </div>
                        <div>
                            <h4>CI/CD Pipeline Implementation</h4>
                        </div>
                    </div>
                    <p>Set up Jenkins CI/CD pipeline, decreasing deployment errors by 60%</p>
                    <div class="tech-tags">
                        <span class="tech-tag">Jenkins</span>
                        <span class="tech-tag">Docker</span>
                        <span class="tech-tag">Kubernetes</span>
                        <span class="tech-tag">Git</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="shield"></i>
                        </div>
                        <div>
                            <h4>SOC 2 Compliance & Security</h4>
                        </div>
                    </div>
                    <p>Led SOC 2 compliance initiative, reducing security incidents by 60%</p>
                    <div class="tech-tags">
                        <span class="tech-tag">CloudWatch</span>
                        <span class="tech-tag">VPN</span>
                        <span class="tech-tag">Network Security</span>
                        <span class="tech-tag">Active Directory</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="server"></i>
                        </div>
                        <div>
                            <h4>Multi-Location Network Management</h4>
                        </div>
                    </div>
                    <p>Managed network connectivity and security between 40 branch offices and head office, supporting 130+ retail locations</p>
                    <div class="tech-tags">
                        <span class="tech-tag">EIGRP</span>
                        <span class="tech-tag">OSPF</span>
                        <span class="tech-tag">BGP</span>
                        <span class="tech-tag">RIP</span>
                        <span class="tech-tag">TCP/IP</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="database"></i>
                        </div>
                        <div>
                            <h4>VoIP Infrastructure Deployment</h4>
                        </div>
                    </div>
                    <p>Designed and developed VoIP network using Cisco Unified Communications Manager for 50+ users</p>
                    <div class="tech-tags">
                        <span class="tech-tag">Cisco UCM</span>
                        <span class="tech-tag">VoIP</span>
                        <span class="tech-tag">Network Infrastructure</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="section-bg">
        <div class="container">
            <h2 class="section-title">Technical Skills</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h4>Cloud Platforms</h4>
                    <ul>
                        <li>AWS (EC2, S3, RDS, Lambda)</li>
                        <li>Microsoft Azure</li>
                        <li>CloudFormation</li>
                        <li>CloudWatch</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>System Administration</h4>
                    <ul>
                        <li>Linux</li>
                        <li>Windows Server</li>
                        <li>Active Directory</li>
                        <li>VPN</li>
                        <li>Network Security</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>Automation & IaC</h4>
                    <ul>
                        <li>Terraform</li>
                        <li>Ansible</li>
                        <li>Python</li>
                        <li>PowerShell</li>
                        <li>Bash</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>Networking</h4>
                    <ul>
                        <li>TCP/IP</li>
                        <li>EIGRP</li>
                        <li>OSPF</li>
                        <li>BGP</li>
                        <li>RIP</li>
                        <li>Cisco UCM</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>DevOps & CI/CD</h4>
                    <ul>
                        <li>Jenkins</li>
                        <li>Docker</li>
                        <li>Kubernetes</li>
                        <li>Git</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>Database & Storage</h4>
                    <ul>
                        <li>MySQL</li>
                        <li>Patch Management</li>
                        <li>Infrastructure</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Certifications Section -->
    <section id="certifications" class="section-bg">
        <div class="container">
            <h2 class="section-title">
                <i data-feather="award"></i>
                Certifications
            </h2>
            <div class="cert-list">
                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>AWS Certified Solutions Architect – Associate</h4>
                            <p class="cert-issuer">Amazon Web Services (AWS)</p>
                            <p class="cert-date">Issued Oct 2024 · Expires Oct 2027</p>
                        </div>
                    </div>
                </div>

                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>AWS Certified Cloud Practitioner</h4>
                            <p class="cert-issuer">Amazon Web Services (AWS)</p>
                            <p class="cert-date">Issued May 2025 · Expires May 2028</p>
                        </div>
                    </div>
                </div>

                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>CompTIA IT Operations Specialist – CIOS Stackable Certification</h4>
                            <p class="cert-issuer">CompTIA</p>
                            <p class="cert-date">Issued Nov 2025 · Expires Nov 2028</p>
                        </div>
                    </div>
                </div>

                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>CompTIA Network+ ce Certification</h4>
                            <p class="cert-issuer">CompTIA</p>
                            <p class="cert-date">Issued Nov 2025 · Expires Nov 2028</p>
                        </div>
                    </div>
                </div>

                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>CompTIA A+ ce Certification</h4>
                            <p class="cert-issuer">CompTIA</p>
                            <p class="cert-date">Issued Jul 2025 · Expires Jul 2028</p>
                        </div>
                    </div>
                </div>

                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>Linux Essentials Certification</h4>
                            <p class="cert-issuer">Linux Professional Institute (LPI)</p>
                            <p class="cert-date">Issued Jul 2025</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education">
        <div class="container">
            <h2 class="section-title">
                <i data-feather="graduation-cap"></i>
                Education
            </h2>
            <div class="education-item">
                <div class="education-content">
                    <div>
                        <h3>B.S. Cloud Computing</h3>
                        <h4>Western Governors University</h4>
                        <p class="education-location">Salt Lake City, UT</p>
                    </div>
                    <div>
                        <p class="cert-date">2006 - 2010</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section-bg">
        <div class="container">
            <h2 class="section-title">Get In Touch</h2>
            <div class="contact-box">
                <p>Interested in collaborating or have a project in mind? Feel free to reach out!</p>
                <div class="social-links">
                    <a href="mailto:jubril.adams@jjadams.pro" class="social-link email" title="Email">
                        <i data-feather="mail" width="28" height="28"></i>
                    </a>
                    <a href="tel:+12244740556" class="social-link phone" title="Phone">
                        <i data-feather="phone" width="28" height="28"></i>
                    </a>
                    <a href="https://www.linkedin.com/in/jubriladams" target="_blank" class="social-link linkedin" title="LinkedIn">
                        <i data-feather="linkedin" width="28" height="28"></i>
                    </a>
                    <a href="https://github.com/Jubriladams78" target="_blank" class="social-link github" title="GitHub">
                        <i data-feather="github" width="28" height="28"></i>
                    </a>
                </div>
                <div class="contact-info">
                    <p><span>Email:</span> jubril.adams@jjadams.pro</p>
                    <p><span>Phone:</span> 224-474-0556</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>© 2024 Jubril Adams - Cloud Systems Administrator. Built with HTML, CSS & JavaScript.</p>
        </div>
    </footer>

    <script>
        // Initialize Feather Icons
        feather.replace();

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
    </script>
</body>
</html>
