
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#050505">
<title>Alok Kumar Gupta | Full Stack Developer</title>
<meta name="description" content="Alok Kumar Gupta - Full Stack Developer building modern, scalable digital experiences.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">

<style>
:root {
    --bg: #050505;
    --card: #0b0b0d;
    --border: #242329;
    --purple: #a855f7;
    --blue: #818cf8;
    --white: #f5f5f5;
    --muted: #85858e;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    background: var(--bg);
    color: var(--white);
    font-family: 'Inter', sans-serif;
    overflow-x: hidden;
}

a {
    color: inherit;
    text-decoration: none;
}

button {
    font: inherit;
}

#stars {
    position: fixed;
    inset: 0;
    z-index: -1;
    pointer-events: none;
}

.container {
    width: min(1150px, 92%);
    margin: auto;
}

/* NAVBAR */

nav {
    position: sticky;
    top: 12px;
    z-index: 100;
    width: min(1150px, 94%);
    margin: 12px auto 0;
    padding: 17px 25px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: rgba(10,10,12,.83);
    backdrop-filter: blur(18px);
    border: 1px solid var(--border);
    border-radius: 15px;
}

.logo {
    font-size: 23px;
    font-weight: 800;
    letter-spacing: -2px;
}

.logo span {
    color: var(--purple);
}

.nav-links {
    display: flex;
    gap: 30px;
    list-style: none;
}

.nav-links a {
    font-size: 12px;
    color: #b6b6bd;
    transition: .3s;
}

.nav-links a:hover {
    color: var(--purple);
}

.menu-btn {
    display: none;
    border: 0;
    color: white;
    background: transparent;
    font-size: 24px;
    cursor: pointer;
}

/* HERO */

.hero {
    min-height: 490px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 35px;
    align-items: center;
    padding: 65px 25px;
}

.eyebrow {
    display: inline-block;
    color: #c084fc;
    border: 1px solid #65338c;
    background: rgba(168,85,247,.09);
    padding: 7px 13px;
    border-radius: 30px;
    font-size: 11px;
    margin-bottom: 24px;
}

.hero h1 {
    font-size: clamp(38px, 5vw, 65px);
    line-height: 1.08;
    letter-spacing: -3px;
    margin-bottom: 20px;
}

.gradient {
    background: linear-gradient(100deg, #c084fc, #818cf8);
    -webkit-background-clip: text;
    color: transparent;
}

.hero p {
    color: var(--muted);
    font-size: 14px;
    line-height: 1.9;
    max-width: 470px;
}

.tech-pills {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin: 24px 0;
}

.tech-pills span {
    border: 1px solid var(--border);
    background: #111114;
    color: #c6c6cf;
    padding: 7px 11px;
    font-size: 10px;
    border-radius: 6px;
}

.buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
}

.btn {
    padding: 13px 20px;
    border-radius: 8px;
    font-size: 12px;
    font-weight: 600;
    transition: .3s;
    display: inline-block;
}

.btn-primary {
    background: linear-gradient(110deg, #9333ea, #6366f1);
    color: white;
    box-shadow: 0 0 25px #9333ea30;
}

.btn-secondary {
    border: 1px solid var(--border);
    background: #111114;
}

.btn:hover {
    transform: translateY(-4px);
    box-shadow: 0 0 25px #9333ea55;
}

/* TERMINAL */

.terminal {
    background: rgba(10,10,12,.95);
    border: 1px solid #34313d;
    border-radius: 13px;
    overflow: hidden;
    box-shadow: 0 20px 70px #000;
    animation: float 5s ease-in-out infinite;
}

.terminal-top {
    padding: 13px 16px;
    display: flex;
    align-items: center;
    gap: 7px;
    background: #17171b;
    border-bottom: 1px solid var(--border);
    font-family: monospace;
    font-size: 11px;
    color: #aaa;
}

.dot {
    height: 8px;
    width: 8px;
    border-radius: 50%;
}

.red { background: #ff5f57; }
.yellow { background: #febc2e; }
.green { background: #28c840; }

.terminal-body {
    padding: 25px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    line-height: 2.1;
    color: #b8b8c1;
}

.terminal-body .command { color: #c084fc; }
.terminal-body .value { color: #86efac; }

.cursor {
    display: inline-block;
    width: 7px;
    height: 14px;
    background: #a855f7;
    vertical-align: middle;
    animation: blink 1s infinite;
}

@keyframes blink { 50% { opacity: 0; } }
@keyframes float {
    50% { transform: translateY(-10px); }
}

/* SECTION */

section {
    padding: 35px 0;
}

.section-title {
    text-align: center;
    margin-bottom: 30px;
}

.section-title h2 {
    font-size: 23px;
    letter-spacing: -1px;
    margin-bottom: 9px;
}

.section-title p {
    color: var(--muted);
    font-size: 12px;
}

.grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 12px;
}

.card {
    background: linear-gradient(145deg, #101014, #09090b);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 22px;
    transition: .3s;
}

.card:hover {
    transform: translateY(-5px);
    border-color: #8850b9;
    box-shadow: 0 10px 35px #9333ea15;
}

.skill-icon {
    font-size: 25px;
    margin-bottom: 15px;
}

.card h3 {
    font-size: 13px;
    margin-bottom: 7px;
}

.card p {
    font-size: 11px;
    color: var(--muted);
    line-height: 1.7;
}

/* PROJECT */

.project-card {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 25px;
    align-items: center;
    padding: 30px;
}

.project-visual {
    min-height: 210px;
    border: 1px solid #383044;
    border-radius: 10px;
    background:
      radial-gradient(circle at 50% 40%, #7835aa45, transparent 60%),
      #0c0a11;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.project-visual .symbol {
    font-size: 55px;
    color: #c084fc;
}

.project-visual span {
    font-size: 12px;
    color: #aaa;
    margin-top: 10px;
}

.project-info h3 {
    font-size: 24px;
    margin-bottom: 15px;
}

.project-info p {
    font-size: 13px;
    line-height: 1.9;
    color: var(--muted);
}

.project-tags {
    display: flex;
    gap: 7px;
    flex-wrap: wrap;
    margin: 18px 0;
}

.project-tags span {
    font-size: 10px;
    color: #c084fc;
    background: #a855f715;
    border: 1px solid #a855f730;
    padding: 6px 10px;
    border-radius: 5px;
}

/* ABOUT */

.about-grid {
    display: grid;
    grid-template-columns: 1.3fr 1fr;
    gap: 15px;
}

.about-text {
    font-size: 13px;
    color: var(--muted);
    line-height: 2;
}

.stats {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 12px;
}

.stat {
    padding: 20px;
    background: #111114;
    border: 1px solid var(--border);
    border-radius: 10px;
}

.stat strong {
    font-size: 25px;
    color: #c084fc;
    display: block;
    margin-bottom: 6px;
}

.stat span {
    color: var(--muted);
    font-size: 11px;
}

/* LEARNING */

.learning {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
}

.learning span {
    padding: 12px 17px;
    border: 1px solid var(--border);
    background: #101014;
    border-radius: 8px;
    color: #c4c4ce;
    font-size: 12px;
}

/* CONTACT */

.contact-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 15px;
}

.contact-links {
    display: grid;
    gap: 12px;
}

.contact-item {
    padding: 16px;
    background: #111114;
    border: 1px solid var(--border);
    border-radius: 9px;
    color: #ccc;
    font-size: 12px;
    transition: .3s;
}

.contact-item:hover {
    border-color: var(--purple);
    color: white;
}

form {
    display: grid;
    gap: 12px;
}

input, textarea {
    background: #111114;
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 14px;
    color: white;
    outline: none;
    font-family: inherit;
    font-size: 12px;
    width: 100%;
}

input:focus, textarea:focus {
    border-color: var(--purple);
}

textarea {
    resize: vertical;
    min-height: 110px;
}

form button {
    border: 0;
    cursor: pointer;
}

/* FOOTER */

footer {
    margin-top: 40px;
    padding: 30px 0;
    border-top: 1px solid var(--border);
    text-align: center;
    color: var(--muted);
    font-size: 11px;
}

footer span {
    color: #c084fc;
}

/* REVEAL */

.reveal {
    opacity: 0;
    transform: translateY(25px);
    transition: .7s ease;
}

.reveal.visible {
    opacity: 1;
    transform: translateY(0);
}

/* RESPONSIVE */

@media(max-width: 800px) {
    .hero {
        grid-template-columns: 1fr;
        padding: 65px 10px;
    }

    .terminal {
        max-width: 600px;
        width: 100%;
    }

    .grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .project-card,
    .about-grid,
    .contact-grid {
        grid-template-columns: 1fr;
    }
}

@media(max-width: 600px) {
    nav {
        padding: 15px 18px;
    }

    .menu-btn {
        display: block;
    }

    .nav-links {
        display: none;
        position: absolute;
        top: 58px;
        left: 0;
        right: 0;
        flex-direction: column;
        gap: 20px;
        padding: 22px;
        background: #101014;
        border: 1px solid var(--border);
        border-radius: 12px;
    }

    .nav-links.active {
        display: flex;
    }

    .hero h1 {
        letter-spacing: -2px;
    }

    .grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .project-card {
        padding: 18px;
    }

    .terminal-body {
        font-size: 10px;
        padding: 17px;
    }
}
</style>
</head>

<body>

<canvas id="stars"></canvas>

<!-- NAVIGATION -->

<nav>
    <a href="#" class="logo">ALOK<span>.</span></a>

    <button class="menu-btn" id="menuBtn" aria-label="Toggle navigation">☰</button>

    <ul class="nav-links" id="navLinks">
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#certifications">Certifications</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<main class="container">

<!-- HERO -->

<div class="hero">

    <div class="hero-content reveal">

        <span class="eyebrow">● FULL STACK DEVELOPER</span>

        <h1>
            Hi, I'm <br>
            <span class="gradient">Alok Kumar Gupta</span>
        </h1>

        <p>
            I architect and build modern web applications,
            scalable backend systems and meaningful digital
            experiences. Passionate about turning ideas into reality.
        </p>

        <div class="tech-pills">
            <span>JavaScript</span>
            <span>TypeScript</span>
            <span>React</span>
            <span>Node.js</span>
            <span>MongoDB</span>
            <span>PostgreSQL</span>
        </div>

        <div class="buttons">
            <a href="#contact" class="btn btn-primary">Let's work together ↗</a>
            <a href="#projects" class="btn btn-secondary">View my work →</a>
        </div>

    </div>

    <!-- TERMINAL -->

    <div class="terminal reveal">

        <div class="terminal-top">
            <span class="dot red"></span>
            <span class="dot yellow"></span>
            <span class="dot green"></span>
            <span style="margin-left:10px">alok@developer:~</span>
        </div>

        <div class="terminal-body">
            <div><span class="command">$ whoami</span></div>
            <div class="value">FullStackDeveloper</div>
            <br>

            <div><span class="command">$ ls skills/</span></div>
            <div>▸ frontend_development</div>
            <div>▸ backend_engineering</div>
            <div>▸ database_management</div>
            <div>▸ cloud_and_devops</div>
            <div>▸ problem_solving</div>
            <br>

            <div><span class="command">$ cat currently_building.txt</span></div>
            <div class="value">ShramSetu</div>
            <br>

            <div><span class="command">$ echo $MINDSET</span></div>
            <div class="value">Build. Learn. Improve.</div>
            <br>

            <div><span class="command">$ </span><span class="cursor"></span></div>
        </div>

    </div>

</div>

<!-- SKILLS -->

<section id="skills" class="reveal">

    <div class="section-title">
        <h2>Tech Stack & <span class="gradient">Skills</span></h2>
        <p>Technologies I use to bring ideas to life.</p>
    </div>

    <div class="grid">

        <div class="card">
            <div class="skill-icon">🌐</div>
            <h3>Frontend</h3>
            <p>HTML, CSS, JavaScript, TypeScript, React, Tailwind CSS, Three.js</p>
        </div>

        <div class="card">
            <div class="skill-icon">⚙️</div>
            <h3>Backend</h3>
            <p>Node.js, Express.js, REST APIs and server-side development</p>
        </div>

        <div class="card">
            <div class="skill-icon">🗄️</div>
            <h3>Databases</h3>
            <p>MongoDB, PostgreSQL, MySQL and Prisma</p>
        </div>

        <div class="card">
            <div class="skill-icon">🛠️</div>
            <h3>Tools</h3>
            <p>Git, GitHub, Figma, C, C++ and development tools</p>
        </div>

    </div>

</section>

<!-- PROJECTS -->

<section id="projects" class="reveal">

    <div class="section-title">
        <h2>Featured <span class="gradient">Project</span></h2>
        <p>Some things I'm building and working on.</p>
    </div>

    <div class="card project-card">

        <div class="project-visual">
            <div class="symbol">✳</div>
            <span>SHRAMSETU</span>
        </div>

        <div class="project-info">

            <span class="eyebrow">CURRENTLY BUILDING</span>

            <h3>ShramSetu</h3>

            <p>
                A project focused on building a meaningful
                digital experience. Explore the live platform
                to discover its features and functionality.
            </p>

            <div class="project-tags">
                <span>Full Stack</span>
                <span>Web Development</span>
                <span>Engineering</span>
            </div>

            <a href="https://shramsetu.onrender.com"
               target="_blank"
               rel="noopener noreferrer"
               class="btn btn-primary">
               Explore Project ↗
            </a>

        </div>

    </div>

</section>

<!-- ABOUT -->

<section id="about" class="reveal">

    <div class="section-title">
        <h2>About <span class="gradient">Me</span></h2>
        <p>A little more about the developer behind the code.</p>
    </div>

    <div class="about-grid">

        <div class="card">
            <h3 style="margin-bottom:15px">Hello, World! 👋</h3>

            <p class="about-text">
                I'm Alok Kumar Gupta, a Full Stack Developer from India.
                I enjoy designing and developing modern web applications
                with clean interfaces and reliable backend architecture.

                <br><br>

                I love exploring new technologies, solving problems
                and continuously improving my development skills.

                <br><br>

                Currently, I'm working on ShramSetu and exploring
                cloud computing and DevOps technologies.
            </p>
        </div>

        <div class="stats">

            <div class="stat">
                <strong>01</strong>
                <span>Current featured project</span>
            </div>

            <div class="stat">
                <strong>∞</strong>
                <span>Ideas to explore</span>
            </div>

            <div class="stat">
                <strong>15+</strong>
                <span>Technologies and tools</span>
            </div>

            <div class="stat">
                <strong>24/7</strong>
                <span>Curiosity to learn</span>
            </div>

        </div>

    </div>

</section>

<!-- LEARNING -->

<section class="reveal">

    <div class="section-title">
        <h2>Currently <span class="gradient">Exploring</span></h2>
        <p>Always learning. Always evolving.</p>
    </div>

    <div class="card">
        <div class="learning">
            <span>🐳 Docker</span>
            <span>☁️ AWS</span>
            <span>☸️ Kubernetes</span>
            <span>🌐 Nginx</span>
        </div>
    </div>

</section>

<!-- CERTIFICATIONS -->

<section id="certifications" class="reveal">

    <div class="section-title">
        <h2>Certifications & <span class="gradient">Achievements</span></h2>
        <p>Learning is a continuous journey.</p>
    </div>

    <div class="card" style="text-align:center">
        <div class="skill-icon">🏆</div>
        <h3>More coming soon</h3>
        <p>
            Certifications and achievements will be showcased here.
        </p>
    </div>

</section>

<!-- CONTACT -->

<section id="contact" class="reveal">

    <div class="section-title">
        <h2>Let's <span class="gradient">Connect</span></h2>
        <p>Have an idea or opportunity? Let's make it happen.</p>
    </div>

    <div class="contact-grid">

        <div class="card contact-links">

            <a class="contact-item"
               href="mailto:trooooperr@gmail.com">
                ✉️ &nbsp; Email: trooooperr@gmail.com
            </a>

            <a class="contact-item"
               href="https://linkedin.com/in/trooperr"
               target="_blank">
                💼 &nbsp; LinkedIn
            </a>

            <a class="contact-item"
               href="https://twitter.com/trooooperr"
               target="_blank">
                𝕏 &nbsp; Twitter / X
            </a>

            <a class="contact-item"
               href="https://github.com/trooooperr"
               target="_blank">
                🐙 &nbsp; GitHub
            </a>

            <a class="contact-item"
               href="https://www.leetcode.com/trooperr"
               target="_blank">
                💻 &nbsp; LeetCode
            </a>

            <a class="contact-item"
               href="https://www.codechef.com/users/trooperr"
               target="_blank">
                👨‍🍳 &nbsp; CodeChef
            </a>

        </div>

        <div class="card">

            <form id="contactForm">

                <input type="text"
                       id="name"
                       placeholder="Your name"
                       required>

                <input type="email"
                       id="email"
                       placeholder="Your email"
                       required>

                <textarea id="message"
                          placeholder="Tell me about your idea..."
                          required></textarea>

                <button class="btn btn-primary" type="submit">
                    Send Message ↗
                </button>

            </form>

        </div>

    </div>

</section>

</main>

<!-- FOOTER -->

<footer>
    <div class="container">
        Designed & Built with <span>♥</span> by Alok Kumar Gupta
        <br><br>
        © <span id="year"></span> Alok Kumar Gupta. All rights reserved.
    </div>
</footer>

<script>

// MOBILE NAVIGATION

const menuBtn = document.getElementById("menuBtn");
const navLinks = document.getElementById("navLinks");

menuBtn.addEventListener("click", () => {
    navLinks.classList.toggle("active");
    menuBtn.textContent =
        navLinks.classList.contains("active") ? "✕" : "☰";
});

document.querySelectorAll(".nav-links a").forEach(link => {
    link.addEventListener("click", () => {
        navLinks.classList.remove("active");
        menuBtn.textContent = "☰";
    });
});

// CURRENT YEAR

document.getElementById("year").textContent =
    new Date().getFullYear();

// SCROLL REVEAL ANIMATION

const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add("visible");
            observer.unobserve(entry.target);
        }
    });
}, { threshold: 0.12 });

document.querySelectorAll(".reveal").forEach(element => {
    observer.observe(element);
});

// ANIMATED STAR BACKGROUND

const canvas = document.getElementById("stars");
const ctx = canvas.getContext("2d");

let stars = [];

function resizeCanvas() {
    const dpr = Math.min(window.devicePixelRatio || 1, 2);

    canvas.width = window.innerWidth * dpr;
    canvas.height = window.innerHeight * dpr;

    canvas.style.width = window.innerWidth + "px";
    canvas.style.height = window.innerHeight + "px";

    ctx.setTransform(dpr, 0, 0, dpr, 0, 0);

    stars = Array.from({length: 120}, () => ({
        x: Math.random() * window.innerWidth,
        y: Math.random() * window.innerHeight,
        size: Math.random() * 1.5,
        speed: Math.random() * 0.25 + 0.05,
        opacity: Math.random()
    }));
}

function animateStars() {
    ctx.clearRect(0, 0, window.innerWidth, window.innerHeight);

    stars.forEach(star => {
        star.y -= star.speed;

        if (star.y < 0) {
            star.y = window.innerHeight;
            star.x = Math.random() * window.innerWidth;
        }

        ctx.beginPath();
        ctx.arc(star.x, star.y, star.size, 0, Math.PI * 2);
        ctx.fillStyle = `rgba(210,190,255,${star.opacity})`;
        ctx.fill();
    });

    requestAnimationFrame(animateStars);
}

window.addEventListener("resize", resizeCanvas);

resizeCanvas();
animateStars();

// CONTACT FORM

document.getElementById("contactForm")
    .addEventListener("submit", function(e) {

        e.preventDefault();

        const name = document.getElementById("name").value;
        const email = document.getElementById("email").value;
        const message = document.getElementById("message").value;

        const subject = encodeURIComponent(
            "Portfolio Contact from " + name
        );

        const body = encodeURIComponent(
            "Name: " + name +
            "\nEmail: " + email +
            "\n\nMessage:\n" + message
        );

        window.location.href =
            `mailto:trooooperr@gmail.com?subject=${subject}&body=${body}`;
    });

</script>

</body>
</html>
