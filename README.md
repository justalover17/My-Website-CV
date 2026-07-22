<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Indra Bahadur Thakuri | Portfolio</title>

    <!-- Elegant Luxury Serif & Premium Clean Sans Serif Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">

    <style>
        :root {
            --rolex-green: #006039;
            --rolex-gold: #c5a059;
            --rolex-gold-hover: #e0b96f;
            --dark-charcoal: #0b0f17;
            --card-dark: #121824;
            --pure-white: #ffffff;
            --off-white: #f4f6f9;
            --border-color-dark: rgba(197, 160, 89, 0.15);
            --border-color-light: #dddddd;
            
            --font-serif: 'Cinzel', serif;
            --font-sans: 'Montserrat', sans-serif;
            --transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: var(--font-sans);
        }

        html {
            scroll-behavior: smooth;
        }

        /* --- Dark Mode (Default) --- */
        body {
            background: var(--dark-charcoal);
            color: var(--pure-white);
            overflow-x: hidden;
            line-height: 1.7;
        }

        nav {
            position: fixed;
            width: 100%;
            padding: 20px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(11, 15, 23, 0.8);
            backdrop-filter: blur(15px);
            border-bottom: 1px solid var(--border-color-dark);
            z-index: 1000;
        }

        .logo {
            font-family: var(--font-serif);
            font-size: 26px;
            font-weight: 700;
            color: var(--rolex-gold);
            letter-spacing: 2px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 35px;
        }

        nav ul li a {
            color: var(--pure-white);
            text-decoration: none;
            transition: var(--transition);
            font-weight: 500;
            font-size: 0.9rem;
            letter-spacing: 1px;
            text-transform: uppercase;
        }

        nav ul li a:hover {
            color: var(--rolex-gold);
        }

        .theme-btn {
            cursor: pointer;
            border: 1px solid var(--rolex-gold);
            background: transparent;
            color: var(--rolex-gold);
            width: 45px;
            height: 45px;
            border-radius: 50%;
            font-size: 18px;
            transition: var(--transition);
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .theme-btn:hover {
            background: var(--rolex-gold);
            color: var(--dark-charcoal);
        }

        /* --- Luxury Hero Section --- */
        .hero {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 150px 20px 100px 20px;
            background: 
                radial-gradient(circle at top left, rgba(0, 96, 57, 0.2), transparent),
                radial-gradient(circle at bottom right, rgba(197, 160, 89, 0.15), transparent),
                var(--dark-charcoal);
        }

        .brand-crown {
            font-size: 2.5rem;
            color: var(--rolex-gold);
            margin-bottom: 10px;
            display: block;
        }

        .hero h1 {
            font-family: var(--font-serif);
            font-size: 4rem;
            font-weight: 400;
            letter-spacing: 4px;
            margin-bottom: 15px;
            color: var(--pure-white);
        }

        .hero h2 {
            font-size: 1.8rem;
            font-weight: 400;
            color: var(--rolex-gold);
            margin-bottom: 25px;
            letter-spacing: 2px;
            text-transform: uppercase;
            min-height: 40px;
        }

        .hero p {
            max-width: 800px;
            margin: auto;
            line-height: 1.9;
            color: #b0b7c3;
            font-size: 1.05rem;
            font-weight: 300;
        }

        .buttons {
            margin-top: 40px;
        }

        .btn {
            display: inline-block;
            margin: 10px;
            padding: 15px 35px;
            text-transform: uppercase;
            font-size: 0.8rem;
            letter-spacing: 2px;
            text-decoration: none;
            transition: var(--transition);
            font-weight: 600;
        }

        .btn-primary {
            background: var(--rolex-green);
            color: var(--pure-white);
            border: 1px solid var(--rolex-green);
        }

        .btn-primary:hover {
            background: transparent;
            border-color: var(--rolex-gold);
            color: var(--rolex-gold);
            transform: translateY(-3px);
        }

        .btn-secondary {
            border: 1px solid var(--rolex-gold);
            color: var(--rolex-gold);
            background: transparent;
        }

        .btn-secondary:hover {
            background: var(--rolex-gold);
            color: var(--dark-charcoal);
            transform: translateY(-3px);
        }

        /* --- Global Structural Layouts --- */
        section {
            padding: 100px 10%;
        }

        .title {
            text-align: center;
            font-family: var(--font-serif);
            font-size: 2.5rem;
            font-weight: 400;
            letter-spacing: 3px;
            margin-bottom: 60px;
            text-transform: uppercase;
            position: relative;
        }

        .title::after {
            content: '';
            display: block;
            width: 50px;
            height: 2px;
            background: var(--rolex-gold);
            margin: 15px auto 0 auto;
        }

        .glass {
            background: var(--card-dark);
            padding: 45px;
            border-radius: 4px;
            border: 1px solid var(--border-color-dark);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
            transition: var(--transition);
        }

        .glass:hover {
            border-color: var(--rolex-gold);
        }

        /* --- About Section --- */
        .about {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 60px;
            align-items: center;
        }

        .profile {
            width: 220px;
            height: 220px;
            margin: auto;
            border-radius: 50%;
            background: transparent;
            border: 2px solid var(--rolex-gold);
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 70px;
            color: var(--rolex-gold);
            box-shadow: inset 0 0 20px rgba(197, 160, 89, 0.2);
        }

        .about p {
            line-height: 2;
            font-size: 1.05rem;
            color: #b0b7c3;
            font-weight: 300;
        }

        .about strong {
            color: var(--rolex-gold);
            font-weight: 600;
        }

        /* --- Grid & Cards Styling --- */
        .grid-layout {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
        }

        .card-box {
            background: var(--card-dark);
            padding: 35px;
            border-radius: 4px;
            border: 1px solid var(--border-color-dark);
            transition: var(--transition);
        }

        .card-box:hover {
            transform: translateY(-5px);
            border-color: var(--rolex-gold);
            background: linear-gradient(to bottom, var(--card-dark), rgba(0, 96, 57, 0.1));
        }

        .card-box h3 {
            font-family: var(--font-serif);
            font-size: 1.3rem;
            font-weight: 500;
            letter-spacing: 1px;
            margin-bottom: 20px;
            color: var(--pure-white);
        }

        .card-box p {
            color: #b0b7c3;
            font-size: 0.95rem;
            font-weight: 300;
            margin-bottom: 15px;
        }

        .card-box ul {
            list-style: none;
            margin-bottom: 20px;
        }

        .card-box ul li {
            font-size: 0.9rem;
            color: #b0b7c3;
            margin-bottom: 8px;
            font-weight: 300;
        }

        .card-box ul li i {
            color: var(--rolex-gold);
            margin-right: 8px;
            font-size: 0.85rem;
        }

        .tech-tag-title {
            display: block;
            font-size: 0.75rem;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            color: var(--rolex-gold);
            font-weight: 600;
            margin-top: 15px;
            margin-bottom: 5px;
        }

        .tech-tag-values {
            font-size: 0.85rem;
            color: var(--pure-white);
            font-weight: 400;
        }

        /* --- Executive Timelines & Custom Progress Bars --- */
        .skill-item {
            margin-bottom: 25px;
        }

        .skill-info {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
        }

        .skill-info h3 {
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            font-weight: 500;
        }

        .skill-info span {
            color: var(--rolex-gold);
            font-size: 0.9rem;
            font-weight: 600;
        }

        .bar {
            width: 100%;
            height: 4px;
            background: rgba(255, 255, 255, 0.08);
            border-radius: 2px;
        }

        .progress {
            height: 100%;
            background: var(--rolex-gold);
            border-radius: 2px;
        }

        /* --- Institutional Block --- */
        .edu-wrapper {
            display: flex;
            flex-direction: column;
            gap: 35px;
        }

        .edu-block {
            padding-left: 25px;
            border-left: 2px solid var(--rolex-gold);
            position: relative;
        }

        .edu-block::after {
            content: '';
            position: absolute;
            left: -6px;
            top: 6px;
            width: 10px;
            height: 10px;
            background: var(--rolex-green);
            border: 2px solid var(--rolex-gold);
            border-radius: 50%;
        }

        .edu-block h3 {
            font-family: var(--font-serif);
            font-size: 1.4rem;
            font-weight: 400;
            letter-spacing: 1px;
            color: var(--pure-white);
        }

        .edu-meta {
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            color: var(--rolex-gold);
            font-weight: 600;
            margin: 5px 0 12px 0;
        }

        .edu-separator {
            border: 0;
            height: 1px;
            background: var(--border-color-dark);
            margin: 10px 0;
        }

        /* --- Corporate Styled Contact Strip --- */
        .contact-details {
            display: flex;
            flex-direction: column;
            gap: 20px;
            max-width: 500px;
            margin: 0 auto 40px auto;
        }

        .contact-row-item {
            display: flex;
            align-items: center;
            gap: 20px;
            font-size: 1.05rem;
            color: #b0b7c3;
            font-weight: 300;
        }

        .contact-row-item i {
            color: var(--rolex-gold);
            font-size: 1.2rem;
            width: 25px;
            text-align: center;
        }

        .center-btn-box {
            text-align: center;
        }

        /* --- Footer Layout --- */
        footer {
            padding: 60px 20px;
            text-align: center;
            background: #06090f;
            border-top: 1px solid var(--border-color-dark);
        }

        footer h2 {
            font-family: var(--font-serif);
            font-size: 1.8rem;
            font-weight: 400;
            letter-spacing: 3px;
            color: var(--rolex-gold);
            margin-bottom: 15px;
        }

        footer p {
            font-size: 0.85rem;
            color: #666;
            letter-spacing: 1px;
            text-transform: uppercase;
        }

        /* --- LIGHT MODE ADJUSTMENTS --- */
        body.light {
            background: var(--off-white);
            color: #222222;
        }

        body.light nav {
            background: rgba(255, 255, 255, 0.9);
            border-bottom: 1px solid var(--border-color-light);
        }

        body.light nav ul li a {
            color: #222222;
        }

        body.light nav ul li a:hover {
            color: var(--rolex-green);
        }

        body.light .hero {
            background: 
                radial-gradient(circle at top left, rgba(0, 96, 57, 0.08), transparent),
                radial-gradient(circle at bottom right, rgba(197, 160, 89, 0.08), transparent),
                var(--off-white);
        }

        body.light .hero h1 {
            color: #111111;
        }

        body.light .hero p {
            color: #555555;
        }

        body.light .title {
            color: #111111;
        }

        body.light .glass, 
        body.light .card-box {
            background: var(--pure-white);
            border-color: var(--border-color-light);
            box-shadow: 0 15px 35px rgba(0,0,0,0.05);
        }

        body.light .card-box:hover {
            border-color: var(--rolex-green);
            background: linear-gradient(to bottom, var(--pure-white), rgba(0, 96, 57, 0.03));
        }

        body.light .card-box h3,
        body.light .edu-block h3 {
            color: #111111;
        }

        body.light .about p,
        body.light .card-box p,
        body.light .card-box ul li,
        body.light .contact-row-item {
            color: #444444;
        }

        body.light .bar {
            background: rgba(0, 0, 0, 0.08);
        }

        body.light .progress {
            background: var(--rolex-green);
        }

        body.light .edu-block {
            border-left-color: var(--rolex-green);
        }

        body.light footer {
            background: #eef1f6;
            border-top: 1px solid var(--border-color-light);
        }   

        /* --- Responsive Viewports --- */
        @media(max-width:900px){
            nav { padding: 15px 5%; }
            nav ul { display: none; }
            .hero h1 { font-size: 2.6rem; }
            .hero h2 { font-size: 1.3rem; }
            .about { grid-template-columns: 1fr; gap: 40px; }
            section { padding: 60px 5%; }
        }
    </style>
</head>

<body>

    <!-- EXECUTIVE TOP FIXED HEADER NAVIGATION -->
    <nav>
        <div class="logo">INDRA.</div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
        <button class="theme-btn" onclick="toggleTheme()" aria-label="Toggle Interface Theme">
            <i class="fa-solid fa-moon"></i>
        </button>
    </nav>

    <!-- LUXURY RADIAL HERO PLATFORM -->
    <section class="hero" id="home">
        <div>
            <span class="brand-crown">👑</span>
            <h1>INDRA BAHADUR THAKURI</h1>
            <h2 id="typing"></h2>
            <p>
                I am a Bachelor of Information Technology (BIT) student at Informatics College Pokhara with a strong interest in Full-Stack Web Development and Software Engineering. I enjoy building modern web applications using Java, JSP, Servlets, MySQL, HTML, CSS, JavaScript and Bootstrap. I am passionate about learning new technologies and solving real-world problems through software.
            </p>
            <div class="buttons">
                <a href="#" class="btn btn-primary">
                    <i class="fa-solid fa-download"></i> Download CV
                </a>
                <a href="#projects" class="btn btn-secondary">
                    View Projects
                </a>
            </div>
        </div>
    </section>

    <!-- EXECUTIVE BIOGRAPHY SECTION -->
    <section id="about">
        <h2 class="title">About Me</h2>
        <div class="about glass">
            <div class="profile">
                <i class="fa-solid fa-user"></i>
            </div>
            <div>
                <p>
                    Hello! I'm <strong>Indra Bahadur Thakuri</strong>, a BIT student from Nepal who enjoys creating clean, responsive, and user-friendly web applications. Throughout my studies, I have worked on Java desktop applications, JSP & Servlet web systems, database management, and IoT projects.
                    <br><br>
                    My goal is to become a professional Full Stack Developer while continuously improving my programming, problem-solving, and teamwork skills. I enjoy learning new technologies and building software that solves practical problems.
                </p>
            </div>
        </div>
    </section>

    <!-- METRIC TECHNICAL SKILLS SCATTER GRID -->
    <section id="skills">
        <h2 class="title">Technical Skills</h2>
        <div class="grid-layout">
            <div class="card-box skill-item">
                <div class="skill-info">
                    <h3>Java</h3>
                    <span>90%</span>
                </div>
                <div class="bar"><div class="progress" style="width:90%"></div></div>
            </div>
            <div class="card-box skill-item">
                <div class="skill-info">
                    <h3>HTML & CSS</h3>
                    <span>95%</span>
                </div>
                <div class="bar"><div class="progress" style="width:95%"></div></div>
            </div>
            <div class="card-box skill-item">
                <div class="skill-info">
                    <h3>JavaScript</h3>
                    <span>80%</span>
                </div>
                <div class="bar"><div class="progress" style="width:80%"></div></div>
            </div>
            <div class="card-box skill-item">
                <div class="skill-info">
                    <h3>JSP & Servlets</h3>
                    <span>88%</span>
                </div>
                <div class="bar"><div class="progress" style="width:88%"></div></div>
            </div>
            <div class="card-box skill-item">
                <div class="skill-info">
                    <h3>MySQL</h3>
                    <span>85%</span>
                </div>
                <div class="bar"><div class="progress" style="width:85%"></div></div>
            </div>
            <div class="card-box skill-item">
                <div class="skill-info">
                    <h3>Git & GitHub</h3>
                    <span>75%</span>
                </div>
                <div class="bar"><div class="progress" style="width:75%"></div></div>
            </div>
        </div>
    </section>

    <!-- ARCHITECTURAL PROJECT SHOWCASE -->
    <section id="projects">
        <h2 class="title">My Projects</h2>
        <div class="grid-layout">
            
            <div class="card-box">
                <h3>🍽 RIDKKS Eats</h3>
                <p>A full-stack online food ordering system developed using Java, JSP, Servlets, JDBC and MySQL.</p>
                <ul>
                    <li><i class="fa-solid fa-check"></i> User Login & Registration</li>
                    <li><i class="fa-solid fa-check"></i> Shopping Cart</li>
                    <li><i class="fa-solid fa-check"></i> Order Management</li>
                    <li><i class="fa-solid fa-check"></i> Admin Dashboard</li>
                    <li><i class="fa-solid fa-check"></i> Category Management</li>
                </ul>
                <span class="tech-tag-title">Technology</span>
                <span class="tech-tag-values">Java • JSP • Servlets • MySQL • HTML • CSS</span>
            </div>

            <div class="card-box">
                <h3>💼 Student Internship Management System</h3>
                <p>A web application that connects students, companies and administrators to manage internships efficiently.</p>
                <ul>
                    <li><i class="fa-solid fa-check"></i> Student Dashboard</li>
                    <li><i class="fa-solid fa-check"></i> Company Dashboard</li>
                    <li><i class="fa-solid fa-check"></i> Admin Panel</li>
                    <li><i class="fa-solid fa-check"></i> Internship Applications</li>
                    <li><i class="fa-solid fa-check"></i> Report Tracking</li>
                </ul>
                <span class="tech-tag-title">Technology</span>
                <span class="tech-tag-values">Java • JSP • Servlets • MySQL • Bootstrap</span>
            </div>

            <div class="card-box">
                <h3>🚗 Smart Voice Control Car</h3>
                <p>IoT project using ESP32 with Bluetooth voice commands, ultrasonic obstacle detection and motor control.</p>
                <ul>
                    <li><i class="fa-solid fa-check"></i> Voice Control</li>
                    <li><i class="fa-solid fa-check"></i> Bluetooth Control</li>
                    <li><i class="fa-solid fa-check"></i> Ultrasonic Sensor</li>
                    <li><i class="fa-solid fa-check"></i> Obstacle Detection</li>
                </ul>
                <span class="tech-tag-title">Technology</span>
                <span class="tech-tag-values">ESP32 • Arduino IDE • C++ • Dabble</span>
            </div>

        </div>
    </section>

    <!-- TIMELINE EDUCATION TRACKER -->
    <section id="education">
        <h2 class="title">Education</h2>
        <div class="glass edu-wrapper">
            <div class="edu-block">
                <h3>🎓 Bachelor of Information Technology (BIT)</h3>
                <p class="edu-meta">Informatics College Pokhara</p>
                <p style="font-size: 0.95rem; font-weight: 300;">2023 – Present</p>
            </div>
            <hr class="edu-separator">
            <div class="edu-block">
                <h3>🏫 Higher Secondary Education</h3>
                <p class="edu-meta">Balodaya Secondary English Boarding School</p>
            </div>
            <hr class="edu-separator">
            <div class="edu-block">
                <h3>🏫 Secondary Education</h3>
                <p class="edu-meta">Balodaya Secondary English Boarding School</p>
            </div>
        </div>
    </section>

    <!-- PROFICIENCY MILESTONES & CERTIFICATES -->
    <section>
        <h2 class="title">Certificates</h2>
        <div class="grid-layout">
            <div class="card-box">
                <h3>☕ Java Object-Oriented Programming</h3>
                <p>Successfully completed Java OOP programming course mastering structural object constraints.</p>
            </div>
            <div class="card-box">
                <h3>💻 Academic Software Projects</h3>
                <p>Developed multiple modular web and desktop applications using Java system pipelines.</p>
            </div>
            <div class="card-box">
                <h3>🌐 Web Development</h3>
                <p>Experience building responsive websites using HTML, CSS, JavaScript and Bootstrap.</p>
            </div>
        </div>
    </section>

    <!-- ANCHORED HUB CONTACT LAYER -->
    <section id="contact">
        <h2 class="title">Contact Me</h2>
        <div class="glass">
            <h3 style="font-family: var(--font-serif); font-size: 1.5rem; letter-spacing: 1px; margin-bottom: 30px; text-align: center;">Let's Work Together</h3>
            <div class="contact-details">
                <div class="contact-row-item">
                    <i class="fa-solid fa-envelope"></i> 
                    <span>kushal1259@gmail.com</span>
                </div>
                <div class="contact-row-item">
                    <i class="fa-solid fa-phone"></i> 
                    <span>+977 9849947086</span>
                </div>
                <div class="contact-row-item">
                    <i class="fa-solid fa-location-dot"></i> 
                    <span>Pokhara, Nepal</span>
                </div>
            </div>
            <div class="center-btn-box">
                <a href="mailto:kushal1259@gmail.com" class="btn btn-primary">Send Email</a>
            </div>
        </div>
    </section>

    <!-- CORPORATE STYLE ATTRIBUTION FOOTER -->
    <footer>
        <h2>Indra Bahadur Thakuri</h2>
        <p>© 2026 All Rights Reserved.</p>
    </footer>

    <!-- INTERACTION LOGIC & TYPING CORE ENGINE -->
    <script>
        const textArray = [
            "Full Stack Developer",
            "Java Developer",
            "BIT Student",
            "Web Developer"
        ];

        let arrayIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        let typingTimeoutId = null;

        function typeEffect() {
            const typingContainer = document.getElementById("typing");
            if (!typingContainer) return;

            const currentString = textArray[arrayIndex];

            if (isDeleting) {
                typingContainer.textContent = currentString.substring(0, charIndex - 1);
                charIndex--;
            } else {
                typingContainer.textContent = currentString.substring(0, charIndex + 1);
                charIndex++;
            }

            let typingSpeed = isDeleting ? 60 : 120;

            if (!isDeleting && charIndex === currentString.length) {
                typingSpeed = 1200; 
                isDeleting = true;
            } else if (isDeleting && charIndex === 0) {
                isDeleting = false;
                arrayIndex = (arrayIndex + 1) % textArray.length;
                typingSpeed = 300; 
            }

            typingTimeoutId = setTimeout(typeEffect, typingSpeed);
        }

        function toggleTheme() {
            const bodyElement = document.body;
            bodyElement.classList.toggle("light");
            
            const themeButtonIcon = document.querySelector(".theme-btn i");
            if (themeButtonIcon) {
                if (bodyElement.classList.contains("light")) {
                    themeButtonIcon.classList.replace("fa-moon", "fa-sun");
                } else {
                    themeButtonIcon.classList.replace("fa-sun", "fa-moon");
                }
            }
        }

        document.addEventListener("DOMContentLoaded", () => {
            setTimeout(typeEffect, 300);
        });
    </script>

</body>
</html>