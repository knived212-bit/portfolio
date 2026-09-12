<!DOCTYPE html>
<html lang="en" data-theme="emerald">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Nived Krishna S R | Software Engineer & Developer</title>
  <meta name="description" content="Portfolio of Nived Krishna S R - Computer Science & Engineering undergraduate specializing in C++, Python, JavaScript, Kotlin, IoT Systems, and Web Applications." />
  <meta name="keywords" content="Nived Krishna S R, Portfolio, Software Engineer, Python, C++, Kotlin, JavaScript, MongoDB, Android Studio, IoT, Web Developer" />
  <meta name="author" content="Nived Krishna S R" />

  <!-- Open Graph Meta Tags for social sharing -->
  <meta property="og:title" content="Nived Krishna S R | Developer Portfolio" />
  <meta property="og:description" content="Computer Science Engineer | C++, Python, JavaScript, Kotlin, IoT & Web Developer" />
  <meta property="og:type" content="website" />

  <!-- Stylesheet -->
  <link rel="stylesheet" href="css/style.css" />
</head>
<body>

  <!-- Interactive Constellation Particles Background -->
  <canvas id="particlesCanvas"></canvas>

  <!-- Ambient Glow & Cyber Grid Overlays -->
  <div class="ambient-glow glow-1"></div>
  <div class="ambient-glow glow-2"></div>
  <div class="bg-grid-overlay"></div>

  <!-- Toast Notification -->
  <div id="toast" class="toast" role="alert" aria-live="polite"></div>

  <!-- Header & Navigation -->
  <header class="header" id="header">
    <div class="container nav-container">
      <a href="#hero" class="brand-logo" aria-label="Nived Krishna S R Home">
        <span class="logo-symbol">&lt;</span><span class="logo-text">NK</span><span class="logo-symbol">/&gt;</span>
      </a>

      <!-- Desktop Nav -->
      <nav class="nav-menu" id="navMenu">
        <ul class="nav-list">
          <li><a href="#about" class="nav-link">About</a></li>
          <li><a href="#skills" class="nav-link">Skills</a></li>
          <li><a href="#projects" class="nav-link">Projects</a></li>
          <li><a href="#certifications" class="nav-link">Certifications</a></li>
          <li><a href="#education" class="nav-link">Education</a></li>
          <li><a href="#contact" class="nav-link">Contact</a></li>
        </ul>
      </nav>

      <!-- Nav Actions (Terminal, Theme & CTA) -->
      <div class="nav-actions">
        <!-- Interactive Terminal Trigger Button -->
        <button id="terminalBtn" class="terminal-trigger-btn" aria-label="Open Interactive CLI Terminal" title="Open Terminal (Ctrl+K)">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="4 17 10 11 4 5"></polyline><line x1="12" y1="19" x2="20" y2="19"></line></svg>
          <span>Terminal</span>
          <span class="kbd-shortcut">^K</span>
        </button>

        <!-- Palette Selector Menu -->
        <div class="theme-menu-wrapper">
          <button id="themePaletteBtn" class="theme-toggle" aria-label="Select Color Theme" title="Choose color theme">
            <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <circle cx="13.5" cy="6.5" r=".5" fill="currentColor"></circle>
              <circle cx="17.5" cy="10.5" r=".5" fill="currentColor"></circle>
              <circle cx="8.5" cy="7.5" r=".5" fill="currentColor"></circle>
              <circle cx="6.5" cy="12.5" r=".5" fill="currentColor"></circle>
              <path d="M12 2C6.5 2 2 6.5 2 12s4.5 10 10 10c.926 0 1.648-.746 1.648-1.688 0-.437-.18-.835-.437-1.125-.29-.289-.438-.652-.438-1.125a1.64 1.64 0 0 1 1.668-1.668h1.996c3.051 0 5.555-2.503 5.555-5.554C21.965 6.012 17.461 2 12 2z"></path>
            </svg>
          </button>
          <div class="theme-dropdown" id="themeDropdown">
            <div class="theme-dropdown-header">Color Themes</div>
            <div class="theme-options">
              <button class="theme-option" data-theme-set="emerald">
                <span class="theme-preview emerald-preview"></span>
                <span class="theme-name">Emerald Matrix</span>
              </button>
              <button class="theme-option" data-theme-set="nebula">
                <span class="theme-preview nebula-preview"></span>
                <span class="theme-name">Cosmic Nebula</span>
              </button>
              <button class="theme-option" data-theme-set="cyber">
                <span class="theme-preview cyber-preview"></span>
                <span class="theme-name">Cyber Indigo</span>
              </button>
              <button class="theme-option" data-theme-set="sunset">
                <span class="theme-preview sunset-preview"></span>
                <span class="theme-name">Sunset Crimson</span>
              </button>
              <button class="theme-option" data-theme-set="gold">
                <span class="theme-preview gold-preview"></span>
                <span class="theme-name">Luxury Amber</span>
              </button>
              <button class="theme-option" data-theme-set="light">
                <span class="theme-preview light-preview"></span>
                <span class="theme-name">Minimal Light</span>
              </button>
            </div>
          </div>
        </div>

        <!-- Quick Dark/Light Toggle -->
        <button id="themeToggle" class="theme-toggle" aria-label="Toggle dark/light mode" title="Toggle dark/light">
          <svg class="sun-icon icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <circle cx="12" cy="12" r="4"></circle>
            <path d="M12 2v2"></path>
            <path d="M12 20v2"></path>
            <path d="m4.93 4.93 1.41 1.41"></path>
            <path d="m17.66 17.66 1.41 1.41"></path>
            <path d="M2 12h2"></path>
            <path d="M20 12h2"></path>
            <path d="m6.34 17.66-1.41 1.41"></path>
            <path d="m19.07 4.93-1.41 1.41"></path>
          </svg>
          <svg class="moon-icon icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <path d="M12 3a6 6 0 0 0 9 9 9 9 0 1 1-9-9Z"></path>
          </svg>
        </button>

        <a href="#contact" class="btn btn-sm btn-primary">Hire Me</a>

        <button class="hamburger" id="hamburger" aria-label="Open menu" aria-expanded="false">
          <span></span>
          <span></span>
          <span></span>
        </button>
      </div>
    </div>
  </header>

  <!-- Interactive Terminal Modal -->
  <div id="terminalModal" class="terminal-modal" role="dialog" aria-modal="true">
    <div class="terminal-window">
      <div class="terminal-header">
        <div style="display: flex; align-items: center; gap: 0.5rem;">
          <span class="dot red"></span>
          <span class="dot yellow"></span>
          <span class="dot green"></span>
          <span class="terminal-title">nived-shell v2.4 (CLI)</span>
        </div>
        <button id="terminalClose" class="terminal-close-btn" aria-label="Close Terminal">&times;</button>
      </div>
      <div class="terminal-body">
        <div style="color: var(--text-dim); margin-bottom: 0.85rem;">
          Welcome to Nived Krishna's Interactive Terminal. Type <span style="color: var(--primary-light); font-weight: bold;">help</span> to see available commands.
        </div>
        <div id="terminalOutput"></div>
        <div class="terminal-prompt-line">
          <span class="terminal-user">visitor@nived-os:~$</span>
          <input type="text" id="terminalInput" class="terminal-input" autocomplete="off" spellcheck="false" autofocus />
        </div>
      </div>
    </div>
  </div>

  <main>
    <!-- HERO SECTION -->
    <section class="hero-section section" id="hero">
      <div class="container hero-container">
        <div class="hero-content">
          <div class="hero-meta-badge">
            <span class="status-dot"></span>
            <span>📍 Kozhikode, Kerala &bull; LPU Punjab</span>
          </div>
          <h1 class="hero-title">
            Hi, I'm <span class="gradient-text">Nived Krishna S R</span>
          </h1>
          <h2 class="hero-subtitle">
            I am a <span class="typing-text" id="typingText"></span><span class="cursor">|</span>
          </h2>
          <p class="hero-description">
            Computer Science and Engineering undergraduate at Lovely Professional University. Passionate about software architecture, embedded IoT security systems, and high-performance applications.
          </p>

          <div class="hero-cta-group">
            <a href="#projects" class="btn btn-primary">
              <span>Explore Projects</span>
              <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14"></path><path d="m12 5 7 7-7 7"></path></svg>
            </a>
            <a href="#contact" class="btn btn-secondary">
              <span>Get in Touch</span>
            </a>
          </div>

          <!-- Social Quick Links -->
          <div class="hero-socials">
            <a href="https://www.linkedin.com/in/nived-krishna-sr-b0583a377/" target="_blank" rel="noopener noreferrer" class="social-icon" aria-label="LinkedIn Profile" title="LinkedIn">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.46 10.9v8.37H9.2V10.9H6.46M7.83 6.64a1.65 1.65 0 0 0-1.66 1.66 1.66 1.66 0 0 0 1.66 1.65 1.65 1.65 0 0 0 1.65-1.65c0-.92-.74-1.66-1.65-1.66Z"/></svg>
            </a>
            <a href="https://github.com/knived212-bit" target="_blank" rel="noopener noreferrer" class="social-icon" aria-label="GitHub Profile" title="GitHub">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34-.46-1.16-1.11-1.47-1.11-1.47-.91-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.87 1.52 2.34 1.07 2.91.83.1-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.92 0-1.11.38-2 1.03-2.71-.1-.25-.45-1.29.1-2.64 0 0 .84-.27 2.75 1.02.79-.22 1.65-.33 2.5-.33.85 0 1.71.11 2.5.33 1.91-1.29 2.75-1.02 2.75-1.02.55 1.35.2 2.39.1 2.64.65.71 1.03 1.6 1.03 2.71 0 3.82-2.34 4.66-4.57 4.91.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2Z"/></svg>
            </a>
            <button class="social-icon copy-btn" data-copy="knived212@gmail.com" aria-label="Copy Email" title="Copy Email: knived212@gmail.com">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect width="20" height="16" x="2" y="4" rx="2"></path><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"></path></svg>
            </button>
            <button class="social-icon copy-btn" data-copy="+918590869839" aria-label="Copy Phone" title="Copy Phone: +91 8590869839">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>
            </button>
          </div>
        </div>

        <!-- Hero Graphic / Profile & Code Card -->
        <div class="hero-visual">
          <div class="hero-profile-wrapper">
            <!-- Profile Identity Bento Card -->
            <div class="profile-card bento-card">
              <div class="profile-image-container">
                <div class="profile-glow-ring"></div>
                <img src="assets/profile.jpg" alt="Nived Krishna S R" class="profile-img" />
                <div class="profile-status-badge">
                  <span class="status-dot"></span>
                  <span>Online</span>
                </div>
              </div>
              <div class="profile-card-details">
                <div class="profile-name">Nived Krishna S R</div>
                <div class="profile-tagline">Computer Science Engineer &bull; LPU</div>
                <div class="profile-chips">
                  <span class="p-chip">C++</span>
                  <span class="p-chip">Python</span>
                  <span class="p-chip">Kotlin</span>
                  <span class="p-chip">IoT</span>
                  <span class="p-chip">SQL</span>
                </div>
              </div>
            </div>

            <!-- Code Window Mockup -->
            <div class="code-window">
              <div class="code-header">
                <span class="dot red"></span>
                <span class="dot yellow"></span>
                <span class="dot green"></span>
                <span class="code-title">nived_profile.py</span>
              </div>
              <pre class="code-body"><code><span class="token-keyword">class</span> <span class="token-class">SoftwareEngineer</span>:
    <span class="token-keyword">def</span> <span class="token-function">__init__</span>(<span class="token-param">self</span>):
        <span class="token-param">self</span>.name = <span class="token-string">"Nived Krishna S R"</span>
        <span class="token-param">self</span>.education = <span class="token-string">"B.Tech CSE @ LPU (CGPA: 7.56)"</span>
        <span class="token-param">self</span>.languages = [<span class="token-string">"C++"</span>, <span class="token-string">"Python"</span>, <span class="token-string">"Kotlin"</span>, <span class="token-string">"SQL"</span>]

    <span class="token-keyword">def</span> <span class="token-function">build</span>(<span class="token-param">self</span>):
        <span class="token-keyword">return</span> <span class="token-string">"High-performance & intuitive software ⚡"</span></code></pre>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- ABOUT SECTION (BENTO GRID) -->
    <section class="section about-section" id="about">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">&lt; Bio & Background /&gt;</span>
          <h2 class="section-title">About Me</h2>
          <p class="section-subtitle">Bridging strong computational engineering with versatile software development.</p>
        </div>

        <div class="about-bento-grid">
          <div class="bento-card bento-about-main">
            <div class="bento-icon-box">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
            </div>
            <h3 class="bento-title">Academic & Technical Foundation</h3>
            <p class="bento-text">
              I am an undergraduate Computer Science and Engineering student at <strong>Lovely Professional University</strong> (CGPA: 7.56).
            </p>
            <p class="bento-text">
              I completed my schooling at <strong>GVHSS Madapally, Kozhikode, Kerala</strong>, achieving academic distinction with <strong>90.58%</strong> in 12th PCM and <strong>92.4%</strong> in 10th grade.
            </p>
          </div>

          <div class="bento-card bento-about-skills">
            <div class="bento-icon-box">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="16 18 22 12 16 6"></polyline><polyline points="8 6 2 12 8 18"></polyline></svg>
            </div>
            <h3 class="bento-title">Engineering Focus</h3>
            <p class="bento-text">
              Proficient in low-level and high-level programming across <strong>C++, Python, C, JavaScript, SQL, and Kotlin</strong>.
            </p>
            <p class="bento-text">
              Passionate about creating clean software architectures, embedded IoT security systems, and responsive user experiences.
            </p>
          </div>
        </div>

        <!-- Key Metrics Bento Row -->
        <div class="metrics-bento-grid">
          <div class="bento-card metric-bento-card">
            <div class="metric-number-wrap">
              <span class="metric-number" data-target="3">0</span><span class="metric-plus">+</span>
            </div>
            <span class="metric-label">Key Projects Delivered</span>
          </div>
          <div class="bento-card metric-bento-card">
            <div class="metric-number-wrap">
              <span class="metric-number" data-target="3">0</span>
            </div>
            <span class="metric-label">Verified Certifications</span>
          </div>
          <div class="bento-card metric-bento-card">
            <div class="metric-number-wrap">
              <span class="metric-number" data-target="91">0</span><span class="metric-plus">%</span>
            </div>
            <span class="metric-label">12th Grade PCM (90.58%)</span>
          </div>
          <div class="bento-card metric-bento-card">
            <div class="metric-number-wrap">
              <span class="metric-number" data-target="92">0</span><span class="metric-plus">%</span>
            </div>
            <span class="metric-label">10th Grade Score (92.4%)</span>
          </div>
        </div>
      </div>
    </section>

    <!-- SKILLS SECTION (BENTO MATRIX) -->
    <section class="section skills-section" id="skills">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">&lt; Capabilities /&gt;</span>
          <h2 class="section-title">Technical Skillset</h2>
          <p class="section-subtitle">Core programming languages, development tools, and engineering methodologies.</p>
        </div>

        <div class="skills-bento-grid">
          <!-- Programming Languages -->
          <div class="bento-card skills-col-langs">
            <div class="skill-category-header">
              <div class="bento-icon-box" style="margin-bottom: 0;">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="16 18 22 12 16 6"></polyline><polyline points="8 6 2 12 8 18"></polyline></svg>
              </div>
              <h3 class="bento-title" style="margin-bottom: 0;">Programming Languages</h3>
            </div>
            <div class="skill-pills-wrap">
              <div class="skill-pill"><span class="pill-dot"></span> C++</div>
              <div class="skill-pill"><span class="pill-dot"></span> Python</div>
              <div class="skill-pill"><span class="pill-dot"></span> C</div>
              <div class="skill-pill"><span class="pill-dot"></span> JavaScript</div>
              <div class="skill-pill"><span class="pill-dot"></span> SQL</div>
              <div class="skill-pill"><span class="pill-dot"></span> Kotlin</div>
              <div class="skill-pill"><span class="pill-dot"></span> HTML5 / CSS3</div>
            </div>
          </div>

          <!-- Tools & Platforms -->
          <div class="bento-card skills-col-tools">
            <div class="skill-category-header">
              <div class="bento-icon-box" style="margin-bottom: 0;">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"></path></svg>
              </div>
              <h3 class="bento-title" style="margin-bottom: 0;">Tools & Platforms</h3>
            </div>
            <div class="skill-pills-wrap">
              <div class="skill-pill"><span class="pill-dot"></span> MongoDB</div>
              <div class="skill-pill"><span class="pill-dot"></span> Android Studio</div>
              <div class="skill-pill"><span class="pill-dot"></span> VS Code</div>
              <div class="skill-pill"><span class="pill-dot"></span> PyCharm</div>
              <div class="skill-pill"><span class="pill-dot"></span> Git & GitHub</div>
            </div>
          </div>

          <!-- Professional & Soft Skills -->
          <div class="bento-card skills-col-soft">
            <div class="skill-category-header">
              <div class="bento-icon-box" style="margin-bottom: 0;">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="9" cy="7" r="4"></circle><path d="M23 21v-2a4 4 0 0 0-3-3.87"></path><path d="M16 3.13a4 4 0 0 1 0 7.75"></path></svg>
              </div>
              <h3 class="bento-title" style="margin-bottom: 0;">Soft Skills & Engineering Practices</h3>
            </div>
            <div class="skill-pills-wrap">
              <div class="skill-pill"><span class="pill-dot"></span> Problem-Solving</div>
              <div class="skill-pill"><span class="pill-dot"></span> Teamwork</div>
              <div class="skill-pill"><span class="pill-dot"></span> Project Management</div>
              <div class="skill-pill"><span class="pill-dot"></span> Adaptability</div>
              <div class="skill-pill"><span class="pill-dot"></span> Technical Communication</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- PROJECTS SECTION -->
    <section class="section projects-section" id="projects">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">&lt; Showcase /&gt;</span>
          <h2 class="section-title">Featured Projects</h2>
          <p class="section-subtitle">Real-world applications spanning embedded security, web productivity apps, and interactive tools.</p>
        </div>

        <!-- Project Filter Buttons -->
        <div class="project-filters">
          <button class="filter-btn active" data-filter="all">All Projects</button>
          <button class="filter-btn" data-filter="iot">IoT & Security</button>
          <button class="filter-btn" data-filter="web">Web & Productivity</button>
        </div>

        <div class="projects-grid">
          <!-- Project 1: IoT ATM Security System -->
          <article class="bento-card project-card" data-category="iot">
            <div class="project-card-header">
              <div class="project-tag-list">
                <span class="tag-badge">IoT</span>
                <span class="tag-badge">Embedded Systems</span>
              </div>
              <div class="bento-icon-box" style="width: 36px; height: 36px; margin-bottom: 0;">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect width="18" height="11" x="3" y="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>
              </div>
            </div>
            <div class="project-content">
              <h3 class="project-title">IoT-Based ATM Security System</h3>
              <p class="project-desc">
                An IoT-based security system developed to detect unauthorized ATM access and suspicious activity through real-time continuous monitoring.
              </p>
              <ul class="project-bullet-list">
                <li>Integrated sensors and connected hardware to enable automated, timely security alerts.</li>
                <li>Monitors physical access parameters to detect physical tampering in real time.</li>
                <li>Constructed an automated safety alert mechanism for rapid threat notification.</li>
              </ul>
            </div>
            <div class="project-footer">
              <div class="tech-stack-chips">
                <span>IoT</span>
                <span>Embedded Systems</span>
                <span>Hardware Sensors</span>
                <span>Automated Alerts</span>
              </div>
            </div>
          </article>

          <!-- Project 2: Taskify -->
          <article class="bento-card project-card" data-category="web">
            <div class="project-card-header">
              <div class="project-tag-list">
                <span class="tag-badge">HTML</span>
                <span class="tag-badge">CSS</span>
                <span class="tag-badge">JavaScript</span>
              </div>
              <div class="bento-icon-box" style="width: 36px; height: 36px; margin-bottom: 0;">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 20h9"></path><path d="M16.5 3.5a2.12 2.12 0 0 1 3 3L7 19l-4 1 1-4Z"></path></svg>
              </div>
            </div>
            <div class="project-content">
              <h3 class="project-title">Taskify – Task Management App</h3>
              <p class="project-desc">
                A productivity-focused web application designed to create, organise, prioritise, and track daily tasks with zero friction.
              </p>
              <ul class="project-bullet-list">
                <li>Designed an intuitive, responsive interface with interactive task-management features using JavaScript.</li>
                <li>Enabled streamlined task creation, priority setting, and structured daily progress monitoring.</li>
                <li>Implemented dynamic DOM manipulation for seamless task state transitions.</li>
              </ul>
            </div>
            <div class="project-footer">
              <div class="tech-stack-chips">
                <span>HTML5</span>
                <span>CSS3</span>
                <span>JavaScript</span>
                <span>Productivity UI</span>
              </div>
            </div>
          </article>

          <!-- Project 3: Pomodoro Timer -->
          <article class="bento-card project-card" data-category="web">
            <div class="project-card-header">
              <div class="project-tag-list">
                <span class="tag-badge">HTML</span>
                <span class="tag-badge">CSS</span>
                <span class="tag-badge">JavaScript</span>
              </div>
              <div class="bento-icon-box" style="width: 36px; height: 36px; margin-bottom: 0;">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"></circle><polyline points="12 6 12 12 16 14"></polyline></svg>
              </div>
            </div>
            <div class="project-content">
              <h3 class="project-title">Pomodoro Timer</h3>
              <p class="project-desc">
                A web-based Pomodoro timer engineered for structured, deep work sessions and scheduled recovery breaks.
              </p>
              <ul class="project-bullet-list">
                <li>Implemented interactive countdown functionality with a clean, distraction-free interface.</li>
                <li>Supports customizable intervals for focus sessions, short pauses, and long recovery breaks.</li>
                <li>Zero dependencies with accurate interval execution using vanilla JavaScript.</li>
              </ul>
            </div>
            <div class="project-footer">
              <div class="tech-stack-chips">
                <span>HTML5</span>
                <span>CSS3</span>
                <span>JavaScript</span>
                <span>Timer Engine</span>
              </div>
            </div>
          </article>
        </div>

        <!-- Interactive Live Widget Demonstration -->
        <div class="bento-card interactive-demo-wrapper">
          <div class="demo-header">
            <div class="demo-badge">
              <span class="live-indicator"></span> Live Interactive Engine
            </div>
            <h3 class="section-title" style="font-size: 1.75rem;">Test Nived's Pomodoro Engine Right Here</h3>
            <p class="section-subtitle" style="font-size: 0.95rem;">Experience the countdown functionality built with clean JavaScript.</p>
          </div>

          <div class="pomodoro-widget" id="pomodoroWidget">
            <div class="pomo-mode-tabs">
              <button class="pomo-tab active" data-mode="work" data-time="1500">Focus (25m)</button>
              <button class="pomo-tab" data-mode="short" data-time="300">Short Break (5m)</button>
              <button class="pomo-tab" data-mode="long" data-time="900">Long Break (15m)</button>
            </div>

            <div class="pomo-display">
              <div class="pomo-circle">
                <span id="pomoMinutes">25</span>:<span id="pomoSeconds">00</span>
              </div>
              <div class="pomo-status" id="pomoStatus">Stay focused on your current task 🎯</div>
            </div>

            <div class="pomo-controls">
              <button id="pomoStartBtn" class="btn btn-primary btn-sm">Start</button>
              <button id="pomoPauseBtn" class="btn btn-secondary btn-sm" disabled>Pause</button>
              <button id="pomoResetBtn" class="btn btn-outline btn-sm">Reset</button>
            </div>
          </div>
        </div>

      </div>
    </section>

    <!-- CERTIFICATIONS SECTION -->
    <section class="section certs-section" id="certifications">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">&lt; Accreditations /&gt;</span>
          <h2 class="section-title">Certificates</h2>
          <p class="section-subtitle">Verified programming and technical certifications.</p>
        </div>

        <div class="certs-grid">
          <!-- Cert 1: Python - Saylor Academy -->
          <div class="bento-card cert-card">
            <div class="cert-header">
              <div class="cert-badge-icon python-bg" style="background: linear-gradient(135deg, #3776ab, #ffd438);">
                <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2c2.76 0 5 2.24 5 5v2H9V7c0-2.76 2.24-5 5-5zm-5 7V7c0-3.87 3.13-7 7-7s7 3.13 7 7v2h1c1.1 0 2 .9 2 2v8c0 1.1-.9 2-2 2H6c-1.1 0-2-.9-2-2v-8c0-1.1.9-2 2-2h1z"/></svg>
              </div>
              <span class="cert-date">March 2026</span>
            </div>
            <h3 class="cert-name">Python (CS105)</h3>
            <p class="cert-issuer">Saylor Academy</p>
            <p class="cert-description">
              Core Python programming principles, algorithmic logic, data structures, and computer science fundamentals.
            </p>
            <div class="cert-footer">
              <span class="verified-badge">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"></polyline></svg> Certified (CS105)
              </span>
            </div>
          </div>

          <!-- Cert 2: C++ Programming - Saylor Academy -->
          <div class="bento-card cert-card">
            <div class="cert-header">
              <div class="cert-badge-icon cpp-bg" style="background: linear-gradient(135deg, #00599c, #004482);">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="16 18 22 12 16 6"></polyline><polyline points="8 6 2 12 8 18"></polyline></svg>
              </div>
              <span class="cert-date">Feb 2025</span>
            </div>
            <h3 class="cert-name">C++ Programming (CS107)</h3>
            <p class="cert-issuer">Saylor Academy</p>
            <p class="cert-description">
              C++ language mechanics, object-oriented software engineering, pointer management, and algorithmic problem-solving.
            </p>
            <div class="cert-footer">
              <span class="verified-badge">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"></polyline></svg> Certified (CS107)
              </span>
            </div>
          </div>

          <!-- Cert 3: JavaScript Basics - upGrad -->
          <div class="bento-card cert-card">
            <div class="cert-header">
              <div class="cert-badge-icon js-bg" style="background: linear-gradient(135deg, #f7df1e, #d4be00); color: #000;">
                <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2L2 7l10 5 10-5-10-5zm0 9l-10-5v9l10 5 10-5v-9l-10 5z"/></svg>
              </div>
              <span class="cert-date">May 2025</span>
            </div>
            <h3 class="cert-name">JavaScript Basics</h3>
            <p class="cert-issuer">upGrad</p>
            <p class="cert-description">
              Foundational modern JavaScript, dynamic DOM manipulation, interactive web behaviors, and event handling.
            </p>
            <div class="cert-footer">
              <span class="verified-badge">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"></polyline></svg> Certified
              </span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- EDUCATION SECTION -->
    <section class="section education-section" id="education">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">&lt; Academics /&gt;</span>
          <h2 class="section-title">Education</h2>
          <p class="section-subtitle">Academic dedication and rigorous computer science foundations.</p>
        </div>

        <div class="education-grid">
          <!-- College -->
          <div class="bento-card edu-card">
            <div class="edu-header">
              <div class="edu-icon">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 10v6M2 10l10-5 10 5-10 5z"></path><path d="M6 12v5c3 3 9 3 12 0v-5"></path></svg>
              </div>
              <span class="edu-period">Aug '25 – Present</span>
            </div>
            <h3 class="edu-degree">Bachelor of Technology (B.Tech)</h3>
            <h4 class="edu-institution">Lovely Professional University, Phagwara, Punjab</h4>
            <p class="edu-field">Computer Science and Engineering</p>
            <div class="edu-score-badge">
              <span class="score-label">CGPA</span>
              <span class="score-value">7.56</span>
            </div>
          </div>

          <!-- 12th Grade -->
          <div class="bento-card edu-card">
            <div class="edu-header">
              <div class="edu-icon">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 19.5v-15A2.5 2.5 0 0 1 6.5 2H20v20H6.5a2.5 2.5 0 0 1-2.5-2.5Z"></path><path d="M6 6h10"></path><path d="M6 10h10"></path></svg>
              </div>
              <span class="edu-period">Mar '24 – April '25</span>
            </div>
            <h3 class="edu-degree">Higher Secondary Education (12th Grade)</h3>
            <h4 class="edu-institution">GVHSS Madapally, Kozhikode, Kerala</h4>
            <p class="edu-field">Physics, Chemistry, Mathematics (PCM)</p>
            <div class="edu-score-badge">
              <span class="score-label">Percentage</span>
              <span class="score-value">90.58%</span>
            </div>
          </div>

          <!-- 10th Grade -->
          <div class="bento-card edu-card">
            <div class="edu-header">
              <div class="edu-icon">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 20h9"></path><path d="M16.5 3.5a2.12 2.12 0 0 1 3 3L7 19l-4 1 1-4Z"></path></svg>
              </div>
              <span class="edu-period">Mar '22 – April '23</span>
            </div>
            <h3 class="edu-degree">Secondary School Certificate (10th Grade)</h3>
            <h4 class="edu-institution">GVHSS Madapally, Kozhikode, Kerala</h4>
            <p class="edu-field">General Science & Mathematics</p>
            <div class="edu-score-badge">
              <span class="score-label">Percentage</span>
              <span class="score-value">92.4%</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- CONTACT SECTION -->
    <section class="section contact-section" id="contact">
      <div class="container">
        <div class="section-header">
          <span class="section-badge">&lt; Connect /&gt;</span>
          <h2 class="section-title">Let's Connect</h2>
          <p class="section-subtitle">Interested in collaborating on a project, hiring for a role, or discussing ideas? Reach out anytime!</p>
        </div>

        <div class="contact-grid">
          <!-- Contact Info Cards -->
          <div class="contact-info-col">
            <div class="bento-card contact-card">
              <div class="contact-item">
                <div class="contact-icon-box">
                  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect width="20" height="16" x="2" y="4" rx="2"></path><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"></path></svg>
                </div>
                <div class="contact-details">
                  <span class="contact-type">Email Address</span>
                  <a href="mailto:knived212@gmail.com" class="contact-link">knived212@gmail.com</a>
                </div>
                <button class="copy-action-btn copy-btn" data-copy="knived212@gmail.com" title="Copy email">
                  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect width="14" height="14" x="8" y="8" rx="2" ry="2"></rect><path d="M4 16c-1.1 0-2-.9-2-2V4c0-1.1.9-2 2-2h10c1.1 0 2 .9 2 2"></path></svg>
                </button>
              </div>

              <div class="contact-item">
                <div class="contact-icon-box">
                  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>
                </div>
                <div class="contact-details">
                  <span class="contact-type">Phone / WhatsApp</span>
                  <a href="tel:+918590869839" class="contact-link">+91 8590869839</a>
                </div>
                <button class="copy-action-btn copy-btn" data-copy="+918590869839" title="Copy phone number">
                  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect width="14" height="14" x="8" y="8" rx="2" ry="2"></rect><path d="M4 16c-1.1 0-2-.9-2-2V4c0-1.1.9-2 2-2h10c1.1 0 2 .9 2 2"></path></svg>
                </button>
              </div>

              <div class="contact-item">
                <div class="contact-icon-box">
                  <svg viewBox="0 0 24 24" fill="currentColor"><path d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.46 10.9v8.37H9.2V10.9H6.46M7.83 6.64a1.65 1.65 0 0 0-1.66 1.66 1.66 1.66 0 0 0 1.66 1.65 1.65 1.65 0 0 0 1.65-1.65c0-.92-.74-1.66-1.65-1.66Z"/></svg>
                </div>
                <div class="contact-details">
                  <span class="contact-type">LinkedIn Profile</span>
                  <a href="https://www.linkedin.com/in/nived-krishna-sr-b0583a377/" target="_blank" rel="noopener noreferrer" class="contact-link">linkedin.com/in/nived-krishna-sr</a>
                </div>
              </div>

              <div class="contact-item">
                <div class="contact-icon-box">
                  <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34-.46-1.16-1.11-1.47-1.11-1.47-.91-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.87 1.52 2.34 1.07 2.91.83.1-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.92 0-1.11.38-2 1.03-2.71-.1-.25-.45-1.29.1-2.64 0 0 .84-.27 2.75 1.02.79-.22 1.65-.33 2.5-.33.85 0 1.71.11 2.5.33 1.91-1.29 2.75-1.02 2.75-1.02.55 1.35.2 2.39.1 2.64.65.71 1.03 1.6 1.03 2.71 0 3.82-2.34 4.66-4.57 4.91.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2Z"/></svg>
                </div>
                <div class="contact-details">
                  <span class="contact-type">GitHub Profile</span>
                  <a href="https://github.com/knived212-bit" target="_blank" rel="noopener noreferrer" class="contact-link">github.com/knived212-bit</a>
                </div>
              </div>
            </div>
          </div>

          <!-- Interactive Message Form -->
          <div class="contact-form-col">
            <form id="contactForm" class="bento-card contact-form">
              <h3 class="bento-title">Send a Direct Message</h3>
              <div class="form-group">
                <label for="senderName">Your Name</label>
                <input type="text" id="senderName" class="form-control" placeholder="Jane Doe" required />
              </div>
              <div class="form-group">
                <label for="senderEmail">Your Email</label>
                <input type="email" id="senderEmail" class="form-control" placeholder="jane@example.com" required />
              </div>
              <div class="form-group">
                <label for="senderSubject">Subject</label>
                <input type="text" id="senderSubject" class="form-control" placeholder="Project collaboration / Opportunity" required />
              </div>
              <div class="form-group">
                <label for="senderMessage">Message</label>
                <textarea id="senderMessage" class="form-control" rows="4" placeholder="Hi Nived, I came across your portfolio..." required></textarea>
              </div>
              <button type="submit" class="btn btn-primary btn-block">
                <span>Send Message</span>
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" class="icon"><line x1="22" y1="2" x2="11" y2="13"></line><polygon points="22 2 15 22 11 13 2 9 22 2"></polygon></svg>
              </button>
            </form>
          </div>
        </div>
      </div>
    </section>
  </main>

  <!-- FOOTER -->
  <footer class="footer">
    <div class="container footer-container">
      <div class="footer-left">
        <a href="#hero" class="brand-logo">
          <span class="logo-symbol">&lt;</span><span class="logo-text">Nived Krishna S R</span><span class="logo-symbol">/&gt;</span>
        </a>
        <p class="footer-tagline">Crafting modern software, smart IoT security & clean web apps.</p>
      </div>

      <div class="footer-links">
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#certifications">Certifications</a>
        <a href="#education">Education</a>
      </div>

      <div class="footer-bottom">
        <p>© 2025–2026 Nived Krishna S R. All Rights Reserved.</p>
        <a href="#hero" class="back-to-top" aria-label="Back to top" title="Back to top">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m18 15-6-6-6 6"/></svg>
        </a>
      </div>
    </div>
  </footer>

  <!-- Scripts -->
  <script src="js/main.js"></script>
</body>
</html>
