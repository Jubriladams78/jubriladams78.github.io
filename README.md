<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Jubril Adams | Cloud &amp; Systems Engineer</title>
</head>
<body>
  <!-- Background (style with CSS later) -->
  <div class="bg-animation"></div>

  <!-- Navigation -->
  <header class="site-header">
    <nav id="navbar" class="nav-bar">
      <div class="nav-container">
        <div class="logo">Jubril Adams</div>
        <ul class="nav-links">
          <li><a href="#home" class="active">Home</a></li>
          <li><a href="#highlights">Highlights</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#skills">Skills</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
    </nav>
  </header>

  <main class="container">
    <!-- Hero Section -->
    <section id="home" class="hero-section">
      <div class="hero-content">
        <p class="hero-role">IT Support &amp; System Administrator → Cloud &amp; Systems Engineer</p>
        <p class="hero-availability">Open to Cloud Support Engineer &amp; Junior System Administrator roles starting in 2026.</p>
        <h1 class="hero-title">Jubril Adams</h1>
        <h2 class="hero-subtitle">Building reliable, secure, and well‑documented cloud and on‑prem environments.</h2>
        <p class="hero-summary">
          Cloud computing student and hands‑on lab builder with experience supporting users, servers, and networks. Focused on AWS, Linux, networking, and automation that reduces incidents and speeds up troubleshooting.
        </p>
        <div class="hero-actions">
          <a href="#projects" class="btn btn-primary">View Cloud Projects</a>
          <a href="#highlights" class="btn btn-secondary">See Experience Highlights</a>
          <!-- Replace URL with your real LinkedIn profile -->
          <a href="https://linkedin.com/in/jubriladams" class="btn btn-linkedin">View my LinkedIn</a>
        </div>
      </div>
    </section>

    <!-- Highlights Section -->
    <section id="highlights" class="highlights-section">
      <header class="section-header">
        <h2 class="section-title">Professional Highlights</h2>
        <p class="section-subtitle">
          A track record of reliable support work plus cloud labs that mirror real‑world environments.
        </p>
      </header>
      <ul class="highlights-list">
        <li>3+ years supporting users, servers, and networks with a strong record of resolving tickets and preventing repeat issues.</li>
        <li>Hands‑on labs in AWS, Linux, networking, security, and automation focused on troubleshooting and root‑cause analysis.</li>
        <li>CompTIA A+, Network+, Security+, and Linux Essentials certified; actively building AWS and cloud‑native skills.</li>
        <li>Home lab built with AD, Linux servers, monitoring, backups, and scripted tasks to simulate production environments.</li>
      </ul>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects-section">
      <header class="section-header">
        <h2 class="section-title">Cloud &amp; Systems Projects</h2>
        <p class="section-subtitle">
          Each project focuses on the problem solved, what was done, and the tools used.
        </p>
      </header>

      <div class="projects-grid">
        <!-- Project 1 -->
        <!-- Replace text and link with your real AWS multi-tier project -->
        <article class="project-card">
          <div class="project-media">🏗️</div>
          <div class="project-content">
            <h3 class="project-title">AWS Multi‑Tier Web Application Lab</h3>
            <p class="project-description">
              Designed and deployed a multi‑tier web application in AWS to practice high availability, secure network design, and observability.
            </p>
            <p class="project-details">
              <strong>What I did:</strong> Built a VPC with public and private subnets, Internet and NAT gateways, EC2 instances behind an Application Load Balancer, and RDS in private subnets. Configured security groups, IAM roles, CloudWatch alarms, and automated backups.
            </p>
            <p class="project-tech">
              <strong>Technologies:</strong> AWS, VPC, EC2, RDS, ALB, IAM, CloudWatch
            </p>
            <a href="https://github.com/jubriladams78" class="project-link">View on GitHub</a>
          </div>
        </article>

        <!-- Project 2 -->
        <article class="project-card">
          <div class="project-media">🧱</div>
          <div class="project-content">
            <h3 class="project-title">Home Lab: Active Directory &amp; Linux Integration</h3>
            <p class="project-description">
              Built a mixed Windows and Linux home lab to practice identity, access, and day‑to‑day systems administration.
            </p>
            <p class="project-details">
              <strong>What I did:</strong> Deployed Windows Server for AD DS, DNS, and DHCP. Joined Windows and Linux clients to the domain, created OUs and Group Policies, and set up role‑based file shares. Documented troubleshooting steps for login and name‑resolution issues.
            </p>
            <p class="project-tech">
              <strong>Technologies:</strong> Windows Server, Active Directory, Group Policy, Linux, DNS, DHCP
            </p>
            <a href="https://github.com/jubriladams78" class="project-link">View Lab Notes</a>
          </div>
        </article>

        <!-- Project 3 -->
        <article class="project-card">
          <div class="project-media">💾</div>
          <div class="project-content">
            <h3 class="project-title">AWS S3 Backup &amp; Recovery Automation</h3>
            <p class="project-description">
              Implemented automated backups to practice disaster recovery and data protection fundamentals.
            </p>
            <p class="project-details">
              <strong>What I did:</strong> Wrote scripts to sync local or on‑prem data to S3 with versioning and lifecycle policies. Tested restore scenarios and documented RTO/RPO so non‑technical stakeholders can understand recovery expectations.
            </p>
            <p class="project-tech">
              <strong>Technologies:</strong> AWS S3, IAM, Bash, Python, versioning, lifecycle rules
            </p>
            <a href="https://github.com/jubriladams78" class="project-link">View Scripts &amp; Docs</a>
          </div>
        </article>

        <!-- Project 4 -->
        <article class="project-card">
          <div class="project-media">📡</div>
          <div class="project-content">
            <h3 class="project-title">Network Monitoring &amp; Uptime Dashboard</h3>
            <p class="project-description">
              Built a lightweight monitoring setup to track service availability and latency for lab systems and cloud resources.
            </p>
            <p class="project-details">
              <strong>What I did:</strong> Created checks for key endpoints, logged response times and status codes, and fed metrics into dashboards. Configured alerts for priority services to practice incident response and runbook‑driven troubleshooting.
            </p>
            <p class="project-tech">
              <strong>Technologies:</strong> Linux, Bash/Python, Prometheus, Grafana
            </p>
            <a href="https://github.com/jubriladams78" class="project-link">View Dashboards</a>
          </div>
        </article>

        <!-- Project 5 -->
        <article class="project-card">
          <div class="project-media">⚙️</div>
          <div class="project-content">
            <h3 class="project-title">Intro Infrastructure as Code Lab</h3>
            <p class="project-description">
              Used infrastructure as code to provision repeatable AWS environments instead of manual configuration.
            </p>
            <p class="project-details">
              <strong>What I did:</strong> Defined basic VPC, networking, security groups, and EC2 instances in Terraform/CloudFormation. Practiced creating and destroying environments and versioning changes in Git.
            </p>
            <p class="project-tech">
              <strong>Technologies:</strong> Terraform, CloudFormation, AWS, Git
            </p>
            <a href="https://github.com/jubriladams78" class="project-link">View IaC Code</a>
          </div>
        </article>

        <!-- Project 6 (placeholder
