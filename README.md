
    <style>
        /* ==========================================================================
           ESTILOS E VARIÁVEIS (CSS EMBUTIDO)
           ========================================================================== */
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --card-border: #334155;
            --text-primary: #f8fafc;
            --text-secondary: #94a3b8;
            --accent: #38bdf8;
            --accent-glow: rgba(56, 189, 248, 0.15);
            --font-main: 'Inter', sans-serif;
            --radius: 12px;
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-primary);
            font-family: var(--font-main);
            line-height: 1.6;
            padding: 40px 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
        }

        /* CABEÇALHO / HERO */
        .profile-header {
            text-align: center;
            padding: 40px 20px;
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: var(--radius);
            margin-bottom: 30px;
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.3);
        }

        .profile-avatar {
            width: 80px;
            height: 80px;
            background: var(--accent-glow);
            border: 2px solid var(--accent);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px auto;
            font-size: 2rem;
            color: var(--accent);
        }

        .profile-name {
            font-size: 2.2rem;
            font-weight: 700;
            color: var(--text-primary);
            margin-bottom: 8px;
        }

        .profile-title {
            font-size: 1.1rem;
            color: var(--accent);
            font-weight: 500;
            margin-bottom: 15px;
        }

        .profile-bio {
            color: var(--text-secondary);
            max-width: 600px;
            margin: 0 auto 20px auto;
            font-size: 0.95rem;
        }

        .social-links a {
            color: var(--text-secondary);
            font-size: 1.5rem;
            margin: 0 10px;
            transition: var(--transition);
            text-decoration: none;
        }

        .social-links a:hover {
            color: var(--accent);
        }

        /* SEÇÕES E CARDS */
        .section {
            margin-bottom: 35px;
        }

        .section-title {
            font-size: 1.3rem;
            color: var(--text-primary);
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .section-title i {
            color: var(--accent);
        }

        .card {
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: var(--radius);
            padding: 24px;
            transition: var(--transition);
        }

        .card:hover {
            border-color: var(--accent);
            box-shadow: 0 4px 20px var(--accent-glow);
        }

        .card-accent {
            border-left: 4px solid var(--accent);
        }

        .margin-bottom {
            margin-bottom: 20px;
        }

        /* LINHA DO TEMPO (TIMELINE) */
        .timeline {
            position: relative;
            padding-left: 20px;
            border-left: 2px solid var(--card-border);
        }

        .timeline-item {
            position: relative;
            margin-bottom: 25px;
            padding-left: 20px;
        }

        .timeline-item:last-child {
            margin-bottom: 0;
        }

        .timeline-dot {
            position: absolute;
            left: -27px;
            top: 5px;
            width: 12px;
            height: 12px;
            background: var(--bg-color);
            border: 2px solid var(--accent);
            border-radius: 50%;
            transition: var(--transition);
        }

        .timeline-item:hover .timeline-dot {
            background: var(--accent);
            box-shadow: 0 0 10px var(--accent);
        }

        .timeline-date {
            display: inline-block;
            font-size: 0.8rem;
            color: var(--accent);
            font-weight: 600;
            margin-bottom: 4px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .timeline-content h3 {
            font-size: 1.05rem;
            color: var(--text-primary);
            margin-bottom: 6px;
        }

        .timeline-content p {
            color: var(--text-secondary);
            font-size: 0.9rem;
        }

        /* GRID & EXPERIÊNCIA */
        .grid-2-col {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .experience-badge {
            display: inline-block;
            background: var(--accent-glow);
            color: var(--accent);
            font-size: 0.75rem;
            font-weight: 600;
            padding: 4px 10px;
            border-radius: 20px;
            margin-bottom: 12px;
        }

        .role-title {
            font-size: 1.1rem;
            color: var(--text-primary);
        }

        .role-subtitle {
            font-size: 0.85rem;
            color: var(--accent);
            margin-bottom: 15px;
        }

        .skills-list {
            list-style: none;
        }

        .skills-list li {
            color: var(--text-secondary);
            font-size: 0.88rem;
            margin-bottom: 8px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .skills-list li i {
            color: var(--accent);
            font-size: 0.75rem;
        }

        .institution {
            color: var(--text-secondary);
            font-size: 0.88rem;
        }

        /* BADGES & TECNOLOGIAS */
        .skills-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .skills-group-title {
            font-size: 1rem;
            margin-bottom: 15px;
            color: var(--text-primary);
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .badges-wrapper {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .badge {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid var(--card-border);
            color: var(--text-primary);
            padding: 6px 12px;
            border-radius: 6px;
            font-size: 0.85rem;
            display: flex;
            align-items: center;
            gap: 6px;
            transition: var(--transition);
        }

        .badge:hover {
            border-color: var(--accent);
            transform: translateY(-2px);
        }

        .badge-learning {
            border-style: dashed;
            color: var(--text-secondary);
        }

        /* RODAPÉ */
        .footer {
            text-align: center;
            padding: 20px 0;
            color: var(--text-secondary);
            font-size: 0.85rem;
            border-top: 1px solid var(--card-border);
            margin-top: 40px;
        }

        /* RESPONSIVIDADE (MEDIA QUERIES) */
        @media (max-width: 768px) {
            .grid-2-col,
            .skills-container {
                grid-template-columns: 1fr;
            }
            
            .profile-name {
                font-size: 1.8rem;
            }
            
            body {
                padding: 20px 12px;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        
        <!-- CABEÇALHO / HERO -->
        <header class="profile-header">
            <div class="profile-avatar">
                <i class="fa-solid fa-user-gear"></i>
            </div>
            <h1 class="profile-name">Vinicius Santos da Silva</h1>
            <p class="profile-title">Tecnologia da Informação | Logística | Gestão</p>
            <p class="profile-bio">
                Unindo a visão analítica do Desenvolvimento de Sistemas à eficiência operacional da Logística e da Gestão de TI.
            </p>
            <div class="social-links">
                <a href="https://linkedin.com" target="_blank" aria-label="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>
                <a href="https://github.com" target="_blank" aria-label="GitHub"><i class="fa-brands fa-github"></i></a>
            </div>
        </header>

        <!-- OBJETIVO PROFISSIONAL -->
        <section class="section">
            <h2 class="section-title"><i class="fa-solid fa-bullseye"></i> Objetivo Profissional</h2>
            <div class="card card-accent">
                <p>
                    Meu objetivo é conectar a experiência prática em <strong>Logística</strong> aos conhecimentos em <strong>Tecnologia da Informação e Gestão</strong>, desenvolvendo soluções tecnológicas capazes de otimizar processos, aumentar a eficiência operacional e contribuir estrategicamente na tomada de decisões organizacionais.
                </p>
            </div>
        </section>

        <!-- LINHA DO TEMPO / TRAJETÓRIA -->
        <section class="section">
            <h2 class="section-title"><i class="fa-solid fa-route"></i> Minha Trajetória</h2>
            <div class="timeline">
                
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="timeline-date">2022</span>
                        <h3>Início no Desenvolvimento de Sistemas</h3>
                        <p>Início do curso técnico, estabelecendo as bases de lógica, bancos de dados e programação.</p>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="timeline-date">2023</span>
                        <h3>Conclusão & Entrada na Logística</h3>
                        <p>Conclusão da formação técnica e início da trajetória prática nas operações logísticas como Ajudante Geral em distribuidora de eletrônicos.</p>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="timeline-date">2023 - Atual</span>
                        <h3>Evolução Profissional & Liderança</h3>
                        <p>Promoção para <strong>Líder de Expedição</strong>. Gestão de equipes, organização de processos operacionais e expedição.</p>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="timeline-date">2026</span>
                        <h3>Graduação em Gestão da TI</h3>
                        <p>Início do curso superior em Gestão da Tecnologia da Informação (atualmente no 2º Semestre).</p>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="timeline-date">2026 - Atual</span>
                        <h3>Foco e Aprimoramento Técnico</h3>
                        <p>Aprofundamento contínuo em Python, Linguagem C, modelagem de Banco de Dados e sistemas aplicados à gestão.</p>
                    </div>
                </div>

            </div>
        </section>

        <!-- EXPERIÊNCIA E FORMAÇÃO (2 COLUNAS) -->
        <div class="grid-2-col">
            
            <!-- EXPERIÊNCIA PROFISSIONAL -->
            <section class="section">
                <h2 class="section-title"><i class="fa-solid fa-briefcase"></i> Experiência</h2>
                <div class="card">
                    <div class="experience-badge">Promoção Conquistada</div>
                    <h3 class="role-title">Líder de Expedição</h3>
                    <p class="role-subtitle">Ajudante Geral <i class="fa-solid fa-arrow-right"></i> Líder de Expedição</p>
                    <ul class="skills-list">
                        <li><i class="fa-solid fa-check"></i> Liderança e gestão de equipes em campo</li>
                        <li><i class="fa-solid fa-check"></i> Controle de processos e rotinas de expedição</li>
                        <li><i class="fa-solid fa-check"></i> Organização e tomada de decisões ágeis</li>
                        <li><i class="fa-solid fa-check"></i> Resolução de problemas operacionais</li>
                    </ul>
                </div>
            </section>

            <!-- FORMAÇÃO ACADÊMICA -->
            <section class="section">
                <h2 class="section-title"><i class="fa-solid fa-graduation-cap"></i> Formação</h2>
                
                <div class="card margin-bottom">
                    <span class="timeline-date">2026 - Cursando (2º Semestre)</span>
                    <h3>Gestão da Tecnologia da Informação</h3>
                    <p class="institution">Ensino Superior</p>
                </div>

                <div class="card">
                    <span class="timeline-date">2022 - 2023</span>
                    <h3>Desenvolvimento de Sistemas</h3>
                    <p class="institution">Curso Técnico</p>
                </div>
            </section>

        </div>

        <!-- TECNOLOGIAS E COMPETÊNCIAS -->
        <section class="section">
            <h2 class="section-title"><i class="fa-solid fa-code"></i> Tecnologias & Conhecimentos</h2>
            
            <div class="skills-container">
                
                <!-- CONHECIMENTOS ADQUIRIDOS -->
                <div class="card">
                    <h3 class="skills-group-title"><i class="fa-solid fa-circle-check"></i> Conhecimentos</h3>
                    <div class="badges-wrapper">
                        <span class="badge"><i class="fa-brands fa-java"></i> Java</span>
                        <span class="badge"><i class="fa-brands fa-html5"></i> HTML5</span>
                        <span class="badge"><i class="fa-brands fa-css3-alt"></i> CSS3</span>
                        <span class="badge"><i class="fa-brands fa-js"></i> JavaScript</span>
                        <span class="badge"><i class="fa-brands fa-android"></i> Kotlin / Android Studio</span>
                        <span class="badge"><i class="fa-solid fa-database"></i> SQL Server</span>
                        <span class="badge"><i class="fa-solid fa-diagram-project"></i> Lógica & Sistemas</span>
                    </div>
                </div>

                <!-- EM APRENDIZADO -->
                <div class="card">
                    <h3 class="skills-group-title"><i class="fa-solid fa-spinner"></i> Em Aprendizado</h3>
                    <div class="badges-wrapper">
                        <span class="badge badge-learning"><i class="fa-brands fa-python"></i> Python</span>
                        <span class="badge badge-learning"><i class="fa-solid fa-c"></i> Linguagem C</span>
                        <span class="badge badge-learning"><i class="fa-solid fa-server"></i> Banco de Dados</span>
                        <span class="badge badge-learning"><i class="fa-solid fa-chart-line"></i> Tecnologia em Gestão</span>
                    </div>
                </div>

            </div>
        </section>

        <!-- RODAPÉ -->
        <footer class="footer">
            <p>Vinicius Santos da Silva &copy; 2026 — Construindo a ponte entre TI e Logística.</p>
        </footer>

    </div>

</body>
</html>
