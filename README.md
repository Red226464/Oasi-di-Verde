<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Oasi di Verde | Plantas Premium & Decoração Natural</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<link rel="stylesheet" href="style.css">
  <style>
    /* Design System Unificado */
    :root {
      /* Cores */
      --verde-escuro: #3A5D3D;
      --verde: #4B7F52;
      --terracota: #C97F4F;
      --terracota-claro: #E3A87D;
      --bege: #F5F1E6;
      --cinza-escuro: #2D2D2A;
      --branco: #FFFFFF;
      
      /* Tipografia */
      --fonte-titulo: 'Playfair Display', serif;
      --fonte-texto: 'Poppins', sans-serif;
      
      /* Efeitos */
      --sombra: 0 4px 20px rgba(0,0,0,0.08);
      --borda-arredondada: 12px;
      --transicao: all 0.3s ease;
    }

    /* Reset & Base */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: var(--fonte-texto);
      color: var(--cinza-escuro);
      background-color: var(--bege);
      line-height: 1.6;
    }

    h1, h2, h3, h4 {
      font-family: var(--fonte-titulo);
      font-weight: 700;
      color: var(--verde-escuro);
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    img {
      max-width: 100%;
      height: auto;
      display: block;
    }

    .container {
      width: 100%;
      max-width: 1400px;
      margin: 0 auto;
      padding: 0 20px;
    }

    .btn {
      display: inline-block;
      padding: 12px 28px;
      border-radius: 50px;
      font-weight: 600;
      transition: var(--transicao);
      text-align: center;
      border: none;
      cursor: pointer;
    }

    .btn-primary {
      background-color: var(--terracota);
      color: var(--branco);
    }

    .btn-primary:hover {
      background-color: var(--terracota-claro);
      transform: translateY(-3px);
      box-shadow: var(--sombra);
    }

    .btn-secondary {
      background-color: var(--verde);
      color: var(--branco);
    }

    .btn-secondary:hover {
      background-color: var(--verde-escuro);
      transform: translateY(-3px);
      box-shadow: var(--sombra);
    }

    .destaque {
      color: var(--terracota);
    }

    /* Header - Versão Unificada */
    .main-header {
      background-color: var(--verde-escuro);
      color: var(--branco);
      padding: 15px 0;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }

    .header-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 28px;
      font-family: var(--fonte-titulo);
      font-weight: 700;
    }

    .logo span {
      color: var(--terracota);
    }

    .main-nav ul {
      display: flex;
      list-style: none;
      gap: 30px;
    }

    .main-nav a {
      font-weight: 500;
      transition: var(--transicao);
      position: relative;
    }

    .main-nav a:hover {
      color: var(--terracota);
    }

    .main-nav a:after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      background: var(--terracota);
      bottom: -5px;
      left: 0;
      transition: var(--transicao);
    }

    .main-nav a:hover:after {
      width: 100%;
    }

    .nav-icons {
      display: flex;
      gap: 20px;
    }

    .nav-icons a {
      font-size: 18px;
      transition: var(--transicao);
      position: relative;
    }

    .nav-icons a:hover {
      color: var(--terracota);
      transform: translateY(-2px);
    }

    .cart-count {
      background-color: var(--terracota);
      color: var(--branco);
      border-radius: 50%;
      width: 18px;
      height: 18px;
      font-size: 12px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      position: absolute;
      top: -8px;
      right: -8px;
    }

    /* Hero Section - Versão Unificada */
    .hero {
      height: 90vh;
      background: linear-gradient(rgba(58, 93, 61, 0.7), rgba(58, 93, 61, 0.7)), 
                  url('https://images.unsplash.com/photo-1487147264018-f937fba0c817?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1400&q=80') center/cover;
      color: var(--branco);
      display: flex;
      align-items: center;
      margin-top: 60px;
      text-align: center;
    }

    .hero-content {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
    }

    .hero h1 {
      font-size: 48px;
      margin-bottom: 20px;
      line-height: 1.2;
    }

    .hero p {
      margin-bottom: 30px;
      font-size: 18px;
      max-width: 600px;
      margin-left: auto;
      margin-right: auto;
    }

    .hero-btns {
      display: flex;
      gap: 15px;
      justify-content: center;
    }

    /* Seções - Versão Unificada */
    .section {
      padding: 80px 0;
    }

    .section-title {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title h2 {
      font-size: 36px;
      color: var(--verde-escuro);
      margin-bottom: 15px;
    }

    .section-title p {
      max-width: 700px;
      margin: 0 auto;
      color: var(--cinza-escuro);
    }

    /* Produtos em Destaque - Versão Unificada */
    .produtos-destaque {
      background-color: var(--branco);
    }

    .produtos-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 30px;
    }

    .produto-card {
      background: var(--branco);
      border-radius: var(--borda-arredondada);
      overflow: hidden;
      box-shadow: var(--sombra);
      transition: var(--transicao);
      position: relative;
    }

    .produto-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 15px 30px rgba(0,0,0,0.1);
    }

    .produto-badge {
      position: absolute;
      top: 15px;
      right: 15px;
      background-color: var(--terracota);
      color: var(--branco);
      padding: 5px 10px;
      border-radius: 4px;
      font-size: 12px;
      font-weight: 600;
    }

    .produto-img {
      height: 250px;
      width: 100%;
      object-fit: cover;
    }

    .produto-info {
      padding: 20px;
    }

    .produto-info h3 {
      margin-bottom: 8px;
      font-size: 18px;
      color: var(--verde-escuro);
    }

    .produto-info p {
      margin-bottom: 15px;
      color: var(--cinza-escuro);
    }

    .produto-meta {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .preco {
      font-weight: 700;
      color: var(--verde);
      font-size: 18px;
    }

    .preco-antigo {
      text-decoration: line-through;
      color: #999;
      font-size: 14px;
      margin-right: 5px;
    }

    .btn-carrinho {
      background-color: var(--verde);
      color: var(--branco);
      width: 40px;
      height: 40px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: var(--transicao);
    }

    .btn-carrinho:hover {
      background-color: var(--verde-escuro);
      transform: scale(1.1);
    }

    /* Galeria Inspiração - Versão Unificada */
    .galeria-inspiracao {
      background-color: var(--bege);
    }

    .galeria-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 20px;
    }

    .galeria-item {
      position: relative;
      border-radius: var(--borda-arredondada);
      overflow: hidden;
      box-shadow: var(--sombra);
      transition: var(--transicao);
      height: 300px;
    }

    .galeria-item:hover {
      transform: scale(1.03);
    }

    .galeria-img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .galeria-overlay {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      background: linear-gradient(to top, rgba(0,0,0,0.7), transparent);
      padding: 20px;
      color: var(--branco);
      opacity: 0;
      transition: var(--transicao);
    }

    .galeria-item:hover .galeria-overlay {
      opacity: 1;
    }

    /* Depoimentos - Versão Unificada */
    .depoimentos-section {
      background-color: var(--branco);
    }

    .depoimentos-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 30px;
    }

    .depoimento-card {
      background-color: var(--bege);
      padding: 30px;
      border-radius: var(--borda-arredondada);
      box-shadow: var(--sombra);
    }

    .depoimento-texto {
      font-style: italic;
      margin-bottom: 20px;
      position: relative;
    }

    .depoimento-texto:before,
    .depoimento-texto:after {
      content: '"';
      font-size: 24px;
      color: var(--terracota);
    }

    .depoimento-autor {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .depoimento-foto {
      width: 60px;
      height: 60px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid var(--terracota);
    }

    .autor-info h4 {
      margin-bottom: 5px;
      color: var(--verde-escuro);
    }

    .autor-info p {
      color: var(--cinza-escuro);
      font-size: 14px;
    }

    .avaliacao {
      color: var(--terracota);
      margin-top: 5px;
    }

    /* Newsletter - Versão Unificada */
    .newsletter-section {
      background-color: var(--verde-escuro);
      color: var(--branco);
      padding: 60px 0;
      text-align: center;
    }

    .newsletter-form {
      max-width: 600px;
      margin: 0 auto;
      display: flex;
      background-color: var(--branco);
      border-radius: 50px;
      overflow: hidden;
    }

    .newsletter-input {
      flex: 1;
      padding: 15px 25px;
      border: none;
      font-size: 16px;
    }

    .newsletter-btn {
      background-color: var(--terracota);
      color: var(--branco);
      border: none;
      padding: 0 30px;
      font-weight: 600;
      cursor: pointer;
      transition: var(--transicao);
    }

    .newsletter-btn:hover {
      background-color: var(--terracota-claro);
    }

    /* Footer - Versão Unificada */
    .main-footer {
      background-color: var(--cinza-escuro);
      color: var(--branco);
      padding: 60px 0 30px;
    }

    .footer-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 40px;
      margin-bottom: 40px;
    }

    .footer-logo {
      font-size: 24px;
      font-family: var(--fonte-titulo);
      margin-bottom: 20px;
      display: block;
    }

    .footer-logo span {
      color: var(--terracota);
    }

    .footer-about p {
      margin-bottom: 20px;
      color: #ccc;
    }

    .social-links {
      display: flex;
      gap: 15px;
    }

    .social-links a {
      width: 40px;
      height: 40px;
      background-color: rgba(255,255,255,0.1);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: var(--transicao);
      color: var(--branco);
    }

    .social-links a:hover {
      background-color: var(--terracota);
      transform: translateY(-3px);
    }

    .footer-links h3 {
      color: var(--branco);
      margin-bottom: 20px;
      font-size: 18px;
    }

    .footer-links ul {
      list-style: none;
    }

    .footer-links li {
      margin-bottom: 10px;
    }

    .footer-links a {
      transition: var(--transicao);
      color: #ccc;
    }

    .footer-links a:hover {
      color: var(--terracota);
      padding-left: 5px;
    }

    .footer-contact p {
      display: flex;
      align-items: center;
      gap: 10px;
      margin-bottom: 15px;
      color: #ccc;
    }

    .copyright {
      text-align: center;
      padding-top: 30px;
      border-top: 1px solid rgba(255,255,255,0.1);
      color: #999;
      font-size: 14px;
    }

    /* Botão Voltar ao Topo */
    .back-to-top {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: var(--terracota);
      color: var(--branco);
      border: none;
      width: 50px;
      height: 50px;
      border-radius: 50%;
      cursor: pointer;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      font-weight: bold;
      transition: var(--transicao);
      display: none;
      justify-content: center;
      align-items: center;
      z-index: 999;
    }

    .back-to-top.visible {
      display: flex;
    }

    .back-to-top:hover {
      background-color: var(--terracota-claro);
      transform: translateY(-3px);
    }

    /* Responsividade */
    @media (max-width: 992px) {
      .hero h1 {
        font-size: 40px;
      }
      
      .section-title h2 {
        font-size: 32px;
      }
    }

    @media (max-width: 768px) {
      .main-nav {
        display: none;
        position: fixed;
        top: 80px;
        left: 0;
        right: 0;
        background-color: var(--verde-escuro);
        padding: 20px;
        box-shadow: 0 10px 20px rgba(0,0,0,0.1);
      }
      
      .main-nav.active {
        display: block;
      }
      
      .main-nav ul {
        flex-direction: column;
        gap: 15px;
      }
      
      .menu-toggle {
        display: block !important;
        font-size: 24px;
        cursor: pointer;
      }
      
      .hero h1 {
        font-size: 36px;
      }
      
      .hero-btns {
        flex-direction: column;
        align-items: center;
      }
      
      .newsletter-form {
        flex-direction: column;
        background-color: transparent;
      }
      
      .newsletter-input {
        border-radius: 50px;
        margin-bottom: 10px;
      }
      
      .newsletter-btn {
        border-radius: 50px;
        padding: 15px;
      }
    }

    @media (max-width: 576px) {
      .hero h1 {
        font-size: 32px;
      }
      
      .section {
        padding: 60px 0;
      }
      
      .section-title h2 {
        font-size: 28px;
      }
    }
  </style>
</head>
<body>
  <!-- Header -->
  <header class="main-header">
    <div class="container header-container">
      <a href="index.html" class="logo">Oasi<span>diVerde</span></a>
      
      <nav class="main-nav">
        <ul>
          <li><a href="index.html">Início</a></li>
          <li><a href="produtos.html">Produtos</a></li>
          <li><a href="galeria.html">Galeria</a></li>
          <li><a href="blog.html">Blog</a></li>
          <li><a href="sobre.html">Sobre</a></li>
          <li><a href="contato.html">Contato</a></li>
        </ul>
      </nav>
      
      <div class="nav-icons">
        <a href="#"><i class="fas fa-search"></i></a>
        <a href="login.html"><i class="fas fa-user"></i></a>
        <a href="carrinho.html" class="cart-icon">
          <i class="fas fa-shopping-cart"></i>
          <span class="cart-count">2</span>
        </a>
        <div class="menu-toggle" style="display: none;">
          <i class="fas fa-bars"></i>
        </div>
      </div>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div class="container">
      <div class="hero-content">
        <h1>Transforme seu espaço em um <span class="destaque">oásis verde</span></h1>
        <p>Descubra nossa coleção exclusiva de plantas e acessórios para criar ambientes naturais e cheios de vida.</p>
        <div class="hero-btns">
          <a href="produtos.html" class="btn btn-primary">Explorar Produtos</a>
          <a href="galeria.html" class="btn btn-secondary">Inspirações</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Produtos em Destaque -->
  <section class="section produtos-destaque">
    <div class="container">
      <div class="section-title">
        <h2>Nossos <span class="destaque">Destaques</span></h2>
        <p>Conheça os produtos mais amados pelos nossos clientes</p>
      </div>
      
      <div class="produtos-grid">
        <!-- Produto 1 -->
        <div class="produto-card">
          <span class="produto-badge">Mais Vendido</span>
          <img src="https://i.postimg.cc/mrTqD2Y8/arranjo-de-pendente-jiboia-com-vaso-de-ceramica-preto-zigzag-4445-1-7325929c4997537f755779c7fd01faa2.webp" alt="Jiboia no Vaso Cerâmico" class="produto-img">
          <div class="produto-info">
            <h3>Jiboia no Vaso Cerâmico</h3>
            <p>Planta pendente perfeita para interiores</p>
            <div class="produto-meta">
              <div class="preco">
                <span class="preco-antigo">R$ 149,90</span>
                R$ 129,90
              </div>
              <button class="btn-carrinho">
                <i class="fas fa-plus"></i>
              </button>
            </div>
          </div>
        </div>
        
        <!-- Produto 2 -->
        <div class="produto-card">
          <img src="https://i.postimg.cc/gJsGJTL6/173638257d-1.webp" alt="Espada de São Jorge Mini" class="produto-img">
          <div class="produto-info">
            <h3>Espada de São Jorge Mini</h3>
            <p>Purificadora de ar e resistente</p>
            <div class="produto-meta">
              <div class="preco">R$ 39,90</div>
              <button class="btn-carrinho">
                <i class="fas fa-plus"></i>
              </button>
            </div>
          </div>
        </div>
        
        <!-- Produto 3 -->
        <div class="produto-card">
          <span class="produto-badge">Novidade</span>
          <img src="https://i.postimg.cc/bwZ0RXzp/sg-11134201-22110-nbb2qwwrdcjvf0.jpg" alt="Vaso Terracota Decorado" class="produto-img">
          <div class="produto-info">
            <h3>Vaso Terracota Decorado</h3>
            <p>Padrões exclusivos artesanais</p>
            <div class="produto-meta">
              <div class="preco">R$ 109,00</div>
              <button class="btn-carrinho">
                <i class="fas fa-plus"></i>
              </button>
            </div>
          </div>
        </div>
        
        <!-- Produto 4 -->
        <div class="produto-card">
          <img src="imagens/20250605_1443_Kit de Suculentas_simple_compose_01jx0jzkysf8gtxct9gj5zsh8c.png" alt="Mini Suculenta no Vidro" class="produto-img">
          <div class="produto-info">
            <h3>Mini Suculenta no Vidro</h3>
            <p>Kit presente com 3 variedades</p>
            <div class="produto-meta">
              <div class="preco">R$ 79,90</div>
              <button class="btn-carrinho">
                <i class="fas fa-plus"></i>
              </button>
            </div>
          </div>
        </div>
      </div>
      
      <div style="text-align: center; margin-top: 40px;">
        <a href="produtos.html" class="btn btn-secondary">Ver Todos os Produtos</a>
      </div>
    </div>
  </section>

  <!-- Galeria de Inspiração -->
  <section class="section galeria-inspiracao">
    <div class="container">
      <div class="section-title">
        <h2>Inspire-se com <span class="destaque">Nossas Criações</span></h2>
        <p>Veja como nossas plantas podem transformar ambientes</p>
      </div>
      
      <div class="galeria-grid">
        <div class="galeria-item">
          <img src="imagens/20250605_1500_Sala de Estar Verdejante_simple_compose_01jx0ky7p4fxv852wvr4my7p9h.png" alt="Sala de estar com plantas" class="galeria-img">
          <div class="galeria-overlay">
            <h3>Sala de Estar Verdejante</h3>
            <p>Combinação de jiboia e samambaias</p>
          </div>
        </div>
        
        <div class="galeria-item">
          <img src="imagens/20250605_1551_Escritório Verde Produtivo_simple_compose_01jx0pt030em7syvz9rv2cs9bt.png" alt="Escritório com plantas" class="galeria-img">
          <div class="galeria-overlay">
            <h3>Escritório Natural</h3>
            <p>Plantas que melhoram a produtividade</p>
          </div>
        </div>
        
        <div class="galeria-item">
         <img src="imagens/20250605_1457_Varanda com Suculentas_simple_compose_01jx0kqykgfvm8ttgvk04c1xm6.png" alt="Escritório com plantas" class="galeria-img">
          <div class="galeria-overlay">
            <h3>Varanda Aconchegante</h3>
            <p>Vasos de terracota e suculentas</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Depoimentos -->
  <section class="section depoimentos-section">
    <div class="container">
      <div class="section-title">
        <h2>O que dizem <span class="destaque">Nossos Clientes</span></h2>
        <p>Veja a experiência de quem já transformou seus ambientes</p>
      </div>
      
      <div class="depoimentos-container">
        <!-- Depoimento 1 -->
        <div class="depoimento-card">
          <div class="depoimento-texto">
            Minha casa ficou muito mais aconchegante depois que comprei minhas plantas na Oasi di Verde. O atendimento foi incrível e me ajudaram a escolher as espécies perfeitas para cada ambiente.
          </div>
          <div class="depoimento-autor">
            <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Maria Clara" class="depoimento-foto">
            <div class="autor-info">
              <h4>Maria Clara</h4>
              <p>São Paulo, SP</p>
              <div class="avaliacao">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
              </div>
            </div>
          </div>
        </div>
        
        <!-- Depoimento 2 -->
        <div class="depoimento-card">
          <div class="depoimento-texto">
            Produtos lindos e de ótima qualidade! Super recomendo para quem ama plantas. A entrega foi rápida e tudo muito bem embalado. Amei meus vasos novos!
          </div>
          <div class="depoimento-autor">
            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="João Pedro" class="depoimento-foto">
            <div class="autor-info">
              <h4>João Pedro</h4>
              <p>Belo Horizonte, MG</p>
              <div class="avaliacao">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Newsletter -->
  <section class="newsletter-section">
    <div class="container">
      <h2>Receba Nossas Novidades</h2>
      <p>Assine nossa newsletter e receba dicas exclusivas, promoções e inspirações para seu espaço verde</p>
      
      <form class="newsletter-form">
        <input type="email" placeholder="Seu melhor e-mail" class="newsletter-input" required>
        <button type="submit" class="newsletter-btn">Assinar</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer class="main-footer">
    <div class="container">
      <div class="footer-container">
        <div class="footer-about">
          <a href="index.html" class="footer-logo">Oasi<span>diVerde</span></a>
          <p>Transformando ambientes através da natureza desde 2018. Plantas premium e acessórios para criar seu oásis particular.</p>
          
          <div class="social-links">
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-pinterest-p"></i></a>
            <a href="#"><i class="fab fa-youtube"></i></a>
          </div>
        </div>
        
        <div class="footer-links">
          <h3>Links Rápidos</h3>
          <ul>
            <li><a href="index.html">Início</a></li>
            <li><a href="produtos.html">Produtos</a></li>
            <li><a href="galeria.html">Galeria</a></li>
            <li><a href="blog.html">Blog</a></li>
            <li><a href="sobre.html">Sobre Nós</a></li>
            <li><a href="contato.html">Contato</a></li>
          </ul>
        </div>
        
        <div class="footer-links">
          <h3>Categorias</h3>
          <ul>
            <li><a href="produtos.html?categoria=plantas-interior">Plantas de Interior</a></li>
            <li><a href="produtos.html?categoria=plantas-exterior">Plantas de Exterior</a></li>
            <li><a href="produtos.html?categoria=vasos">Vasos Decorativos</a></li>
            <li><a href="produtos.html?categoria=kits">Kits Presente</a></li>
            <li><a href="produtos.html?categoria=acessorios">Acessórios</a></li>
            <li><a href="produtos.html?categoria=novidades">Novidades</a></li>
          </ul>
        </div>
        
        <div class="footer-contact">
          <h3>Contato</h3>
          <p><i class="fas fa-map-marker-alt"></i> Rua das Flores, 123 - Jardim Botânico, Curitiba/PR</p>
          <p><i class="fas fa-phone"></i> (41) 99999-9999</p>
          <p><i class="fas fa-envelope"></i> contato@oasidiverde.com.br</p>
          <p><i class="fas fa-clock"></i> Seg-Sex: 9h às 18h | Sáb: 9h às 13h</p>
        </div>
      </div>
      
      <div class="copyright">
        <p>&copy; 2023 Oasi di Verde. Todos os direitos reservados. | Desenvolvido com <i class="fas fa-heart" style="color: var(--terracota);"></i> por sua equipe</p>
      </div>
    </div>
  </footer>

  <!-- Botão Voltar ao Topo -->
  <button class="back-to-top" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">
    <i class="fas fa-arrow-up"></i>
  </button>

  <script>
    // Menu Mobile
    document.addEventListener('DOMContentLoaded', function() {
      const menuToggle = document.querySelector('.menu-toggle');
      const mainNav = document.querySelector('.main-nav');
      
      menuToggle.addEventListener('click', function() {
        mainNav.classList.toggle('active');
      });
      
      // Botão voltar ao topo
      const backToTopButton = document.querySelector('.back-to-top');
      
      window.addEventListener('scroll', function() {
        if (window.scrollY > 300) {
          backToTopButton.classList.add('visible');
        } else {
          backToTopButton.classList.remove('visible');
        }
      });
      
      // Adicionar ao carrinho
      const addToCartButtons = document.querySelectorAll('.btn-carrinho');
      const cartCount = document.querySelector('.cart-count');
      
      addToCartButtons.forEach(button => {
        button.addEventListener('click', function() {
          // Animação do botão
          this.innerHTML = '<i class="fas fa-check"></i>';
          setTimeout(() => {
            this.innerHTML = '<i class="fas fa-plus"></i>';
          }, 1000);
          
          // Atualizar contador do carrinho
          let count = parseInt(cartCount.textContent);
          cartCount.textContent = count + 1;
          
          // Feedback visual
          cartCount.style.transform = 'scale(1.5)';
          setTimeout(() => {
            cartCount.style.transform = 'scale(1)';
          }, 300);
        });
      });
    });
  </script>
</body>
</html>
