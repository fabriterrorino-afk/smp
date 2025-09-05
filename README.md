<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="SM Personalizados - Canecas de porcelana personalizadas. Faça seu orçamento pelo WhatsApp ou formulário."/>
  <title>SM Personalizados</title>
  <link rel="icon" href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUA... (exemplo)" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    /* ====== CSS (inline) ====== */
    :root{
      --rosa-claro: #FADADD;
      --rosa-medio: #E89AB4;
      --marrom: #A4756D;
      --texto: #333333;
      --fundo: #fff5f7;
      --radius: 14px;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:'Poppins',sans-serif;background:var(--fundo);color:var(--texto)}
    .container{max-width:1100px;margin:0 auto;padding:0 20px}
    .site-header{position:sticky;top:0;z-index:50;background:linear-gradient(180deg,var(--rosa-claro),var(--rosa-medio));box-shadow:0 2px 10px rgba(0,0,0,.04)}
    .header-wrap{display:flex;align-items:center;justify-content:space-between;padding:12px 0}
    .brand{display:flex;align-items:center;gap:.8rem;text-decoration:none;color:var(--texto)}
    .brand-text{font-weight:700;font-family:'Montserrat',sans-serif;font-size:1.25rem;color:var(--marrom)}
    .nav a{color:var(--marrom);text-decoration:none;font-weight:600;margin-left:16px}
    .nav a:hover{text-decoration:underline}
    .hero{padding:44px 0}
    .hero-grid{display:grid;grid-template-columns:1fr 460px;gap:28px;align-items:center}
    .hero-copy h1{font-family:'Montserrat',sans-serif;font-size:2.05rem;margin:0 0 10px;color:var(--marrom)}
    .hero-copy p{font-size:1.05rem;margin:0 0 16px}
    .btn{padding:12px 18px;border-radius:12px;font-weight:700;text-decoration:none;display:inline-block;font-family:'Montserrat',sans-serif}
    .btn.primary{background:var(--marrom);color:#fff}
    .btn.ghost{border:2px solid var(--marrom);color:var(--marrom)}
    .section{padding:48px 0}
    .section.gray{background:#fff}
    h2{font-family:'Montserrat',sans-serif;font-size:1.6rem;color:var(--marrom)}
    .cards{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .card{background:#fff;border-radius:var(--radius);padding:12px;box-shadow:0 4px 12px rgba(0,0,0,.08)}
    .card img{width:100%;height:160px;object-fit:cover;border-radius:10px;margin-bottom:10px}
    .card h3{margin:0 0 6px;font-size:1rem;color:var(--marrom)}
    .form{background:#fff;border-radius:16px;padding:16px;box-shadow:0 4px 16px rgba(0,0,0,.05)}
    input,select,textarea{width:100%;padding:10px;border:1px solid #ddd;border-radius:10px;font:inherit}
    .contact-list{list-style:none;padding:0;margin:0}
    .contact-list a{color:var(--marrom);font-weight:600;text-decoration:none}
    .site-footer{text-align:center;padding:22px 0;color:#666}
    .whatsapp-fab{position:fixed;right:18px;bottom:18px;height:56px;width:56px;border-radius:50%;background:#25D366;display:flex;align-items:center;justify-content:center}
    .whatsapp-fab img{height:28px;width:28px;filter:brightness(0) invert(1)}
    @media(max-width:800px){.hero-grid{grid-template-columns:1fr}.cards{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <header class="site-header">
    <div class="container header-wrap">
      <a href="#" class="brand">
        <img src="data:image/png;base64,{{LOGO_BASE64}}" alt="Logo SM Personalizados" style="height:56px;width:56px;border-radius:8px"/>
        <span class="brand-text">SM Personalizados</span>
      </a>
      <nav class="nav">
        <a href="#produtos">Produtos</a>
        <a href="#sobre">Sobre</a>
        <a href="#contato">Contato</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero container">
      <div class="hero-grid">
        <div class="hero-copy">
          <h1>Transforme suas ideias em canecas exclusivas</h1>
          <p>Canecas personalizadas em porcelana para presentes, empresas ou para tornar o seu dia mais especial.</p>
          <a class="btn primary" id="btnWhatsHero" href="#">Peça pelo WhatsApp</a>
        </div>
        <div>
          <img src="https://via.placeholder.com/400x280?text=Canecas" alt="Canecas personalizadas"/>
        </div>
      </div>
    </section>

    <section id="sobre" class="section gray">
      <div class="container">
        <h2>Sobre</h2>
        <p>Na SM Personalizados, transformamos suas ideias em canecas exclusivas e únicas. Trabalhamos com personalização de canecas de porcelana para presentear ou divulgar sua marca, ou simplesmente deixar o seu dia mais especial.</p>
        <p><strong>Valores:</strong> Criatividade • Qualidade • Exclusividade</p>
      </div>
    </section>

    <section id="produtos" class="section">
      <div class="container">
        <h2>Produtos</h2>
        <div class="cards">
          <div class="card">
            <img src="https://via.placeholder.com/300x160?text=Caneca+Clássica"/>
            <h3>Caneca Clássica 300ml</h3>
            <p>Porcelana branca 300ml, personalizável com sua arte.</p>
            <a class="btn primary" href="#" id="prod1">Pedir no WhatsApp</a>
          </div>
          <div class="card">
            <img src="https://via.placeholder.com/300x160?text=Caneca+Colorida"/>
            <h3>Caneca Colorida</h3>
            <p>Interior colorido e personalização externa vibrante.</p>
            <a class="btn primary" href="#" id="prod2">Pedir no WhatsApp</a>
          </div>
          <div class="card">
            <img src="https://via.placeholder.com/300x160?text=Caneca+Premium"/>
            <h3>Caneca Premium</h3>
            <p>Acabamento premium com brilho e alta durabilidade.</p>
            <a class="btn primary" href="#" id="prod3">Pedir no WhatsApp</a>
          </div>
        </div>
      </div>
    </section>

    <section id="contato" class="section gray">
      <div class="container">
        <h2>Contato</h2>
        <ul class="contact-list">
          <li><strong>WhatsApp:</strong> <a id="whatsLink" href="#">(51) 99140-0100</a></li>
          <li><strong>Instagram:</strong> <a href="https://www.instagram.com/sm_personalizadosltda" target="_blank">@sm_personalizadosltda</a></li>
          <li><strong>E-mail:</strong> <a href="mailto:contato@smpersonalizados.com.br">contato@smpersonalizados.com.br</a></li>
        </ul>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    © 2025 SM Personalizados — Todos os direitos reservados
  </footer>

  <a class="whatsapp-fab" id="btnWhatsFab" href="#">
    <img src="data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94..."/>
  </a>

  <script>
    // ====== JavaScript inline ======
    const WHATS_NUMBER = "5551991400100";
    function toWhatsLink(msg="Olá! Gostaria de um orçamento.") {
      return "https://wa.me/" + WHATS_NUMBER + "?text=" + encodeURIComponent(msg);
    }
    function initWhats() {
      document.getElementById("btnWhatsHero").href = toWhatsLink();
      document.getElementById("btnWhatsFab").href = toWhatsLink();
      document.getElementById("whatsLink").href = toWhatsLink();
      document.getElementById("prod1").href = toWhatsLink("Olá, quero a Caneca Clássica 300ml.");
      document.getElementById("prod2").href = toWhatsLink("Olá, quero a Caneca Colorida.");
      document.getElementById("prod3").href = toWhatsLink("Olá, quero a Caneca Premium.");
    }
    document.addEventListener("DOMContentLoaded", initWhats);
  </script>
</body>
</html>
