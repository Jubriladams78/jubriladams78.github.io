<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Jubril Adams | Cloud &amp; Systems Engineer</title>
</head>
<body>
  <!-- Header & Navigation -->
  <header id="top">
    <nav class="site-nav">
      <div class="nav-container">
        <div class="nav-brand">
          <span class="nav-name">Jubril Adams</span>
          <span class="nav-title">Cloud &amp; Systems Engineer</span>
        </div>
        <button class="nav-toggle" aria-label="Toggle navigation">
          <!-- Icon handled via CSS/JS -->
        </button>
        <ul class="nav-links">
          <li><a href="#hero">Home</a></li>
          <li><a href="#skills">Skills</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
    </nav>
  </header>

  <main>
    <!-- Hero -->
    <section id="hero" class="section section-hero">
      <div class="hero-inner">
        <p class="hero-kicker">Cloud Support Engineer &amp; Systems Administrator</p>
        <p class="hero-availability">Open to Cloud Support Engineer and Cloud / Systems roles starting in 2026.</p>
        <h1 class="hero-heading">Designing and supporting reliable, secure cloud infrastructure.</h1>
        <p class="hero-bio">
          Cloud computing student and IT professional with 4+ years of experience across AWS, Azure, Linux, and Windows Server. 
          Focused on automation, observability, and secure operations that reduce incidents and keep services available.
        </p>
        <div class="hero-actions">
          <a href="#projects" class="btn btn-primary">View Cloud Projects</a>
          <a href="#contact" class="btn btn-secondary">Contact &amp; LinkedIn</a>
        </div>
      </div>
    </section>

    <!-- Skills -->
    <section id="skills" class="section section-skills">
      <header class="section-header">
        <h2>Technical Skills</h2>
        <p>Skills applied in home labs, professional roles, and hands‑on cloud projects.</p>
      </header>
      <div class="skills-grid">
        <article class="skill-card">
          <h3>Cloud Platforms</h3>
          <p>AWS (EC2, S3, RDS, Lambda, VPC, IAM, CloudWatch, CloudFormation) and Azure (VMs, Storage, Azure AD).</p>
        </article>
        <article class="skill-card">
          <h3>Linux &amp; Systems</h3>
          <p>Linux (RHEL, Ubuntu), Windows Server, Active Directory, patching, hardening, backup, and recovery.</p>
        </article>
        <article class="skill-card">
          <h3>Networking</h3>
          <p>VPC design, subnets, VPN, load balancing, DNS, routing, and secure connectivity patterns.</p>
        </article>
        <article class="skill-card">
          <h3>Security</h3>
          <p>IAM, least privilege, encryption, logging and alerting, SOC 2 awareness, and HIPAA‑aligned practices.</p>
        </article>
        <article class="skill-card">
          <h3>Scripting &amp; Automation</h3>
          <p>Terraform, CloudFormation, Ansible, Python, Bash, and PowerShell for IaC and operational automation.</p>
        </article>
        <article class="skill-card">
          <h3>DevOps &amp; Monitoring</h3>
          <p>Jenkins, GitHub Actions, Docker, Kubernetes labs, CloudWatch, centralized logging, and incident response.</p>
        </article>
      </div>
    </section>

    <!-- Projects -->
    <section id="projects" class="section section-projects">
      <header class="section-header">
        <h2>Projects &amp; Portfolio</h2>
        <p>Selected projects that show how cloud, systems, and automation skills translate into real impact.</p>
      </header>

      <div class="projects-grid">
        <!-- Project 1 -->
        <article class="project-card">
          <h3 class="project-title">AWS Three‑Tier Web Application Lab</h3>
          <p class="project-description">
            Designed and deployed a three‑tier web application in AWS to practice highly available, production‑style architectures.
          </p>
          <p class="project-description">
            Built a VPC with public and private subnets, ALB, Auto Scaling, EC2, and RDS, then added CloudWatch monitoring and automated backups to validate reliability and recovery.
          </p>
          <p class="project-tech">
            <strong>Tech stack:</strong> AWS VPC, EC2, ALB, Auto Scaling, RDS, IAM, CloudWatch
          </p>
          <!-- Replace href with the specific GitHub repo when ready -->
          <a href="https://github.com/Jubriladams78" class="project-link">View on GitHub</a>
        </article>

        <!-- Project 2 -->
        <article class="project-card">
          <h3 class="project-title">Infrastructure as Code for AWS VPC</h3>
          <p class="project-description">
            Created reusable Terraform configurations to standardize VPCs, subnets, security groups, and EC2 instances across environments.
          </p>
          <p class="project-description">
            Introduced version‑controlled infrastructure, reducing manual setup, configuration drift, and time‑to‑provision new environments.
          </p>
          <p class="project-tech">
            <strong>Tech stack:</strong> Terraform, AWS (VPC, EC2, security groups), Git
          </p>
          <a href="https://github.com/Jubriladams78" class="project-link">View on GitHub</a>
        </article>

        <!-- Project 3 -->
        <article class="project-card">
          <h3 class="project-title">CI/CD Pipeline for Demo Application</h3>
          <p class="project-description">
            Implemented CI/CD pipelines using GitHub Actions and Jenkins to automate builds, tests, and deployments for a demo app.
          </p>
          <p class="project-description">
            Added basic quality gates and rollback‑capable jobs, improving release consistency and shortening deployment cycles.
          </p>
          <p class="project-tech">
            <strong>Tech stack:</strong> GitHub Actions, Jenkins, Docker, Git
          </p>
          <a href="https://github.com/Jubriladams78" class="project-link">View on GitHub</a>
        </article>

        <!-- Project 4 -->
        <article class="project-card">
          <h3 class="project-title">Cloud Monitoring &amp; Incident Response Lab</h3>
          <p class="project-description">
            Configured metrics, logs, and alerts to build an actionable view of application and infrastructure health in AWS.
          </p>
          <p class="project-description">
            Practiced end‑to‑end incident response using dashboards and runbooks to quickly identify root causes and restore service.
          </p>
          <p class="project-tech">
            <strong>Tech stack:</strong> AWS CloudWatch, log aggregation, alerting, dashboards
          </p>
          <a href="https://github.com/Jubriladams78" class="project-link">View on GitHub</a>
        </article>

        <!-- Project 5 -->
        <article class="project-card">
          <h3 class="project-title">Linux &amp; Windows Systems Administration Lab</h3>
          <p class="project-description">
            Built a mixed Linux and Windows environment to practice patching, hardening, access management, and backup strategy.
          </p>
          <p class="project-description">
            Documented repeatable procedures for user onboarding, updates, and recovery to mirror real service‑desk and sysadmin work.
          </p>
          <p class="project-tech">
            <strong>Tech stack:</strong> Linux (RHEL, Ubuntu), Windows Server, Active Directory, backup tools
          </p>
          <a href="https://github.com/Jubriladams78" class="project-link">View on GitHub</a>
        </article>

        <!-- Project 6 -->
        <article class="project-card">
          <h3 class="project-title">Healthcare IT Support &amp; EHR Environment</h3>
          <p class="project-description">
            Supported EHR and healthcare applications, focusing on uptime, secure access, and clinician productivity.
          </p>
          <p class="project-description">
            Resolved login and workflow issues, maintained access controls, and upheld HIPAA requirements for patient data.
          </p>
          <p class="project-tech">
            <strong>Tech stack:</strong> EHR systems, Windows, networking, HIPAA, access control
          </p>
          <a href="https://github.com/Jubriladams78" class="project-link">View supporting docs</a>
        </article>
      </div>
    </section>

    <!-- About -->
    <section id="about" class="section section-about">
      <header class="section-header">
        <h2>About</h2>
      </header>
      <div class="about-layout">
        <p class="about-text">
          Cloud Support Engineer and Systems Administrator with a background in healthcare IT and cloud infrastructure. 
          Comfortable owning issues from first alert to resolution, collaborating with cross‑functional teams, and documenting clear runbooks and procedures.
        </p>
        <ul class="about-points">
          <li>4+ years supporting cloud and on‑prem environments across AWS, Azure, Linux, and Windows.</li>
          <li>Experience reducing cloud costs, improving uptime, and automating repetitive provisioning tasks.</li>
          <li>Strong focus on security, compliance, and reliable operations in regulated environments.</li>
          <li>Enjoys mentoring users, simplifying complex topics, and leaving systems better documented than they were found.</li>
        </ul>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="section section-contact">
      <header class="section-header">
        <h2>Contact</h2>
        <p>If this experience aligns with your team, use the form or contact details below to connect.</p>
      </header>
      <div class="contact-layout">
        <!-- Contact Form -->
        <form class="contact-form">
          <div class="form-row">
            <label for="name">Name</label>
            <input id="name" name="name" type="text" required>
          </div>
          <div class="form-row">
            <label for="email">Email</label>
            <input id="email" name="email" type="email" required>
          </div>
          <div class="form-row">
            <label for="subject">Subject</label>
            <input id="subject" name="subject" type="text" required>
          </div>
          <div class="form-row">
            <label for="message">Message</label>
            <textarea id="message" name="message" rows="5" required></textarea>
          </div>
          <button type="submit" class="btn btn-primary">Submit</button>
        </form>

        <!-- Contact Details -->
        <div class="contact-details">
          <h3>Contact Details</h3>
          <p><strong>Email:</strong> <a href="mailto:adam.jubril78@gmail.com">adam.jubril78@gmail.com</a></p>
          <p><strong>Phone:</strong> <a href="tel:224-474-0556">224‑474‑0556</a></p>
          <p><strong>Location:</strong> Palatine, IL, USA</p>
          <h3>Connect</h3>
          <ul class="contact-links">
            <li><a href="https://www.linkedin.com/in/jubriladams">LinkedIn</a></li>
            <li><a href="https://github.com/Jubriladams78">GitHub</a></li>
            <li><a href="mailto:adam.jubril78@gmail.com">Email Me</a></li>
          </ul>
        </div>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <div class="footer-inner">
      <div class="footer-social">
        <a href="https://www.linkedin.com/in/jubriladams" class="footer-icon-link">LinkedIn</a>
        <a href="https://github.com/Jubriladams78" class="footer-icon-link">GitHub</a>
        <a href="mailto:adam.jubril78@gmail.com" class="footer-icon-link">Email</a>
      </div>
      <p class="footer-copy">&copy; 2025 Jubril Adams. All rights reserved.</p>
    </div>
  </footer>
</body>
</html>
