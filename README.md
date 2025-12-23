<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Jubril Adams - Cloud Support Engineer & Systems Administrator Portfolio">
    <title>Jubril Adams | Cloud & Systems Engineer</title>
    
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- Custom Stylesheet -->
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Sticky Navigation Bar -->
    <header>
        <nav id="navbar">
            <div class="nav-container">
                <div class="logo">
                    <a href="#home">JA</a>
                </div>
                <ul class="nav-menu" id="navMenu">
                    <li><a href="#home" class="nav-link active">Home</a></li>
                    <li><a href="#skills" class="nav-link">Skills</a></li>
                    <li><a href="#projects" class="nav-link">Projects</a></li>
                    <li><a href="#about" class="nav-link">About</a></li>
                    <li><a href="#contact" class="nav-link">Contact</a></li>
                </ul>
                <div class="hamburger" id="hamburger">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h1 class="hero-title">Jubril Adams</h1>
                <p class="hero-subtitle">Cloud & Systems Engineer</p>
                <p class="hero-description">
                    Cloud Support Engineer with 4+ years of experience in AWS, Azure, Linux/Windows administration, 
                    and Infrastructure as Code. Passionate about building secure, scalable cloud solutions.
                </p>
                <div class="hero-buttons">
                    <a href="#projects" class="btn btn-primary">View My Work</a>
                    <a href="#contact" class="btn btn-secondary">Get In Touch</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills">
        <div class="container">
            <h2 class="section-title">Core Competencies</h2>
            <div class="skills-grid">
                <!-- Cloud Platforms -->
                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-cloud"></i>
                    </div>
                    <h3>Cloud Platforms</h3>
                    <p>AWS (EC2, S3, RDS, Lambda, VPC, IAM), Azure (VMs, Storage, Azure AD), GCP</p>
                </div>

                <!-- Infrastructure as Code -->
                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-code"></i>
                    </div>
                    <h3>Infrastructure as Code</h3>
                    <p>Terraform, CloudFormation, Ansible, Python, Bash, PowerShell</p>
                </div>

                <!-- Linux & Windows -->
                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-server"></i>
                    </div>
                    <h3>Systems Administration</h3>
                    <p>Linux (RHEL, Ubuntu), Windows Server, Active Directory, System Hardening</p>
                </div>

                <!-- Networking -->
                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-network-wired"></i>
                    </div>
                    <h3>Networking</h3>
                    <p>VPN, Load Balancing, DNS, Network Security, EIGRP, OSPF, TCP/IP</p>
                </div>

                <!-- DevOps & CI/CD -->
                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-infinity"></i>
                    </div>
                    <h3>DevOps & CI/CD</h3>
                    <p>Jenkins, GitHub Actions, GitLab CI, Docker, Kubernetes, Git</p>
                </div>

                <!-- Security & Compliance -->
                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Security & Compliance</h3>
                    <p>SOC 2, HIPAA, CloudWatch Monitoring, Incident Response, Disaster Recovery</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects">
        <div class="container">
            <h2 class="section-title">Featured Projects & Labs</h2>
            <div class="projects-grid">
                <!-- Project 1 -->
                <div class="project-card">
                    <div class="project-header">
                        <i class="fas fa-diagram-project"></i>
                    </div>
                    <h3>AWS Three-Tier Web Application</h3>
                    <p>Designed and deployed a highly available three-tier application using Application Load Balancer, Auto Scaling, EC2, and RDS with CloudWatch monitoring.</p>
                    <div class="tech-stack">
                        <span class="tech-tag">AWS</span>
                        <span class="tech-tag">EC2</span>
                        <span class="tech-tag">RDS</span>
                        <span class="tech-tag">VPC</span>
                    </div>
                    <a href="https://github.com/jubriladams78" class="project-link" target="_blank">
                        <i class="fab fa-github"></i> View on GitHub
                    </a>
                </div>

                <!-- Project 2 -->
                <div class="project-card">
                    <div class="project-header">
                        <i class="fas fa-code-branch"></i>
                    </div>
                    <h3>Infrastructure as Code for AWS</h3>
                    <p>Built reusable Terraform configurations for VPCs, subnets, EC2 instances, and security groups across multiple AWS regions with version control.</p>
                    <div class="tech-stack">
                        <span class="tech-tag">Terraform</span>
                        <span class="tech-tag">AWS</span>
                        <span class="tech-tag">CloudFormation</span>
                    </div>
                    <a href="https://github.com/jubriladams78" class="project-link" target="_blank">
                        <i class="fab fa-github"></i> View on GitHub
                    </a>
                </div>

                <!-- Project 3 -->
                <div class="project-card">
                    <div class="project-header">
                        <i class="fas fa-rocket"></i>
                    </div>
                    <h3>CI/CD Pipeline Implementation</h3>
                    <p>Implemented automated CI/CD pipeline using GitHub Actions and Jenkins with automated builds, testing, and deployment with rollback capabilities.</p>
                    <div class="tech-stack">
                        <span class="tech-tag">Jenkins</span>
                        <span class="tech-tag">GitHub Actions</span>
                        <span class="tech-tag">Docker</span>
                    </div>
                    <a href="https://github.com/jubriladams78" class="project-link" target="_blank">
                        <i class="fab fa-github"></i> View on GitHub
                    </a>
                </div>

                <!-- Project 4 -->
                <div class="project-card">
                    <div class="project-header">
                        <i class="fas fa-users-cog"></i>
                    </div>
                    <h3>Active Directory Home Lab</h3>
                    <p>Set up hybrid Linux and Windows lab with Active Directory, group policies, LDAP integration, and secure remote access for identity management.</p>
                    <div class="tech-stack">
                        <span class="tech-tag">Active Directory</span>
                        <span class="tech-tag">Windows Server</span>
                        <span class="tech-tag">Linux</span>
                    </div>
                    <a href="https://github.com/jubriladams78" class="project-link" target="_blank">
                        <i class="fab fa-github"></i> View on GitHub
                    </a>
                </div>

                <!-- Project 5 -->
                <div class="project-card">
                    <div class="project-header">
                        <i class="fas fa-terminal"></i>
                    </div>
                    <h3>Automation & Scripting Toolkit</h3>
                    <p>Developed collection of Python, Bash, and PowerShell scripts for routine admin tasks including log cleanup, health checks, and user management.</p>
                    <div class="tech-stack">
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">Bash</span>
                        <span class="tech-tag">PowerShell</span>
                    </div>
                    <a href="https://github.com/jubriladams78" class="project-link" target="_blank">
                        <i class="fab fa-github"></i> View on GitHub
                    </a>
                </div>

                <!-- Project 6 -->
                <div class="project-card">
                    <div class="project-header">
                        <i class="fas fa-network-wired"></i>
                    </div>
                    <h3>Network Fundamentals Lab</h3>
                    <p>Practiced routing protocols and network troubleshooting using EIGRP, OSPF, and static routing to strengthen core networking fundamentals.</p>
                    <div class="tech-stack">
                        <span class="tech-tag">TCP/IP</span>
                        <span class="tech-tag">EIGRP</span>
                        <span class="tech-tag">OSPF</span>
                    </div>
                    <a href="https://github.com/jubriladams78" class="project-link" target="_blank">
                        <i class="fab fa-github"></i> View on GitHub
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title">About Me</h2>
            <div class="about-content">
                <div class="about-text">
                    <p class="about-intro">
                        I'm a Cloud Support Engineer and Systems Administrator with over 4 years of hands-on experience 
                        building and maintaining secure, highly available infrastructure in AWS and Azure. I specialize 
                        in Infrastructure as Code, CI/CD automation, and supporting mission-critical systems in regulated 
                        environments.
                    </p>
                    <div class="experience-highlights">
                        <h3>Key Achievements</h3>
                        <ul>
                            <li>
                                <i class="fas fa-check-circle"></i>
                                Migrated mission-critical applications to AWS and Azure, reducing infrastructure costs by 40% while maintaining 99.99% uptime
                            </li>
                            <li>
                                <i class="fas fa-check-circle"></i>
                                Automated infrastructure provisioning with Terraform and Ansible, cutting deployment times by 70%
                            </li>
                            <li>
                                <i class="fas fa-check-circle"></i>
                                Designed CI/CD pipelines in Jenkins and GitHub Actions, reducing deployment errors by 60%
                            </li>
                            <li>
                                <i class="fas fa-check-circle"></i>
                                Administered Linux and Windows servers for 100+ users across hybrid cloud environments
                            </li>
                            <li>
                                <i class="fas fa-check-circle"></i>
                                Implemented SOC 2 compliant monitoring and security practices using CloudWatch and centralized logging
                            </li>
                        </ul>
                    </div>
                    <div class="certifications">
                        <h3>Certifications</h3>
                        <div class="cert-badges">
                            <span class="cert-badge">AWS Solutions Architect Associate</span>
                            <span class="cert-badge">AWS Cloud Practitioner</span>
                            <span class="cert-badge">CompTIA Network+</span>
                            <span class="cert-badge">CompTIA A+</span>
                            <span class="cert-badge">Linux Essentials</span>
                        </div>
                    </div>
                    <div class="education">
                        <h3>Education</h3>
                        <p><strong>B.S. Cloud Computing</strong> (In Progress)<br>Western Governors University</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">Get In Touch</h2>
            <div class="contact-content">
                <div class="contact-info">
                    <h3>Contact Information</h3>
                    <div class="contact-item">
                        <i class="fas fa-envelope"></i>
                        <a href="mailto:adam.jubril78@mail.com">adam.jubril78@mail.com</a>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-phone"></i>
                        <a href="tel:224-474-0556">224-474-0556</a>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-map-marker-alt"></i>
                        <span>Palatine, IL, USA</span>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-briefcase"></i>
                        <span>Open to remote opportunities</span>
                    </div>
                    <div class="social-links">
                        <a href="https://linkedin.com/in/jubriladams" target="_blank" aria-label="LinkedIn">
                            <i class="fab fa-linkedin"></i>
                        </a>
                        <a href="https://github.com/jubriladams78" target="_blank" aria-label="GitHub">
                            <i class="fab fa-github"></i>
                        </a>
                        <a href="mailto:adam.jubril78@mail.com" aria-label="Email">
                            <i class="fas fa-envelope"></i>
                        </a>
                    </div>
                </div>

                <div class="contact-form-container">
                    <form id="contactForm" class="contact-form">
                        <div class="form-group">
                            <label for="name">Name</label>
                            <input type="text" id="name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" name="email" required>
                        </div>
                        <div class="form-group">
                            <label for="subject">Subject</label>
                            <input type="text" id="subject" name="subject" required>
                        </div>
                        <div class="form-group">
                            <label for="message">Message</label>
                            <textarea id="message" name="message" rows="5" required></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary">Send Message</button>
                        <div id="formMessage" class="form-message"></div>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <p>&copy; 2025 Jubril Adams. All rights reserved.</p>
                <div class="footer-links">
                    <a href="https://linkedin.com/in/jubriladams" target="_blank" aria-label="LinkedIn">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="https://github.com/jubriladams78" target="_blank" aria-label="GitHub">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="mailto:adam.jubril78@mail.com" aria-label="Email">
                        <i class="fas fa-envelope"></i>
                    </a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Custom JavaScript -->
    <script src="script.js"></script>
</body>
</html>
