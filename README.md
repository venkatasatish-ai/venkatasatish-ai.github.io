<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Venkata Satish | Data & AI Career Blog</title>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
    <style>
        /* ----- RESET & BASE ----- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f4f7fc;
            color: #1e2a41;
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* ----- HEADER / NAV ----- */
        header {
            background: linear-gradient(135deg, #0b1a33 0%, #1a3a5c 100%);
            color: #fff;
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }

        .header-flex {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .logo h1 {
            font-size: 1.8rem;
            font-weight: 700;
            letter-spacing: -0.5px;
        }

        .logo h1 span {
            color: #6fc3ff;
        }

        .logo p {
            font-size: 0.85rem;
            opacity: 0.8;
            margin-top: 2px;
            letter-spacing: 1px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 28px;
            flex-wrap: wrap;
        }

        nav ul li a {
            font-weight: 500;
            font-size: 0.95rem;
            padding: 6px 0;
            border-bottom: 2px solid transparent;
            transition: 0.3s;
        }

        nav ul li a:hover {
            border-bottom-color: #6fc3ff;
            color: #6fc3ff;
        }

        .nav-cta {
            background: #6fc3ff;
            color: #0b1a33 !important;
            padding: 8px 18px !important;
            border-radius: 30px;
            font-weight: 600;
            border-bottom: none !important;
            transition: 0.3s;
        }

        .nav-cta:hover {
            background: #fff;
            color: #0b1a33 !important;
            transform: scale(1.03);
        }

        /* ----- HERO SECTION ----- */
        .hero {
            background: linear-gradient(135deg, #e8f0fe 0%, #d4e4f7 100%);
            padding: 60px 0 50px;
            border-bottom: 1px solid #cbd8e9;
        }

        .hero-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .hero-text h2 {
            font-size: 2.8rem;
            font-weight: 800;
            line-height: 1.2;
            color: #0b1a33;
        }

        .hero-text h2 .highlight {
            color: #0066b3;
            background: rgba(111, 195, 255, 0.25);
            padding: 0 8px;
            border-radius: 6px;
        }

        .hero-text p {
            font-size: 1.15rem;
            color: #1e3a5f;
            margin: 20px 0 30px;
            max-width: 500px;
        }

        .hero-badge-group {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-bottom: 25px;
        }

        .hero-badge {
            background: #fff;
            padding: 6px 18px;
            border-radius: 50px;
            font-size: 0.8rem;
            font-weight: 600;
            color: #0b1a33;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.06);
            border: 1px solid #cbd8e9;
        }

        .hero-badge i {
            color: #0066b3;
            margin-right: 6px;
        }

        .hero-actions {
            display: flex;
            gap: 16px;
            flex-wrap: wrap;
        }

        .btn-primary {
            background: #0b1a33;
            color: #fff;
            padding: 12px 32px;
            border-radius: 40px;
            font-weight: 600;
            transition: 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            border: none;
            cursor: pointer;
        }

        .btn-primary:hover {
            background: #1a3a5c;
            transform: translateY(-2px);
            box-shadow: 0 8px 24px rgba(11, 26, 51, 0.25);
        }

        .btn-outline {
            background: transparent;
            color: #0b1a33;
            padding: 12px 32px;
            border-radius: 40px;
            font-weight: 600;
            border: 2px solid #0b1a33;
            transition: 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 10px;
        }

        .btn-outline:hover {
            background: #0b1a33;
            color: #fff;
            transform: translateY(-2px);
        }

        .hero-image {
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .hero-image .avatar-circle {
            width: 320px;
            height: 320px;
            border-radius: 50%;
            background: linear-gradient(135deg, #0b1a33, #1a3a5c);
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: 0 20px 60px rgba(11, 26, 51, 0.25);
            border: 6px solid rgba(255, 255, 255, 0.6);
        }

        .avatar-circle i {
            font-size: 10rem;
            color: #6fc3ff;
            opacity: 0.9;
        }

        /* ----- SECTION TITLES ----- */
        .section-title {
            text-align: center;
            margin-bottom: 40px;
        }

        .section-title h3 {
            font-size: 2.2rem;
            font-weight: 700;
            color: #0b1a33;
        }

        .section-title p {
            color: #3a5a7a;
            max-width: 600px;
            margin: 10px auto 0;
        }

        .section-title .accent-line {
            width: 60px;
            height: 4px;
            background: #0066b3;
            margin: 12px auto 0;
            border-radius: 4px;
        }

        /* ----- TOPICS GRID (Data & AI) ----- */
        .topics-section {
            padding: 70px 0 50px;
        }

        .topics-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
            gap: 30px;
        }

        .topic-card {
            background: #fff;
            border-radius: 20px;
            padding: 30px 24px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.05);
            transition: 0.3s;
            border: 1px solid #e9eef5;
            position: relative;
            overflow: hidden;
        }

        .topic-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.08);
            border-color: #b8d0e8;
        }

        .topic-card .icon-wrap {
            font-size: 2.4rem;
            color: #0066b3;
            margin-bottom: 16px;
        }

        .topic-card h4 {
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: #0b1a33;
        }

        .topic-card p {
            color: #3a5a7a;
            font-size: 0.95rem;
        }

        .topic-card .tag {
            display: inline-block;
            margin-top: 14px;
            font-size: 0.7rem;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            background: #e8f0fe;
            color: #0066b3;
            padding: 4px 14px;
            border-radius: 30px;
        }

        /* ----- BLOG POSTS (Career Journey) ----- */
        .blog-section {
            background: #fff;
            padding: 70px 0 60px;
        }

        .blog-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
            gap: 35px;
        }

        .blog-card {
            background: #f9fbfd;
            border-radius: 20px;
            overflow: hidden;
            border: 1px solid #e9eef5;
            transition: 0.3s;
        }

        .blog-card:hover {
            transform: translateY(-6px);
            box-shadow: 0 16px 48px rgba(0, 0, 0, 0.07);
        }

        .blog-card .blog-img {
            height: 180px;
            background: linear-gradient(135deg, #d4e4f7, #b0cce5);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3.5rem;
            color: #0b1a33;
            opacity: 0.7;
        }

        .blog-card .blog-body {
            padding: 24px 26px 30px;
        }

        .blog-card .blog-meta {
            font-size: 0.8rem;
            color: #5a7a9a;
            display: flex;
            gap: 18px;
            margin-bottom: 10px;
        }

        .blog-card .blog-meta i {
            margin-right: 4px;
        }

        .blog-card h4 {
            font-size: 1.25rem;
            color: #0b1a33;
            margin-bottom: 10px;
        }

        .blog-card p {
            color: #3a5a7a;
            font-size: 0.95rem;
        }

        .blog-card .read-more {
            display: inline-block;
            margin-top: 16px;
            font-weight: 600;
            color: #0066b3;
            transition: 0.3s;
        }

        .blog-card .read-more:hover {
            color: #0b1a33;
            transform: translateX(4px);
        }

        /* ----- SKILLS / CLOUD BADGES ----- */
        .skills-section {
            background: #e8f0fe;
            padding: 60px 0;
        }

        .skills-cloud {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 16px 24px;
            max-width: 900px;
            margin: 0 auto;
        }

        .skill-item {
            background: #fff;
            padding: 10px 26px;
            border-radius: 60px;
            font-weight: 600;
            font-size: 0.95rem;
            color: #0b1a33;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.04);
            border: 1px solid #d4e4f7;
            transition: 0.3s;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .skill-item i {
            color: #0066b3;
            font-size: 1.1rem;
        }

        .skill-item:hover {
            transform: scale(1.04);
            border-color: #0066b3;
            box-shadow: 0 6px 20px rgba(0, 102, 179, 0.12);
        }

        /* ----- CTA SECTION ----- */
        .cta-section {
            background: linear-gradient(135deg, #0b1a33, #1a3a5c);
            color: #fff;
            padding: 60px 0;
            text-align: center;
        }

        .cta-section h3 {
            font-size: 2.2rem;
            font-weight: 700;
        }

        .cta-section p {
            max-width: 500px;
            margin: 16px auto 30px;
            opacity: 0.85;
            font-size: 1.1rem;
        }

        .cta-section .btn-primary {
            background: #6fc3ff;
            color: #0b1a33;
        }

        .cta-section .btn-primary:hover {
            background: #fff;
        }

        /* ----- FOOTER ----- */
        footer {
            background: #071220;
            color: #a0b8d0;
            padding: 30px 0;
            text-align: center;
            border-top: 1px solid #1a3a5c;
        }

        footer .social-links {
            display: flex;
            justify-content: center;
            gap: 24px;
            margin-bottom: 16px;
        }

        footer .social-links a {
            color: #a0b8d0;
            font-size: 1.3rem;
            transition: 0.3s;
        }

        footer .social-links a:hover {
            color: #6fc3ff;
            transform: translateY(-3px);
        }

        footer p {
            font-size: 0.9rem;
            opacity: 0.7;
        }

        /* ----- RESPONSIVE ----- */
        @media (max-width: 900px) {
            .hero-grid {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero-text p {
                margin-left: auto;
                margin-right: auto;
            }

            .hero-actions {
                justify-content: center;
            }

            .hero-badge-group {
                justify-content: center;
            }

            .hero-image .avatar-circle {
                width: 220px;
                height: 220px;
            }

            .avatar-circle i {
                font-size: 6rem;
            }

            .header-flex {
                flex-direction: column;
                gap: 16px;
            }

            nav ul {
                justify-content: center;
                gap: 16px;
            }

            .section-title h3 {
                font-size: 1.8rem;
            }
        }

        @media (max-width: 550px) {
            .hero-text h2 {
                font-size: 2rem;
            }

            .blog-grid {
                grid-template-columns: 1fr;
            }

            .topics-grid {
                grid-template-columns: 1fr;
            }

            .skills-cloud {
                gap: 10px;
            }

            .skill-item {
                font-size: 0.8rem;
                padding: 6px 16px;
            }
        }
    </style>
</head>
<body>

    <!-- ===== HEADER ===== -->
    <header>
        <div class="container header-flex">
            <div class="logo">
                <h1>Venkata <span>Satish</span></h1>
                <p>Data · AI · Cloud · Automation</p>
            </div>
            <nav>
                <ul>
                    <li><a href="#topics">Topics</a></li>
                    <li><a href="#blog">Blog</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#contact" class="nav-cta"><i class="fas fa-paper-plane"></i> Let's Talk</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- ===== HERO ===== -->
    <section class="hero">
        <div class="container hero-grid">
            <div class="hero-text">
                <h2>
                    Building the <span class="highlight">Future</span> of<br />
                    Data &amp; AI
                </h2>
                <p>
                    Hi, I'm Venkata Satish — a Data &amp; AI professional passionate about
                    Data Science, Engineering, Cloud, and Agentic AI. Explore my career journey
                    and insights.
                </p>
                <div class="hero-badge-group">
                    <span class="hero-badge"><i class="fas fa-database"></i> Data</span>
                    <span class="hero-badge"><i class="fas fa-cloud"></i> Cloud</span>
                    <span class="hero-badge"><i class="fas fa-robot"></i> AI</span>
                    <span class="hero-badge"><i class="fas fa-brain"></i> Gen AI</span>
                    <span class="hero-badge"><i class="fas fa-cogs"></i> Automation</span>
                </div>
                <div class="hero-actions">
                    <a href="#blog" class="btn-primary"><i class="fas fa-newspaper"></i> Read Blog</a>
                    <a href="#contact" class="btn-outline"><i class="fas fa-user-plus"></i> Connect</a>
                </div>
            </div>
            <div class="hero-image">
                <div class="avatar-circle">
                    <i class="fas fa-user-circle"></i>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== TOPICS ===== -->
    <section class="topics-section" id="topics">
        <div class="container">
            <div class="section-title">
                <h3>Core Expertise</h3>
                <p>End‑to‑end data &amp; AI capabilities — from ingestion to intelligent agents.</p>
                <div class="accent-line"></div>
            </div>
            <div class="topics-grid">

                <div class="topic-card">
                    <div class="icon-wrap"><i class="fas fa-chart-line"></i></div>
                    <h4>Data Science</h4>
                    <p>Statistical modeling, ML, predictive analytics, and storytelling with data.</p>
                    <span class="tag">Python · R · SQL</span>
                </div>

                <div class="topic-card">
                    <div class="icon-wrap"><i class="fas fa-chart-pie"></i></div>
                    <h4>Data Analytics</h4>
                    <p>Interactive dashboards, BI, and actionable insights from complex datasets.</p>
                    <span class="tag">Power BI · Tableau · Looker</span>
                </div>

                <div class="topic-card">
                    <div class="icon-wrap"><i class="fas fa-code-branch"></i></div>
                    <h4>Data Engineering</h4>
                    <p>Scalable pipelines, ETL/ELT, data warehousing, and lakehouse architectures.</p>
                    <span class="tag">Spark · Airflow · Kafka</span>
                </div>

                <div class="topic-card">
                    <div class="icon-wrap"><i class="fas fa-databricks"></i></div>
                    <h4>Databricks</h4>
                    <p>Lakehouse platform, Delta Lake, Unity Catalog, and MLflow at scale.</p>
                    <span class="tag">Delta · MLflow · SQL</span>
                </div>

                <div class="topic-card">
                    <div class="icon-wrap"><i class="fas fa-cloud-upload-alt"></i></div>
                    <h4>Cloud</h4>
                    <p>Architecting resilient, cost‑optimized data solutions on AWS, Azure &amp; GCP.</p>
                    <span class="tag">AWS · Azure · GCP</span>
                </div>

                <div class="topic-card">
                    <div class="icon-wrap"><i class="fas fa-robot"></i></div>
                    <h4>AI &amp; Gen AI</h4>
                    <p>LLMs, RAG, fine‑tuning, and generative applications for enterprise.</p>
                    <span class="tag">OpenAI · LangChain · HuggingFace</span>
                </div>

                <div class="topic-card">
                    <div class="icon-wrap"><i class="fas fa-network-wired"></i></div>
                    <h4>Agentic AI</h4>
                    <p>Autonomous agents, multi‑agent systems, and tool‑calling workflows.</p>
                    <span class="tag">CrewAI · AutoGen · Semantic Kernel</span>
                </div>

                <div class="topic-card">
                    <div class="icon-wrap"><i class="fas fa-sync-alt"></i></div>
                    <h4>Automation</h4>
                    <p>Infrastructure as Code, CI/CD, MLOps, and workflow orchestration.</p>
                    <span class="tag">Terraform · GitHub Actions · Kubeflow</span>
                </div>

            </div>
        </div>
    </section>

    <!-- ===== BLOG POSTS ===== -->
    <section class="blog-section" id="blog">
        <div class="container">
            <div class="section-title">
                <h3>Career Blog</h3>
                <p>Insights, tutorials, and lessons from my journey in Data &amp; AI.</p>
                <div class="accent-line"></div>
            </div>
            <div class="blog-grid">

                <!-- Post 1 -->
                <div class="blog-card">
                    <div class="blog-img"><i class="fas fa-cloud-upload-alt"></i></div>
                    <div class="blog-body">
                        <div class="blog-meta">
                            <span><i class="far fa-calendar-alt"></i> 02 Aug 2026</span>
                            <span><i class="far fa-clock"></i> 6 min read</span>
                        </div>
                        <h4>Building a Data Lakehouse on Databricks</h4>
                        <p>Step‑by‑step guide to architecting a lakehouse with Delta Lake, Unity Catalog, and cost‑optimized cloud storage.</p>
                        <a href="#" class="read-more">Read More <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>

                <!-- Post 2 -->
                <div class="blog-card">
                    <div class="blog-img"><i class="fas fa-robot"></i></div>
                    <div class="blog-body">
                        <div class="blog-meta">
                            <span><i class="far fa-calendar-alt"></i> 20 Jul 2026</span>
                            <span><i class="far fa-clock"></i> 8 min read</span>
                        </div>
                        <h4>From RAG to Agentic AI</h4>
                        <p>How we evolved from simple retrieval‑augmented generation to autonomous multi‑agent systems that reason and act.</p>
                        <a href="#" class="read-more">Read More <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>

                <!-- Post 3 -->
                <div class="blog-card">
                    <div class="blog-img"><i class="fas fa-cogs"></i></div>
                    <div class="blog-body">
                        <div class="blog-meta">
                            <span><i class="far fa-calendar-alt"></i> 05 Jul 2026</span>
                            <span><i class="far fa-clock"></i> 5 min read</span>
                        </div>
                        <h4>Automating MLOps Pipelines</h4>
                        <p>End‑to‑end automation with GitHub Actions, Terraform, and Kubeflow — from data ingestion to model deployment.</p>
                        <a href="#" class="read-more">Read More <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>

                <!-- Post 4 -->
                <div class="blog-card">
                    <div class="blog-img"><i class="fas fa-chart-pie"></i></div>
                    <div class="blog-body">
                        <div class="blog-meta">
                            <span><i class="far fa-calendar-alt"></i> 18 Jun 2026</span>
                            <span><i class="far fa-clock"></i> 4 min read</span>
                        </div>
                        <h4>Modern Data Analytics with Power BI &amp; Fabric</h4>
                        <p>Leveraging Microsoft Fabric and Power BI to deliver real‑time dashboards and self‑service analytics at scale.</p>
                        <a href="#" class="read-more">Read More <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>

                <!-- Post 5 -->
                <div class="blog-card">
                    <div class="blog-img"><i class="fas fa-brain"></i></div>
                    <div class="blog-body">
                        <div class="blog-meta">
                            <span><i class="far fa-calendar-alt"></i> 02 Jun 2026</span>
                            <span><i class="far fa-clock"></i> 7 min read</span>
                        </div>
                        <h4>Gen AI in Production: Lessons Learned</h4>
                        <p>Practical tips for deploying LLMs — from prompt engineering and RAG to monitoring, cost, and latency.</p>
                        <a href="#" class="read-more">Read More <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>

                <!-- Post 6 -->
                <div class="blog-card">
                    <div class="blog-img"><i class="fas fa-network-wired"></i></div>
                    <div class="blog-body">
                        <div class="blog-meta">
                            <span><i class="far fa-calendar-alt"></i> 15 May 2026</span>
                            <span><i class="far fa-clock"></i> 9 min read</span>
                        </div>
                        <h4>Designing Agentic Workflows with CrewAI</h4>
                        <p>Orchestrating autonomous AI agents that collaborate, reason, and execute complex tasks with human‑in‑the‑loop.</p>
                        <a href="#" class="read-more">Read More <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- ===== SKILLS / CLOUD ===== -->
    <section class="skills-section" id="skills">
        <div class="container">
            <div class="section-title">
                <h3>Tech Stack &amp; Tools</h3>
                <p>My daily toolkit for building data &amp; AI solutions.</p>
                <div class="accent-line"></div>
            </div>
            <div class="skills-cloud">
                <span class="skill-item"><i class="fab fa-python"></i> Python</span>
                <span class="skill-item"><i class="fas fa-database"></i> SQL</span>
                <span class="skill-item"><i class="fab fa-aws"></i> AWS</span>
                <span class="skill-item"><i class="fab fa-microsoft"></i> Azure</span>
                <span class="skill-item"><i class="fab fa-google"></i> GCP</span>
                <span class="skill-item"><i class="fas fa-databricks"></i> Databricks</span>
                <span class="skill-item"><i class="fas fa-fire"></i> Apache Spark</span>
                <span class="skill-item"><i class="fas fa-stream"></i> Kafka</span>
                <span class="skill-item"><i class="fas fa-cube"></i> Kubernetes</span>
                <span class="skill-item"><i class="fas fa-code-branch"></i> Airflow</span>
                <span class="skill-item"><i class="fas fa-robot"></i> LangChain</span>
                <span class="skill-item"><i class="fas fa-brain"></i> PyTorch</span>
                <span class="skill-item"><i class="fas fa-chart-line"></i> Power BI</span>
                <span class="skill-item"><i class="fas fa-table"></i> Tableau</span>
                <span class="skill-item"><i class="fas fa-code"></i> Terraform</span>
                <span class="skill-item"><i class="fas fa-cogs"></i> MLflow</span>
                <span class="skill-item"><i class="fas fa-network-wired"></i> CrewAI</span>
                <span class="skill-item"><i class="fas fa-cloud"></i> Docker</span>
            </div>
        </div>
    </section>

    <!-- ===== CTA / CONTACT ===== -->
    <section class="cta-section" id="contact">
        <div class="container">
            <h3>Let's Build Something <span style="color:#6fc3ff;">Intelligent</span></h3>
            <p>Whether it's a data platform, an AI agent, or a career move — I'd love to connect.</p>
            <a href="https://wa.me/message/6IMW4V7GZI44P1" class="btn-primary">
                <i class="fas fa-paper-plane"></i> Get in Touch
            </a>
        </div>
    </section>

    <!-- ===== FOOTER ===== -->
    <footer>
        <div class="container">
            <div class="social-links">
                <a href="#" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                <a href="#" aria-label="GitHub"><i class="fab fa-github"></i></a>
                <a href="#" aria-label="Twitter"><i class="fab fa-x-twitter"></i></a>
                <a href="#" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
                <a href="#" aria-label="Medium"><i class="fab fa-medium-m"></i></a>
            </div>
            <p>&copy; 2026 Venkata Satish — Data &amp; AI Career Blog. Built with <i class="fas fa-heart" style="color:#6fc3ff;"></i></p>
        </div>
    </footer>

</body>
</html>
