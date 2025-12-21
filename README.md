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
            <h2>Cloud Support Engineer · Systems Administrator</h2>
            <p>
                Cloud Support Engineer and Systems Administrator with 4+ years of hands-on experience supporting clinical and business users, administering Linux and Windows servers, and operating secure, highly available infrastructure in regulated environments. Proven track record of migrating mission-critical applications to AWS and Azure, reducing costs by 40% while maintaining 99.99% uptime. Skilled in Infrastructure as Code (Terraform, Ansible), CI/CD pipelines (Jenkins, GitHub Actions), and cloud operations (EC2, S3, RDS, Lambda, CloudWatch). Pursuing a B.S. in Cloud Computing at Western Governors University and targeting fully remote Cloud Support Engineer, Cloud Systems Administrator, and early-career DevOps Engineer roles.
            </p>
            <p class="location">📍 Palatine, IL, USA</p>
            <div class="btn-group">
                <a href="PATH_TO_RESUME" class="btn btn-primary" target="_blank" rel="noopener">
                    Download Resume (PDF)
                </a>
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
                        <h4>Secure &amp; Innovate</h4>
                    </div>
                    <div class="experience-date">
                        <p>Jan 2022 - Present</p>
                        <p>Remote · Contract</p>
                    </div>
                </div>
                <ul>
                    <li>Migrated mission-critical applications to AWS and Azure, using services such as EC2, S3, RDS, VPC, and IAM to reduce cloud infrastructure costs by 40% while maintaining 99.99% uptime.</li>
                    <li>Automated infrastructure provisioning and configuration with Terraform and Ansible, implementing Infrastructure as Code standards and cutting deployment times by 70%.</li>
                    <li>Designed and maintained CI/CD pipelines in Jenkins and GitHub Actions, integrating automated testing and approvals and reducing deployment errors by 60%.</li>
                    <li>Improved monitoring and incident management by leveraging CloudWatch, centralized logging, and alerting, strengthening security and supporting SOC 2 compliance efforts.</li>
                    <li>Administered Linux and Windows servers across hybrid environments, handling patching, hardening, backup, and disaster recovery for approximately 100 end users.</li>
                    <li>Created Python and Bash automation scripts and configuration management routines that reduced manual server maintenance tasks by 50%.</li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="experience-header">
                    <div class="experience-title">
                        <h3>Health Information Technician / IT Support</h3>
                        <h4>Aurora Home Care Inc</h4>
                    </div>
                    <div class="experience-date">
                        <p>Aug 2025 - Present</p>
                        <p>Northbrook, IL</p>
                    </div>
                </div>
                <ul>
                    <li>Support and troubleshoot EHR and related healthcare applications for clinicians and administrative staff, resolving login issues, access problems, and workflow errors.</li>
                    <li>Work with IT teams on user access, permissions, and basic system maintenance to keep health information systems available and secure.</li>
                    <li>Ensure all handling of patient data complies with HIPAA and other privacy regulations, including proper authorization and release-of-information processes.</li>
                    <li>Maintain confidentiality, integrity, and security of electronic records through correct use of access controls, audit trails, and secure work practices.</li>
                    <li>Participate in quality control checks to make sure records are accurate, complete, and stored correctly in the organization's systems.</li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="experience-header">
                    <div class="experience-title">
                        <h3>Systems Administrator (Linux/Windows)</h3>
                        <h4>Clearbrook</h4>
                    </div>
                    <div class="experience-date">
                        <p>Jan 2020 - Feb 2023</p>
                        <p>Arlington Heights, IL</p>
                    </div>
                </div>
                <p class="experience-description">
                    Non-profit empowering children and adults with disabilities, serving thousands of individuals annually across multiple Chicagoland locations.
                </p>
                <ul>
                    <li>Delivered 24/7/365 support for core infrastructure, applications, and network connectivity, improving system reliability for a multi-site nonprofit with dozens of locations.</li>
                    <li>Administered Linux and Windows Server environments, including user management, patching, antivirus, and basic hardening, to support secure access for staff and clients.</li>
                    <li>Managed WAN connectivity and basic network security between 40+ branch offices and the head office, working with routers, switches, firewalls, VPNs, and DNS.</li>
                    <li>Designed and supported a Cisco Unified Communications Manager VoIP network for ~50 users, improving communication quality and uptime.</li>
                    <li>Implemented and documented network infrastructure for more than 150 networked printers, registers, and endpoints, reducing recurring incidents and improving change management.</li>
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
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="cloud"></i>
                        </div>
                        <div>
                            <h4>AWS Three-Tier Web Application Lab</h4>
                        </div>
                    </div>
                    <p>Designed and deployed a three-tier web application in an AWS lab environment using an Application Load Balancer, Auto Scaling groups, EC2, and RDS to practice high availability, VPC networking, monitoring with CloudWatch, and backup strategies.</p>
                    <div class="tech-tags">
                        <span class="tech-tag">AWS</span>
                        <span class="tech-tag">EC2</span>
                        <span class="tech-tag">RDS</span>
                        <span class="tech-tag">VPC</span>
                        <span class="tech-tag">CloudWatch</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="code"></i>
                        </div>
                        <div>
                            <h4>Infrastructure as Code for AWS VPC</h4>
                        </div>
                    </div>
                    <p>Built reusable Terraform configurations to provision VPCs, subnets, EC2 instances, and security groups, enabling consistent, version-controlled environments for testing and learning across multiple AWS regions.</p>
                    <div class="tech-tags">
                        <span class="tech-tag">Terraform</span>
                        <span class="tech-tag">AWS</span>
                        <span class="tech-tag">CloudFormation</span>
                        <span class="tech-tag">IaC</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="server"></i>
                        </div>
                        <div>
                            <h4>CI/CD Pipeline for a Demo App</h4>
                        </div>
                    </div>
                    <p>Implemented a CI/CD pipeline for a sample application using GitHub Actions and Jenkins in a lab environment, including automated builds, basic tests, and deployment to a test server with rollback capabilities.</p>
                    <div class="tech-tags">
                        <span class="tech-tag">Jenkins</span>
                        <span class="tech-tag">GitHub Actions</span>
                        <span class="tech-tag">Docker</span>
                        <span class="tech-tag">CI/CD</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="shield"></i>
                        </div>
                        <div>
                            <h4>Linux and Windows Home Lab with Active Directory</h4>
                        </div>
                    </div>
                    <p>Set up a mixed Linux and Windows lab with Active Directory, group policies, LDAP integration, and secure remote access to practice identity and access management and basic system hardening.</p>
                    <div class="tech-tags">
                        <span class="tech-tag">Active Directory</span>
                        <span class="tech-tag">Windows Server</span>
                        <span class="tech-tag">Linux</span>
                        <span class="tech-tag">VPN</span>
                        <span class="tech-tag">Group Policy</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="cpu"></i>
                        </div>
                        <div>
                            <h4>Network Fundamentals Lab</h4>
                        </div>
                    </div>
                    <p>Practiced routing protocols and network troubleshooting in a virtual lab using EIGRP, OSPF, and static routing to strengthen core networking fundamentals and improve diagnostic skills.</p>
                    <div class="tech-tags">
                        <span class="tech-tag">TCP/IP</span>
                        <span class="tech-tag">EIGRP</span>
                        <span class="tech-tag">OSPF</span>
                        <span class="tech-tag">Routing</span>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-icon">
                            <i data-feather="file-text"></i>
                        </div>
                        <div>
                            <h4>Automation & Scripting Toolkit</h4>
                        </div>
                    </div>
                    <p>Developed a collection of Python, Bash, and PowerShell scripts to automate routine admin tasks, including log cleanup, health checks, and user account management, with comprehensive documentation on GitHub.</p>
                    <div class="tech-tags">
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">Bash</span>
                        <span class="tech-tag">PowerShell</span>
                        <span class="tech-tag">Automation</span>
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
                    <h4>Cloud & Platforms</h4>
                    <ul>
                        <li>AWS (EC2, S3, RDS, Lambda, VPC, IAM, CloudWatch, CloudFormation)</li>
                        <li>Microsoft Azure (VMs, Storage, Azure AD)</li>
                        <li>GCP (exposure)</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>Infrastructure as Code & Automation</h4>
                    <ul>
                        <li>Terraform</li>
                        <li>CloudFormation</li>
                        <li>Ansible (learning / lab use)</li>
                        <li>Python</li>
                        <li>PowerShell</li>
                        <li>Bash</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>Systems & Networking</h4>
                    <ul>
                        <li>Linux (RHEL, Ubuntu)</li>
                        <li>Windows Server</li>
                        <li>Active Directory</li>
                        <li>VPN</li>
                        <li>Load balancing, DNS, network security and hardening</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>DevOps & CI/CD</h4>
                    <ul>
                        <li>Jenkins</li>
                        <li>GitHub Actions</li>
                        <li>GitLab CI</li>
                        <li>Docker</li>
                        <li>Kubernetes (intro labs)</li>
                        <li>Git</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>Database, Storage & Reliability</h4>
                    <ul>
                        <li>MySQL (basic admin)</li>
                        <li>Patch management, backup and recovery, disaster recovery planning</li>
                        <li>CloudWatch, logging and alerting, performance tuning, incident response, on-call support, SOC 2 awareness</li>
                    </ul>
                </div>

                <div class="skill-category">
                    <h4>Healthcare IT</h4>
                    <ul>
                        <li>EHR/EMR support</li>
                        <li>HIPAA compliance and PHI security</li>
                        <li>Clinical workflow optimization</li>
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
                            <h4>CompTIA IT Operations Specialist (CIOS) Stackable Certification</h4>
                            <p class="cert-issuer">CompTIA</p>
                            <p class="cert-date">Issued Nov 2025 · Expires Nov 2028</p>
                        </div>
                    </div>
                </div>

                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>CompTIA Network+ ce</h4>
                            <p class="cert-issuer">CompTIA</p>
                            <p class="cert-date">Issued Nov 2025 · Expires Nov 2028</p>
                        </div>
                    </div>
                </div>

                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>CompTIA A+ ce</h4>
                            <p class="cert-issuer">CompTIA</p>
                            <p class="cert-date">Issued Jul 2025 · Expires Jul 2028</p>
                        </div>
                    </div>
                </div>

                <div class="cert-item">
                    <div class="cert-content">
                        <i data-feather="graduation-cap" class="cert-icon"></i>
                        <div class="cert-details">
                            <h4>Linux Essentials</h4>
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
                        <h3>B.S. Cloud Computing (In Progress)</h3>
                        <h4>Western Governors University</h4>
                        <p class="education-location">Salt Lake City, UT · Online</p>
                    </div>
                    <div>
                        <p class="cert-date">Expected Graduation: To be determined</p>
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
                <p>Open to fully remote Cloud Support Engineer, Cloud Systems Administrator, and early-career DevOps Engineer roles. Interested in collaborating or have a project in mind? Feel free to reach out.</p>
                <div class="social-links">
                    <a href="mailto:adam.jubril78@mail.com" class="social-link email" title="Email">
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
                    <p><span>Email:</span> adam.jubril78@mail.com</p>
                    <p><span>Phone:</span> 224-474-0556</p>
                    <p><span>Resume:</span> <a href="PATH_TO_RESUME" target="_blank" rel="noopener">View PDF</a></p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>© 2024 Jubril Adams – Cloud Support Engineer & Systems Administrator (AWS | Azure | Linux | Terraform). Built with HTML, CSS & JavaScript.</p>
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
