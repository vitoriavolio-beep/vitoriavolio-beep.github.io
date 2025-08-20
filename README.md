# vitoriavolio-beep.github.io
index.html
```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dra. Maria Vitória Bello Avolio | Especialista em Endodontia</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #9b7a5d;
            --secondary-color: #c9a77c;
            --light-color: #f8f9fa;
            --dark-color: #333333;
            --white: #ffffff;
            --light-gray: #f0f0f0;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            color: var(--dark-color);
            background-color: var(--light-color);
            line-height: 1.6;
            position: relative;
        }
        
        h1, h2, h3, h4, h5 {
            font-family: 'Playfair Display', serif;
            font-weight: 600;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* WhatsApp Button */
        .whatsapp-float {
            position: fixed;
            width: 60px;
            height: 60px;
            bottom: 40px;
            right: 40px;
            background-color: #25D366;
            color: #FFF;
            border-radius: 50px;
            text-align: center;
            font-size: 30px;
            box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
            z-index: 100;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            animation: pulse 2s infinite;
        }
        
        .whatsapp-float:hover {
            transform: scale(1.1);
            box-shadow: 2px 2px 15px rgba(0,0,0,0.3);
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        /* Header */
        header {
            background-color: var(--white);
            box-shadow: 0 2px 15px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 24px;
            font-weight: 700;
            color: var(--primary-color);
        }
        
        .logo span {
            color: var(--secondary-color);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark-color);
            font-weight: 500;
            transition: color 0.3s ease;
        }
        
        nav ul li a:hover {
            color: var(--primary-color);
        }
        
        /* Hero Section */
        .hero {
            padding: 160px 0 100px;
            background-color: var(--white);
            position: relative;
            overflow: hidden;
        }
        
        .hero-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .hero-text {
            flex: 1;
        }
        
        .hero-text h1 {
            font-size: 48px;
            line-height: 1.2;
            margin-bottom: 20px;
            color: var(--primary-color);
        }
        
        .hero-text h1 span {
            color: var(--secondary-color);
        }
        
        .hero-text p {
            font-size: 18px;
            margin-bottom: 30px;
            color: var(--dark-color);
        }
        
        .hero-image {
            flex: 1;
            text-align: center;
        }
        
        .hero-image img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: var(--white);
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: var(--secondary-color);
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        /* About Section */
        .about {
            padding: 100px 0;
            background-color: var(--white);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            font-size: 36px;
            color: var(--primary-color);
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: var(--secondary-color);
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-image {
            flex: 1;
        }
        
        .about-image img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            font-size: 24px;
            margin-bottom: 20px;
            color: var(--primary-color);
        }
        
        .about-text p {
            margin-bottom: 20px;
        }
        
        .credentials {
            margin-top: 30px;
        }
        
        .credential-item {
            display: flex;
            margin-bottom: 15px;
        }
        
        .credential-item::before {
            content: '✚';
            color: var(--secondary-color);
            font-weight: bold;
            margin-right: 10px;
        }
        
        /* Services Section */
        .services {
            padding: 100px 0;
            background-color: var(--white);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }
        
        .service-card {
            background-color: var(--light-gray);
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
        }
        
        .service-card h3 {
            font-size: 22px;
            margin-bottom: 15px;
            color: var(--primary-color);
        }
        
        .service-card p {
            color: var(--dark-color);
        }
        
        /* Testimonials */
        .testimonials {
            padding: 100px 0;
            background-color: var(--white);
        }
        
        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }
        
        .testimonial-card {
            background-color: var(--light-gray);
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            position: relative;
        }
        
        .testimonial-card::before {
            content: '"';
            position: absolute;
            top: 10px;
            left: 20px;
            font-size: 80px;
            color: var(--secondary-color);
            opacity: 0.2;
            font-family: 'Playfair Display', serif;
        }
        
        .testimonial-content {
            position: relative;
            z-index: 1;
        }
        
        .testimonial-content p {
            margin-bottom: 20px;
            font-style: italic;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .testimonial-author img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 15px;
        }
        
        .author-info h4 {
            font-size: 18px;
            margin-bottom: 5px;
        }
        
        .author-info span {
            color: #666;
            font-size: 14px;
        }
        
        .trustindex {
            font-size: 12px;
            color: #666;
            margin-top: 10px;
            font-style: italic;
        }
        
        /* Contact Section */
        .contact {
            padding: 100px 0;
            background-color: var(--white);
        }
        
        .contact-content {
            display: flex;
            gap: 50px;
        }
        
        .contact-info {
            flex: 1;
        }
        
        .contact-info h3 {
            font-size: 24px;
            margin-bottom: 20px;
            color: var(--primary-color);
        }
        
        .info-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 20px;
        }
        
        .info-item i {
            color: var(--secondary-color);
            margin-right: 15px;
            margin-top: 5px;
        }
        
        .info-text h4 {
            font-size: 18px;
            margin-bottom: 5px;
        }
        
        .map {
            flex: 1;
            height: 400px;
            border-radius: 10px;
            overflow: hidden;
        }
        
        .map iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
        
        /* Footer */
        footer {
            background-color: var(--primary-color);
            color: var(--white);
            padding: 60px 0 30px;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-between;
            margin-bottom: 40px;
        }
        
        .footer-column {
            flex: 1;
        }
        
        .footer-column h3 {
            font-size: 20px;
            margin-bottom: 20px;
            color: var(--white);
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: rgba(255,255,255,0.8);
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-column ul li a:hover {
            color: var(--white);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: rgba(255,255,255,0.6);
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 992px) {
            .hero-content, .about-content, .contact-content {
                flex-direction: column;
            }
            
            .hero {
                padding: 140px 0 80px;
            }
            
            .hero-text h1 {
                font-size: 36px;
            }
            
            .whatsapp-float {
                bottom: 20px;
                right: 20px;
                width: 50px;
                height: 50px;
                font-size: 24px;
            }
        }
        
        @media (max-width: 768px) {
            nav ul {
                display: none;
            }
            
            .section-title h2 {
                font-size: 28px;
            }
        }
    </style>
</head>
<body>
    <!-- WhatsApp Button -->
    <a href="https://wa.me/5511994802149" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">Dra. Maria Vitória <span>Bello Avolio</span></div>
                <nav>
                    <ul>
                        <li><a href="#inicio">Início</a></li>
                        <li><a href="#sobre">Sobre</a></li>
                        <li><a href="#tratamentos">Tratamentos</a></li>
                        <li><a href="#depoimentos">Depoimentos</a></li>
                        <li><a href="#contato">Contato</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="inicio">
        <div class="container">
            <div class="hero-content">
                <div class="hero-text">
                    <h1>Especialista em <span>Endodontia</span><br>em São Paulo - SP</h1>
                    <p>É uma alegria poder cuidar da saúde do seu sorriso, preservando seus dentes naturais com técnicas modernas e precisas. Sou a Dra. Maria Vitória Bello Avolio, especialista em Endodontia com formação e experiência dedicadas ao alívio da dor e à preservação dos dentes.</p>
                    <p>Meu objetivo é proporcionar um tratamento humanizado, com tecnologia de ponta e atenção aos detalhes, para que você possa sorrir com confiança e conforto.</p>
                    <a href="#contato" class="btn">Agende sua consulta</a>
                </div>
                <div class="hero-image">
                    <img src="https://via.placeholder.com/500x600/f5f2ec/9b7a5d?text=Dra.+Maria+Vitória" alt="Dra. Maria Vitória Bello Avolio">
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="sobre">
        <div class="container">
            <div class="section-title">
                <h2>Conheça a Especialista</h2>
            </div>
            <div class="about-content">
                <div class="about-image">
                    <img src="https://via.placeholder.com/500x600/f5f2ec/9b7a5d?text=Consultório" alt="Consultório Dra. Maria Vitória">
                </div>
                <div class="about-text">
                    <h3>Dra. Maria Vitória Bello Avolio</h3>
                    <p>Formada em Odontologia pela Universidade Estadual de Campinas (UNICAMP) e especialista em Endodontia pela Faculdade São Leopoldo Mandic, dedico minha carreira ao tratamento de canal e à preservação dos dentes naturais. Acredito que cada paciente merece um atendimento personalizado, com empatia e profissionalismo.</p>
                    <p>A Endodontia é uma área que exige precisão, paciência e cuidado extremo. Utilizo tecnologia moderna, como microscópio operatório e sistemas de instrumentação rotatória, para garantir tratamentos mais confortáveis, eficientes e com maior taxa de sucesso.</p>
                    <p>Meu consultório está equipado com os mais modernos recursos para proporcionar segurança e conforto durante todo o procedimento. Acredito que confiança, transparência e bem-estar são tão importantes quanto técnica e experiência.</p>
                    
                    <div class="credentials">
                        <div class="credential-item">Formada em Odontologia pela UNICAMP</div>
                        <div class="credential-item">Especialista em Endodontia pela Faculdade São Leopoldo Mandic</div>
                        <div class="credential-item">Utilização de microscópio operatório para maior precisão</div>
                        <div class="credential-item">Técnicas modernas de anestesia para maior conforto</div>
                        <div class="credential-item">Tratamento de canal em uma única sessão quando possível</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="tratamentos">
        <div class="container">
            <div class="section-title">
                <h2>Tratamentos de Endodontia</h2>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <h3>Tratamento de Canal com Microscópio</h3>
                    <p>Procedimento para salvar dentes com polpa dental inflamada ou infectada. Utilizo microscópio operatório para maior precisão e sucesso do tratamento, garantindo visualização ampliada dos canais radiculares.</p>
                </div>
                <div class="service-card">
                    <h3>Retratamento Endodôntico</h3>
                    <p>Quando um tratamento de canal anterior não obteve sucesso, realizo o retratamento para limpar novamente os canais e salvar o dente natural, utilizando tecnologia avançada.</p>
                </div>
                <div class="service-card">
                    <h3>Cirurgia Paraendodôntica</h3>
                    <p>Procedimento cirúrgico para tratar infecções na ponta da raiz quando o tratamento convencional não é suficiente, com mínima invasão e rápida recuperação.</p>
                </div>
                <div class="service-card">
                    <h3>Limpeza Dental</h3>
                    <p>Procedimento profissional para remover placa bacteriana, tártaro e manchas, prevenindo doenças gengivais e mantendo a saúde bucal em dia.</p>
                </div>
                <div class="service-card">
                    <h3>Atendimento de Urgência</h3>
                    <p>Alívio imediato de dores intensas causadas por problemas endodônticos, com agendamento prioritário para emergências e tratamento eficaz.</p>
                </div>
                <div class="service-card">
                    <h3>Restaurações em Resina</h3>
                    <p>Reconstrução estética e funcional de dentes danificados, utilizando resinas compostas de alta qualidade que se integram perfeitamente à estrutura dental.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials" id="depoimentos">
        <div class="container">
            <div class="section-title">
                <h2>Pacientes Satisfeitos</h2>
            </div>
            <div class="testimonials-grid">
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        <p>Atendimento impecável da Dra Maria Vitória! Fiz um tratamento muito bem sucedido, me senti muito acolhida e nas mãos de uma boa profissional! Recomendo muito!</p>
                        <div class="testimonial-author">
                            <img src="https://via.placeholder.com/50x50/f5f2ec/9b7a5d?text=AS" alt="Aline Sousa">
                            <div class="author-info">
                                <h4>Aline Sousa</h4>
                                <span>9 meses atrás</span>
                            </div>
                        </div>
                        <div class="trustindex">Trustindex verifica se a fonte original da avaliação é Google.</div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        <p>Excelente profissional, com excelentes equipamentos, clínica limpa e organizada. Super recomendo, preços acessíveis e super bem pagos pelo trabalho e profissionalismo da doutora, já cheguei na clínica com muita dor e após cirurgia saí da lá com sentir nada</p>
                        <div class="testimonial-author">
                            <img src="https://via.placeholder.com/50x50/f5f2ec/9b7a5d?text=SR" alt="Stephanny Rosendo">
                            <div class="author-info">
                                <h4>Stephanny Rosendo</h4>
                                <span>11 meses atrás</span>
                            </div>
                        </div>
                        <div class="trustindex">Trustindex verifica se a fonte original da avaliação é Google.</div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        <p>Tive uma ótima experiência na clínica. A Dra Maria Vitória me atendeu prontamente, explicou com detalhes a situação do meu dente e o procedimento a ser realizado. Foi super atenciosa. Ela tem uma mão super leve no tratamento e foi explicando o passo a passo para que me sentisse segura e confortável. A clínica é muito bem montada e com uma higiene impecável!!! Adorei!</p>
                        <div class="testimonial-author">
                            <img src="https://via.placeholder.com/50x50/f5f2ec/9b7a5d?text=FF" alt="Fernanda Faria">
                            <div class="author-info">
                                <h4>Fernanda Faria</h4>
                                <span>um ano atrás</span>
                            </div>
                        </div>
                        <div class="trustindex">Trustindex verifica se a fonte original da avaliação é Google.</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contato">
        <div class="container">
            <div class="section-title">
                <h2>Entre em Contato</h2>
            </div>
            <div class="contact-content">
                <div class="contact-info">
                    <h3>Consultório</h3>
                    <div class="info-item">
                        <i class="fas fa-map-marker-alt"></i>
                        <div class="info-text">
                            <h4>Endereço</h4>
                            <p>Av. Nove de Julho, 3229 - Conjunto 1506<br>São Paulo - SP, 01407-200</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <i class="fas fa-phone-alt"></i>
                        <div class="info-text">
                            <h4>Telefone</h4>
                            <p>(11) 99480-2149</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <i class="fas fa-envelope"></i>
                        <div class="info-text">
                            <h4>E-mail</h4>
                            <p>avolio.odonto@gmail.com</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <i class="fas fa-clock"></i>
                        <div class="info-text">
                            <h4>Horários</h4>
                            <p>Segunda a Sexta: 8h às 19h<br>Sábado: 8h às 14h</p>
                        </div>
                    </div>
                    <a href="https://wa.me/5511994802149" class="btn">Agendar pelo WhatsApp</a>
                </div>
                <div class="map">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3657.264153027319!2d-46.66647568502149!3d-23.56058898467856!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce59c8da0aa315%3A0xd59f9430485749f3!2sAv.%20Paulista%2C%201009%20-%20Bela%20Vista%2C%20S%C3%A3o%20Paulo%20-%20SP%2C%2001311-100!5e0!3m2!1spt-BR!2sbr!4v1619824567897!5m2!1spt-BR!2sbr" allowfullscreen="" loading="lazy"></iframe>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Dra. Maria Vitória Bello Avolio</h3>
                    <p>Especialista em Endodontia dedicada à preservação dos dentes naturais com técnicas modernas e humanizadas.</p>
                </div>
                <div class="footer-column">
                    <h3>Atendimento</h3>
                    <ul>
                        <li><a href="#">Tratamento de Canal com Microscópio</a></li>
                        <li><a href="#">Retratamento Endodôntico</a></li>
                        <li><a href="#">Cirurgia Paraendodôntica</a></li>
                        <li><a href="#">Atendimento de Urgência</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contato</h3>
                    <ul>
                        <li><a href="tel:+5511994802149">(11) 99480-2149</a></li>
                        <li><a href="mailto:avolio.odonto@gmail.com">avolio.odonto@gmail.com</a></li>
                        <li><a href="#">Agendar Consulta</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2024 Dra. Maria Vitória Bello Avolio. Todos os direitos reservados. | CRO: [Número do CRO]</p>
            </div>
        </div>
    </footer>
</body>
</html>
```
