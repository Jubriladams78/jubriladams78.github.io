<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Cloud & Systems Engineer Portfolio</title>
</head>
<body>
  <!-- Navigation -->
  <header class="site-header">
    <nav class="nav-bar">
      <a href="#hero" class="nav-logo">Your Name</a>
      <button class="nav-toggle" aria-label="Toggle navigation">
        <!-- Optional: Add icon via CSS/JS later -->
      </button>
      <ul class="nav-links">
        <li><a href="#hero">Home</a></li>
        <li><a href="#highlights">Highlights</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <!-- Hero Section -->
    <section id="hero" class="hero-section">
      <div class="hero-content">
        <p class="hero-availability">Open to Cloud Support Engineer & Junior System Administrator roles starting in 2026.</p>
        <h1 class="hero-title">Your Name</h1>
        <h2 class="hero-subtitle">Cloud &amp; Systems Engineer</h2>
        <p class="hero-value">
          Helping teams build reliable, secure, and well-documented cloud and on‑prem environments through hands‑on AWS, Linux, and automation experience.
        </p>
        <div class="hero-actions">
          <a href="#projects" class="btn btn-primary">View Cloud Projects</a>
          <!-- Replace # with your actual LinkedIn profile URL -->
          <a href="#" class="btn btn-linkedin">View my LinkedIn</a>
        </div>
      </div>
    </section>

    <!-- Highlights Section -->
    <section id="highlights" class="highlights-section">
      <header class="section-header">
        <h2>Professional Highlights</h2>
      </header>
      <ul class="highlights-list">
        <li>3+ years supporting users, servers, and networks with a strong track record of closing tickets quickly and preventing repeat issues.</li>
        <li>Hands‑on cloud labs in AWS, Linux administration, networking, and security with a focus on troubleshooting and root‑cause analysis.</li>
        <li>CompTIA A+, Network+, Security+, and Linux Essentials certified with active studies in AWS and cloud‑native tooling.</li>
        <li>Experience building a home lab that mirrors real‑world environments: AD, Linux servers, monitoring, backups, and scripted automation.</li>
      </ul>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects-section">
      <header class="section-header">
        <h2>Cloud &amp; Systems Projects</h2>
        <p class="section-subtitle">
          Realistic labs and home‑lab builds that demonstrate troubleshooting, automation, and platform ownership.
        </p>
      </header>

      <div class="projects-grid">
        <!-- Project Card 1 -->
        <!-- Replace project title, description, tech list, and link with your real project details -->
        <article class="project-card">
          <h3 class="project-title">AWS Multi‑Tier Web Application Lab</h3>
          <p class="project-description">
            Designed and deployed a highly available web application using separate public and private subnets. Implemented secure access, monitoring, and backup strategies to simulate a production‑like environment.
          </p>
          <p class="project-details">
            <strong>What I did:</strong> Built VPC with subnets, Internet/NAT gateways, EC2 instances behind a load balancer, and RDS in private subnets. Configured security groups, IAM roles, CloudWatch alarms, and automated backups.
          </p>
          <p class="project-tech">
            <strong>Technologies:</strong> AWS VPC, EC2, RDS, IAM, ALB, CloudWatch, S3, Linux
          </p>
          <a href="#" class="project-link">View on GitHub / Docs</a>
        </article>

        <!-- Project Card 2 -->
        <article class="project-card">
          <h3 class="project-title">Home Lab: Active Directory &amp; Linux Integration</h3>
          <p class="project-description">
            Built a Windows and Linux home lab to mirror a small organization’s environment, focusing on identity, access, and centralized management.
          </p>
          <p class="project-details">
            <strong>What I did:</strong> Deployed Windows Server for AD DS, DNS, and DHCP. Joined Windows and Linux clients to the domain, created OUs and Group Policies, and configured file shares and permissions for different departments.
          </p>
          <p class="project-tech">
            <strong>Technologies:</strong> Windows Server, Active Directory, Group Policy, Rocky Linux, VirtualBox/VMware, DNS, DHCP
          </p>
          <a href="#" class="project-link">View on GitHub / Docs</a>
        </article>

        <!-- Project Card 3 -->
        <article class="project-card">
          <h3 class="project-title">Linux Server Hardening &amp; Monitoring</h3>
          <p class="project-description">
            Hardened a Linux server and implemented monitoring to improve visibility and security for system services and resources.
          </p>
          <p class="project-details">
            <strong>What I did:</strong> Configured firewall rules, SSH hardening, and user/group policies. Set up system metrics collection and alerting, and documented remediation steps for common CPU, memory, and disk issues.
          </p>
          <p class="project-tech">
            <strong>Technologies:</strong> Rocky Linux, SSH, firewalld/ufw, log analysis, monitoring tools (e.g., Prometheus/Grafana), Bash
          </p>
          <a href="#" class="project-link">View on GitHub / Docs</a>
        </article>

        <!-- Project Card 4 -->
        <article class="project-card">
          <h3 class="project-title">AWS S3 Backup &amp; Recovery Automation</h3>
          <p class="project-description">
            Implemented an automated backup solution to protect critical files and demonstrate disaster recovery readiness.
          </p>
          <p class="project-details">
            <strong>What I did:</strong> Wrote scripts to sync local or on‑prem data to S3 with lifecycle policies and versioning. Tested recovery scenarios and documented Recovery Time Objective (RTO) and Recovery Point Objective (RPO).
          </p>
          <p class="project-tech">
            <strong>Technologies:</strong> AWS S3, IAM, CLI, Bash/Python, versioning, lifecycle rules
          </p>
          <a href="#" class="project-link">View on GitHub / Docs</a>
        </article>

        <!-- Project Card 5 -->
        <article class="project-card">
          <h3 class="project-title">Network Monitoring &amp; Uptime Dashboard</h3>
          <p class="project-description">
            Built a lightweight monitoring solution to track service availability and latency across home lab systems and cloud resources.
          </p>
          <p class="project-details">
            <strong>What I did:</strong> Created scripts to periodically check service endpoints and log response times and status. Visualized results in dashboards and configured alerts for key systems.
          </p>
          <p class="project-tech">
            <strong>Technologies:</strong> Python/Bash, ICMP/HTTP checks, Linux cron, time‑series database, dashboarding tool (e.g., Grafana)
          </p>
          <a href="#" class="project-link">View on GitHub / Docs</a>
        </article>

        <!-- Project Card 6 -->
        <article class="project-card">
          <h3 class="project-title">Infrastructure as Code Lab (Intro)</h3>
          <p class="project-description">
            Used infrastructure as code to provision repeatable cloud environments, reducing manual configuration and setup time.
          </p>
          <p class="project-details">
            <strong>What I did:</strong> Defined basic network, compute, and security resources in code. Tested creating and destroying environments, then iterated with variables and modules for reusability.
          </p>
          <p class="project-tech">
            <strong>Technologies:</strong> Terraform/CloudFormation, AWS (VPC, EC2), Git, CLI
          </p>
          <a href="#" class="project-link">View on GitHub / Docs</a>
        </article>

        <!-- Additional projects (optional 7–8) -->
        <!-- Duplicate a project-card block above and customize it for more projects -->
      </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills-section">
      <header class="section-header">
        <h2>Technical Skills</h2>
      </header>
      <div class="skills-grid">
        <section class="skills-category">
          <h3>Cloud Platforms</h3>
          <ul>
            <li>AWS: EC2, S3, IAM, VPC, RDS, CloudWatch, CloudFormation/Terraform (intro)</li>
            <li>Azure: Core compute, storage, and networking fundamentals</li>
          </ul>
        </section>
        <section class="skills-category">
          <h3>Linux &amp; Systems</h3>
          <ul>
            <li>Linux server administration (Rocky/Red Hat, Ubuntu)</li>
            <li>Users, groups, permissions, services, and package management</li>
            <li>Systemd, logging, and basic performance troubleshooting</li>
          </ul>
        </section>
        <section class="skills-category">
          <h3>Networking</h3>
          <ul>
            <li>TCP/IP, DNS, DHCP, routing, VPN concepts</li>
            <li>Subnets, security groups, and firewall rules</li>
            <li>Network diagnostics with ping, traceroute, and related tools</li>
          </ul>
        </section>
        <section class="skills-category">
          <h3>Security</h3>
          <ul>
            <li>Identity and access management, least privilege, and MFA</li>
            <li>OS hardening, patching, and basic vulnerability mitigation</li>
            <li>Backup, recovery, and incident response basics</li>
          </ul>
        </section>
        <section class="skills-category">
          <h3>Scripting &amp; Automation</h3>
          <ul>
            <li>Bash scripting for routine server and network tasks</li>
            <li>Python for automation, log parsing, and simple tools</li>
            <li>Git for version control and documentation of lab work</li>
          </ul>
        </section>
        <section class="skills-category">
          <h3>Tools &amp; Platforms</h3>
          <ul>
            <li>VirtualBox/VMware, Remote Desktop tools, SSH</li>
            <li>Monitoring and logging platforms (e.g., Prometheus, Grafana, CloudWatch)</li>
            <li>Ticketing and ITSM tools, documentation and knowledge base platforms</li>
          </ul>
        </section>
      </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about-section">
      <header class="section-header">
        <h2>About</h2>
      </header>
      <p class="about-text">
        IT support and system administration experience provides a strong foundation in troubleshooting, user support, and stable operations. Over time, this has evolved into a cloud‑focused path, building and documenting labs that look like the environments teams manage every day. The next step is to bring this hands‑on experience into a Cloud Support Engineer or Junior System Administrator role, where clear communication, reliable operations, and ownership of issues from alert to resolution truly matter.
      </p>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
      <header class="section-header">
        <h2>Contact &amp; LinkedIn</h2>
      </header>
      <div class="contact-content">
        <!-- Replace the placeholder values below with your real contact details -->
        <p><strong>Email:</strong> your.email@example.com</p>
        <p><strong>Location:</strong> Palatine, Illinois, USA</p>
        <!-- Replace # with your actual LinkedIn profile URL -->
        <a href="#" class="btn btn-linkedin-large">Connect on LinkedIn</a>
        <p class="contact-note">
          Open to remote and hybrid roles in Cloud Support, Junior System Administration, and related cloud infrastructure positions starting in 2026.
        </p>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <p>&copy; <span class="footer-year">2025</span> Your Name. All rights reserved.</p>
  </footer>
</body>
</html>
