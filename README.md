<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Ubaidullah Khan | ML & DL Developer</title>

    <meta
        name="description"
        content="Ubaidullah Khan - Machine Learning, Deep Learning and AI Developer"
    >

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #070b12;
            color: #e6edf3;
            line-height: 1.6;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        .container {
            width: 90%;
            max-width: 1150px;
            margin: auto;
        }

        /* ================= NAVBAR ================= */

        nav {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(7, 11, 18, 0.92);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid #1d2633;
        }

        .nav-container {
            height: 70px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
            color: #2ee88a;
        }

        .nav-links {
            display: flex;
            gap: 28px;
            list-style: none;
        }

        .nav-links a {
            color: #b8c2cc;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: #2ee88a;
        }

        /* ================= HERO ================= */

        .hero {
            min-height: 650px;
            display: flex;
            align-items: center;
            padding: 80px 0;
        }

        .hero-content {
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 70px;
            align-items: center;
        }

        .hero h1 {
            font-size: clamp(40px, 6vw, 68px);
            line-height: 1.1;
            margin-bottom: 20px;
        }

        .hero h1 span {
            color: #2ee88a;
        }

        .hero h2 {
            font-size: 25px;
            color: #43d9ff;
            margin-bottom: 25px;
        }

        .hero p {
            color: #aab5c2;
            font-size: 17px;
            max-width: 700px;
            margin-bottom: 25px;
        }

        .hero-info {
            list-style: none;
            margin-bottom: 30px;
        }

        .hero-info li {
            margin: 10px 0;
            color: #c7d0da;
        }

        .hero-info span {
            color: #2ee88a;
        }

        .buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 13px 24px;
            border-radius: 8px;
            border: 1px solid #2ee88a;
            transition: 0.3s;
            font-weight: bold;
        }

        .btn-primary {
            background: #2ee88a;
            color: #06110b;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(46, 232, 138, 0.2);
        }

        .btn-outline {
            color: #2ee88a;
        }

        .btn-outline:hover {
            background: #2ee88a;
            color: #06110b;
        }

        /* ================= PROFILE IMAGE ================= */

        .profile-box {
            display: flex;
            justify-content: center;
        }

        .profile-circle {
            width: 330px;
            height: 330px;
            border-radius: 50%;
            padding: 5px;
            background: linear-gradient(
                135deg,
                #2ee88a,
                #27c7ff,
                #2ee88a
            );
            box-shadow:
                0 0 40px rgba(46, 232, 138, 0.15),
                0 0 80px rgba(39, 199, 255, 0.08);
        }

        .profile-circle img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 50%;
            background: #111820;
        }

        /* ================= SECTIONS ================= */

        section {
            padding: 80px 0;
        }

        .section-title {
            font-size: 32px;
            margin-bottom: 45px;
        }

        .section-title span {
            color: #2ee88a;
        }

        /* ================= SKILLS ================= */

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(8, 1fr);
            gap: 15px;
        }

        .skill {
            background: #0d131b;
            border: 1px solid #202b38;
            border-radius: 12px;
            padding: 22px 10px;
            text-align: center;
            transition: 0.3s;
        }

        .skill:hover {
            transform: translateY(-6px);
            border-color: #2ee88a;
        }

        .skill img {
            width: 48px;
            height: 48px;
            object-fit: contain;
            margin-bottom: 10px;
        }

        .skill p {
            color: #c7d0da;
            font-size: 14px;
        }

        /* ================= STATS ================= */

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
        }

        .card {
            background: #0d131b;
            border: 1px solid #202b38;
            border-radius: 14px;
            padding: 25px;
        }

        .card h3 {
            color: #2ee88a;
            margin-bottom: 20px;
        }

        .stats-img {
            width: 100%;
            max-height: 200px;
            object-fit: contain;
        }

        /* ================= STREAK ================= */

        .streak-card {
            margin-top: 25px;
            text-align: center;
        }

        .streak-card img {
            width: 100%;
            max-width: 850px;
        }

        /* ================= ACTIVITY ================= */

        .activity-card {
            margin-top: 25px;
            overflow: hidden;
        }

        .activity-card img {
            width: 100%;
            display: block;
        }

        /* ================= PROJECTS ================= */

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .project {
            background: #0d131b;
            border: 1px solid #202b38;
            border-radius: 14px;
            padding: 25px;
            transition: 0.3s;
        }

        .project:hover {
            transform: translateY(-7px);
            border-color: #2ee88a;
        }

        .project h3 {
            color: #2ee88a;
            margin-bottom: 12px;
        }

        .project p {
            color: #9da9b5;
            margin-bottom: 20px;
        }

        .project-link {
            color: #43d9ff;
            font-weight: bold;
        }

        /* ================= CONTACT ================= */

        .contact {
            text-align: center;
        }

        .contact p {
            color: #aab5c2;
            margin-bottom: 25px;
        }

        .socials {
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        .social {
            width: 50px;
            height: 50px;
            border: 1px solid #293542;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: 0.3s;
            font-size: 22px;
        }

        .social:hover {
            border-color: #2ee88a;
            color: #2ee88a;
            transform: translateY(-5px);
        }

        /* ================= FOOTER ================= */

        footer {
            border-top: 1px solid #1d2633;
            text-align: center;
            padding: 30px;
            color: #75808d;
        }

        footer span {
            color: #2ee88a;
        }

        /* ================= RESPONSIVE ================= */

        @media (max-width: 1000px) {

            .skills-grid {
                grid-template-columns: repeat(4, 1fr);
            }

            .projects-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 768px) {

            .nav-links {
                display: none;
            }

            .hero {
                padding: 60px 0;
            }

            .hero-content {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero p {
                margin-left: auto;
                margin-right: auto;
            }

            .hero-info {
                text-align: left;
                display: inline-block;
            }

            .buttons {
                justify-content: center;
            }

            .profile-box {
                order: -1;
            }

            .profile-circle {
                width: 240px;
                height: 240px;
            }

            .stats-grid {
                grid-template-columns: 1fr;
            }

            .skills-grid {
                grid-template-columns: repeat(4, 1fr);
            }

            .projects-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 480px) {

            .container {
                width: 92%;
            }

            .skills-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .hero h1 {
                font-size: 40px;
            }

            .hero h2 {
                font-size: 20px;
            }
        }
    </style>
</head>

<body>

<!-- ================= NAVBAR ================= -->

<nav>
    <div class="container nav-container">

        <div class="logo">
            Ubaidullah.dev
        </div>

        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#stats">GitHub</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>

    </div>
</nav>


<!-- ================= HERO ================= -->

<section class="hero" id="home">

    <div class="container hero-content">

        <div>

            <h1>
                Hi 👋, I'm <span>Ubaidullah Khan</span>
            </h1>

            <h2>
                Building Intelligent Systems with ML & DL
            </h2>

            <p>
                I'm a passionate developer focused on Machine Learning,
                Deep Learning, and Artificial Intelligence. I enjoy
                building intelligent and data-driven applications
                that solve real-world problems.
            </p>

            <ul class="hero-info">

                <li>
                    🌍 Based in <span>Pakistan</span>
                </li>

                <li>
                    🧠 Currently learning
                    <span>Deep Learning & Advanced AI</span>
                </li>

                <li>
                    🤝 Open to collaborating on
                    <span>AI / ML Projects</span>
                </li>

                <li>
                    💬 Ask me about
                    <span>Python, ML, DL & AI</span>
                </li>

            </ul>

            <div class="buttons">

                <a
                    href="https://github.com/Ubaidullahkhan-dev"
                    target="_blank"
                    class="btn btn-primary"
                >
                    View GitHub
                </a>

                <a
                    href="https://www.linkedin.com/in/ubaid-ullah-7a051a352"
                    target="_blank"
                    class="btn btn-outline"
                >
                    LinkedIn
                </a>

            </div>

        </div>


        <!-- Profile Image -->

        <div class="profile-box">

            <div class="profile-circle">

                <!-- Replace profile.jpg with your image -->

                <img
                    src="profile.jpg"
                    alt="Ubaidullah Khan"
                >

            </div>

        </div>

    </div>

</section>


<!-- ================= SKILLS ================= -->

<section id="skills">

    <div class="container">

        <h2 class="section-title">
            🛠️ <span>Skills</span> & Tools
        </h2>

        <div class="skills-grid">

            <div class="skill">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg">
                <p>Git</p>
            </div>

            <div class="skill">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg">
                <p>Python</p>
            </div>

            <div class="skill">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg">
                <p>Java</p>
            </div>

            <div class="skill">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg">
                <p>VS Code</p>
            </div>

            <div class="skill">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg">
                <p>MySQL</p>
            </div>

            <div class="skill">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tensorflow/tensorflow-original.svg">
                <p>TensorFlow</p>
            </div>

            <div class="skill">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pytorch/pytorch-original.svg">
                <p>PyTorch</p>
            </div>

            <div class="skill">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/wordpress/wordpress-original.svg">
                <p>WordPress</p>
            </div>

        </div>

    </div>

</section>


<!-- ================= GITHUB STATS ================= -->

<section id="stats">

    <div class="container">

        <h2 class="section-title">
            📊 <span>GitHub</span> Statistics
        </h2>

        <div class="stats-grid">

            <!-- GitHub Stats -->

            <div class="card">

                <h3>
                    Ubaidullahkhan-dev's GitHub Stats
                </h3>

                <img
                    class="stats-img"
                    src="https://github-readme-stats.vercel.app/api?username=Ubaidullahkhan-dev&show_icons=true&theme=dark&hide_border=true&bg_color=0d131b&title_color=2ee88a&icon_color=43d9ff"
                    alt="GitHub Stats"
                >

            </div>


            <!-- Languages -->

            <div class="card">

                <h3>
                    Most Used Languages
                </h3>

                <img
                    class="stats-img"
                    src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ubaidullahkhan-dev&layout=compact&theme=dark&hide_border=true&bg_color=0d131b&title_color=2ee88a"
                    alt="Most Used Languages"
                >

            </div>

        </div>


        <!-- ================= STREAK ================= -->

        <div class="card streak-card">

            <h3>
                🔥 GitHub Contribution Streak
            </h3>

            <img
                src="https://streak-stats.demolab.com/?user=Ubaidullahkhan-dev&theme=dark&hide_border=true&background=0d131b&ring=2ee88a&fire=2ee88a&currStreakLabel=2ee88a"
                alt="GitHub Streak"
            >

        </div>


        <!-- ================= ACTIVITY GRAPH ================= -->

        <div class="card activity-card">

            <h3>
                📈 GitHub Activity
            </h3>

            <img
                src="https://github-readme-activity-graph.vercel.app/graph?username=Ubaidullahkhan-dev&bg_color=0d131b&color=2ee88a&line=2ee88a&point=43d9ff&area=true&hide_border=true"
                alt="GitHub Activity Graph"
            >

        </div>

    </div>

</section>


<!-- ================= PROJECTS ================= -->

<section id="projects">

    <div class="container">

        <h2 class="section-title">
            🚀 Featured <span>Projects</span>
        </h2>

        <div class="projects-grid">

            <div class="project">

                <h3>
                    🤖 Smart AI Timetable Generator
                </h3>

                <p>
                    An intelligent timetable generation application
                    designed to automatically create optimized
                    schedules.
                </p>

                <a
                    href="https://github.com/Ubaidullahkhan-dev"
                    target="_blank"
                    class="project-link"
                >
                    View Project →
                </a>

            </div>


            <div class="project">

                <h3>
                    🎙️ AI Voice Assistant
                </h3>

                <p>
                    AI voice assistant using speech recognition,
                    LLM integration and text-to-speech technologies.
                </p>

                <a
                    href="https://github.com/Ubaidullahkhan-dev"
                    target="_blank"
                    class="project-link"
                >
                    View Project →
                </a>

            </div>


            <div class="project">

                <h3>
                    🧠 Deep Learning Projects
                </h3>

                <p>
                    Collection of Deep Learning experiments including
                    neural networks, callbacks and model training.
                </p>

                <a
                    href="https://github.com/Ubaidullahkhan-dev"
                    target="_blank"
                    class="project-link"
                >
                    View Projects →
                </a>

            </div>

        </div>

    </div>

</section>


<!-- ================= CONTACT ================= -->

<section id="contact">

    <div class="container contact">

        <h2 class="section-title">
            🌐 Let's <span>Connect</span>
        </h2>

        <p>
            I'm always interested in learning, collaborating and
            building innovative AI-powered solutions.
        </p>

        <div class="socials">

            <a
                class="social"
                href="https://github.com/Ubaidullahkhan-dev"
                target="_blank"
                title="GitHub"
            >
                🐙
            </a>

            <a
                class="social"
                href="https://www.linkedin.com/in/ubaid-ullah-7a051a352"
                target="_blank"
                title="LinkedIn"
            >
                in
            </a>

            <a
                class="social"
                href="mailto:uu3513610@gmail.com"
                title="Email"
            >
                ✉
            </a>

        </div>

    </div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

    <p>
        © 2026 <span>Ubaidullah Khan</span>.
        Built with passion for AI & Technology.
    </p>

</footer>

</body>
</html>
