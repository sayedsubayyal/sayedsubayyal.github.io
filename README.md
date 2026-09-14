<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sayed Muhammad Subayyal | Cybersecurity Researcher</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #0d1117;
            --text-color: #c9d1d9;
            --heading-color: #f0f6fc;
            --accent-blue: #58a6ff;
            --accent-green: #7ee787;
            --border-color: #30363d;
            --muted-color: #8b949e;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            font-family: 'Fira Code', 'Courier New', monospace;
            line-height: 1.6;
            font-size: 15px;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 3rem 1.5rem;
        }

        a {
            color: var(--accent-blue);
            text-decoration: none;
            transition: color 0.2s ease;
        }

        a:hover {
            text-decoration: underline;
            color: #79c0ff;
        }

        /* Terminal Prompt Styling */
        .prompt {
            color: var(--accent-green);
            font-size: 0.9rem;
            margin-bottom: 0.5rem;
        }

        .nav-hint {
            color: var(--muted-color);
            font-size: 0.9rem;
            margin-bottom: 2rem;
        }

        .highlight {
            color: var(--accent-blue);
            font-weight: 600;
        }

        /* Typography */
        h1 {
            color: var(--heading-color);
            font-size: 2.2rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            letter-spacing: -0.5px;
        }

        h2 {
            color: var(--heading-color);
            font-size: 1.3rem;
            font-weight: 500;
            margin-bottom: 1.5rem;
        }

        h3 {
            color: var(--heading-color);
            font-size: 1.1rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
        }

        h4 {
            color: var(--accent-blue);
            font-size: 0.95rem;
            font-weight: 500;
            margin-bottom: 0.5rem;
        }

        em {
            color: var(--accent-blue);
            font-style: normal;
            text-decoration: underline;
            text-decoration-color: var(--border-color);
            text-underline-offset: 4px;
        }

        /* Sections */
        section {
            margin-bottom: 4rem;
            padding-top: 1rem;
            border-top: 1px solid var(--border-color);
        }

        .section-title {
            color: var(--muted-color);
            font-size: 0.9rem;
            margin-bottom: 1.5rem;
            text-transform: lowercase;
        }

        .summary {
            margin-bottom: 1.5rem;
            max-width: 650px;
        }

        .links {
            display: flex;
            gap: 1.5rem;
            margin-top: 1.5rem;
            font-size: 0.95rem;
        }

        /* Profile Env Block */
        .profile-env {
            background: rgba(110, 118, 129, 0.1);
            border: 1px solid var(--border-color);
            border-radius: 6px;
            padding: 1.5rem;
            margin-top: 1.5rem;
        }

        .profile-env p {
            margin-bottom: 0.5rem;
        }

        .profile-env p:last-child {
            margin-bottom: 0;
        }

        .key {
            color: var(--accent-green);
            display: inline-block;
            width: 140px;
        }

        /* Projects */
        .project {
            margin-bottom: 2.5rem;
        }

        .project-meta {
            color: var(--muted-color);
            font-size: 0.85rem;
            margin-bottom: 0.5rem;
        }

        .project-role {
            color: var(--accent-blue);
            font-size: 0.9rem;
            margin-bottom: 1rem;
            font-weight: 500;
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1rem;
            list-style: none;
        }

        .tech-stack li {
            background: rgba(56, 139, 253, 0.15);
            color: var(--accent-blue);
            padding: 0.2rem 0.6rem;
            border-radius: 12px;
            font-size: 0.8rem;
        }

        /* Stack Grid */
        .stack-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
            margin-top: 1.5rem;
        }

        @media (min-width: 600px) {
            .stack-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        .stack-category {
            border-left: 2px solid var(--border-color);
            padding-left: 1rem;
        }

        /* Timeline */
        .timeline {
            margin-top: 1.5rem;
            border-left: 2px solid var(--border-color);
            padding-left: 1.5rem;
        }

        .timeline-item {
            margin-bottom: 2rem;
            position: relative;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -1.6rem;
            top: 0.4rem;
            width: 10px;
            height: 10px;
            background: var(--accent-green);
            border-radius: 50%;
            border: 2px solid var(--bg-color);
        }

        .date {
            color: var(--muted-color);
            font-size: 0.85rem;
            display: block;
            margin-bottom: 0.3rem;
        }

        /* Credentials */
        .credentials-list {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1rem;
            margin-top: 1.5rem;
        }

        @media (min-width: 600px) {
            .credentials-list {
                grid-template-columns: 1fr 1fr;
            }
        }

        .credential {
            background: rgba(110, 118, 129, 0.1);
            border: 1px solid var(--border-color);
            border-radius: 6px;
            padding: 1rem;
        }

        .badge {
            display: inline-block;
            background: rgba(126, 231, 135, 0.15);
            color: var(--accent-green);
            padding: 0.15rem 0.5rem;
            border-radius: 4px;
            font-size: 0.75rem;
            margin-bottom: 0.5rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        /* Contact */
        .contact-links p {
            margin-bottom: 0.8rem;
        }

        /* Typing animation */
        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }
        .cursor {
            display: inline-block;
            width: 8px;
            height: 15px;
            background-color: var(--accent-green);
            animation: blink 1s infinite;
            vertical-align: middle;
            margin-left: 2px;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- HERO SECTION -->
        <header>
            <p class="prompt">> sayed@security:~$ init --profile=cybersecurity<span class="cursor"></span></p>
            <p class="prompt">> ready</p>
            <br>
            <p class="nav-hint">› <span class="highlight">whoami</span> --verbose</p>
            
            <h1>Sayed Muhammad Subayyal</h1>
            <h2>Ethical Hacker // Web Pentester // Offensive Security Researcher</h2>
            
            <p class="summary">
                17-year-old cybersecurity researcher and founder of <strong>Sipar Security</strong> based in Peshawar, Pakistan. 
                I develop practical cybersecurity solutions, conduct security research, and build network monitoring tools using Python and Linux. 
                My work focuses on defensive security, vulnerability assessment, and making cybersecurity more accessible through open-source projects. 
                Notably recognized for responsibly reporting multiple security vulnerabilities, including a disclosure acknowledged by <strong>NASA</strong>.
            </p>
            
            <div class="links">
                <a href="https://github.com/sayedsubayyal" target="_blank">[ GitHub ]</a>
                <a href="https://www.linkedin.com/in/sayed-muhammad-subayyal" target="_blank">[ LinkedIn ]</a>
                <a href="mailto:sayedmuhammadsubayyal@gmail.com">[ Email ]</a>
            </div>
        </header>

        <!-- 01 // ABOUT -->
        <section id="about">
            <p class="section-title">01 // about</p>
            <h2>Security that <em>protects</em>, research that <em>matters</em></h2>
            <p>I work at the intersection of offensive security and open-source development — turning vulnerability research into practical, accessible tools for home users and small businesses.</p>
            <br>
            <p>My focus is on systems where <strong>security is proactive</strong>: in-depth testing of web, mobile, and cloud applications, providing actionable vulnerability reports with proof-of-concept, and building network monitoring tools that detect threats before they escalate.</p>
            
            <div class="profile-env">
                <p><span class="key">role</span> Ethical Hacker & Security Researcher</p>
                <p><span class="key">building_since</span> 2024 (Open-Source Security Tools)</p>
                <p><span class="key">education</span> Intermediate, Pre-Engineering — Islamia College Peshawar, 2024 → 2026</p>
                <p><span class="key">focus_areas</span> Network Security, Wireless Security, Penetration Testing, Python</p>
                <p><span class="key">based_in</span> Peshawar, Pakistan · Open to remote security research</p>
            </div>
        </section>

        <!-- 02 // SELECTED WORK -->
        <section id="work">
            <p class="section-title">02 // selected work</p>
            <h2>Three pillars, <em>one mission</em></h2>
            <p>Founding a security initiative, hunting bugs in the wild, and publishing academic research to advance the field.</p>
            <br>

            <div class="project">
                <p class="project-meta">[ project://sipar-security ] May 2026 - Present</p>
                <h3>Sipar Security</h3>
                <p class="project-role">Founder & Lead Developer</p>
                <p>Founded to develop accessible cybersecurity tools for home users and small businesses. Lead the design and development of open-source network security software, conduct cybersecurity research, and build practical tools focused on network monitoring, threat detection, and security awareness.</p>
                <ul class="tech-stack">
                    <li>Python</li>
                    <li>Linux / Kali Linux</li>
                    <li>Open-Source Tools</li>
                    <li>Network Monitoring</li>
                </ul>
            </div>

            <div class="project">
                <p class="project-meta">[ project://bug-bounty ] Sep 2025 - Present</p>
                <h3>Security Researcher / Bug Bounty Hunter</h3>
                <p class="project-role">HackerOne · Bugcrowd · Intigriti</p>
                <p>Engage in managed bug bounty and vulnerability disclosure programs across diverse industries. Conduct in-depth testing of web, mobile, and cloud applications. Focus areas include web applications, APIs, authentication flows, and authorization logic. <strong>Notably reported a vulnerability acknowledged by NASA.</strong></p>
                <ul class="tech-stack">
                    <li>Web Pentesting</li>
                    <li>API Security</li>
                    <li>Vulnerability Assessment</li>
                    <li>Responsible Disclosure</li>
                </ul>
            </div>

            <div class="project">
                <p class="project-meta">[ publication://research ] 2026</p>
                <h3>Simulating and Mitigating Rogue Access Point Attacks in Wi-Fi Networks</h3>
                <p class="project-role">Co-Author, Journal of Soft Computing and Artificial Intelligence</p>
                <p>Peer-reviewed research paper exploring the simulation and mitigation of rogue access point attacks in Wi-Fi networks utilizing open-source tools. Contributed to practical defensive strategies for wireless network security.</p>
                <ul class="tech-stack">
                    <li>Wireless Security</li>
                    <li>Open-Source Tools</li>
                    <li>Academic Research</li>
                </ul>
            </div>
        </section>

        <!-- 03 // STACK -->
        <section id="stack">
            <p class="section-title">03 // stack</p>
            <h2>What I <em>reach for</em></h2>
            <p>Grouped by domain — offensive operations first, then the tooling that makes it possible.</p>
            
            <div class="stack-grid">
                <div class="stack-category">
                    <h4>[ offensive_security ]</h4>
                    <p>Ethical Hacking, Penetration Testing, Vulnerability Assessment, Bug Bounty Hunting, Web & API Security</p>
                </div>
                <div class="stack-category">
                    <h4>[ network_security ]</h4>
                    <p>Wireless Security, Rogue AP Mitigation, Network Monitoring, Threat Detection, Security Risk Management</p>
                </div>
                <div class="stack-category">
                    <h4>[ languages_and_tools ]</h4>
                    <p>Python, Linux, Kali Linux, Bash, Open-Source Security Tools, Automation</p>
                </div>
                <div class="stack-category">
                    <h4>[ languages_spoken ]</h4>
                    <p>English (Full Professional), Urdu (Full Professional), Pashto (Professional Working)</p>
                </div>
            </div>
        </section>

        <!-- 04 // JOURNEY -->
        <section id="journey">
            <p class="section-title">04 // journey</p>
            <h2>Compounding <em>expertise</em></h2>
            <p>From foundational cybersecurity concepts to independent security research and open-source leadership.</p>

            <div class="timeline">
                <div class="timeline-item">
                    <span class="date">Sep 2025 - Present</span>
                    <h4>HackerOne & Bugcrowd</h4>
                    <p>Started participating in vulnerability disclosure programs, identifying and responsibly reporting security vulnerabilities in web apps and APIs.</p>
                </div>
                <div class="timeline-item">
                    <span class="date">Jan 2026 - Present</span>
                    <h4>Intigriti</h4>
                    <p>Expanded bug bounty operations, conducting in-depth testing of cloud and mobile applications and providing actionable mitigation recommendations.</p>
                </div>
                <div class="timeline-item">
                    <span class="date">May 2026 - Present</span>
                    <h4>Founded Sipar Security</h4>
                    <p>Launched an initiative to develop accessible, open-source cybersecurity tools for network monitoring and threat detection.</p>
                </div>
                <div class="timeline-item">
                    <span class="date">2026</span>
                    <h4>Published Academic Research</h4>
                    <p>Co-authored a peer-reviewed paper on mitigating rogue access point attacks in Wi-Fi networks using open-source tools.</p>
                </div>
                <div class="timeline-item">
                    <span class="date">Sep 2024 - Sep 2026</span>
                    <h4>Islamia College Peshawar</h4>
                    <p>Intermediate, Pre-Engineering. Building the mathematical and logical foundation for advanced cybersecurity research.</p>
                </div>
            </div>
        </section>

        <!-- 05 // CREDENTIALS -->
        <section id="credentials">
            <p class="section-title">05 // credentials</p>
            <h2>Certifications that <em>validate</em></h2>
            
            <div class="credentials-list">
                <div class="credential">
                    <span class="badge">Certification</span>
                    <h4>Ethical Hacker</h4>
                </div>
                <div class="credential">
                    <span class="badge">Certification</span>
                    <h4>Foundations of Cybersecurity</h4>
                </div>
                <div class="credential">
                    <span class="badge">Certification</span>
                    <h4>Automate Cybersecurity Tasks with Python</h4>
                </div>
                <div class="credential">
                    <span class="badge">Certification</span>
                    <h4>Sound the Alarm: Detection and Response</h4>
                </div>
                <div class="credential">
                    <span class="badge">Certification</span>
                    <h4>Play It Safe: Manage Security Risks</h4>
                </div>
                <div class="credential">
                    <span class="badge">Highlight</span>
                    <h4>NASA Acknowledged Disclosure</h4>
                    <p style="font-size: 0.85rem; margin-top: 0.5rem; color: var(--muted-color);">Responsibly reported and had a security vulnerability acknowledged by NASA.</p>
                </div>
            </div>
        </section>

        <!-- 06 // CONTACT -->
        <section id="contact">
            <p class="section-title">06 // contact</p>
            <h2>Let's secure something <em>together</em></h2>
            <p>Open to cybersecurity internships, freelance penetration testing, bug bounty collaborations, and conversations about open-source security tools.</p>
            <br>

            <div class="contact-links">
                <p><span class="key">email</span> <a href="mailto:sayedmuhammadsubayyal@gmail.com">sayedmuhammadsubayyal@gmail.com</a></p>
                <p><span class="key">phone</span> 03325765207</p>
                <p><span class="key">github</span> <a href="https://github.com/sayedsubayyal" target="_blank">github.com/sayedsubayyal ↗</a></p>
                <p><span class="key">linkedin</span> <a href="https://www.linkedin.com/in/sayed-muhammad-subayyal" target="_blank">linkedin.com/in/sayed-muhammad-subayyal ↗</a></p>
                <p><span class="key">location</span> Peshawar, Khyber Pakhtunkhwa, Pakistan</p>
            </div>
        </section>
        
        <footer style="text-align: center; color: var(--muted-color); font-size: 0.8rem; margin-top: 4rem; padding-top: 2rem; border-top: 1px solid var(--border-color);">
            <p>© 2026 Sayed Muhammad Subayyal. Built with vanilla HTML/CSS.</p>
        </footer>
    </div>
</body>
</html>
