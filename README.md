<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="SM Personalizados - Canecas de porcelana personalizadas. Faça seu orçamento pelo WhatsApp ou formulário."/>
  <title>SM Personalizados</title>
  <link rel="icon" href="/assets/favicon.ico" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="/assets/style.css" />
  <script defer src="/assets/script.js"></script>
</head>
<body>
  <header class="site-header">
    <div class="container header-wrap">
      <a href="#" class="brand">
        <img src="/assets/logo.png" alt="Logo SM Personalizados" class="logo" />
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
          <p>Na SM Personalizados, criamos canecas únicas para presentes, eventos e brindes corporativos. Personalização em porcelana com acabamento de alta qualidade.</p>
          <div class="cta-group">
            <a class="btn primary" id="btnWhatsHero" href="#">Pedir pelo WhatsApp</a>
            <a class="btn ghost" href="#produtos">Ver produtos</a>
          </div>
          <div class="trust">
            <span class="small">Criatividade</span>
            <span class="small">Qualidade</span>
            <span class="small">Exclusividade</span>
          </div>
        </div>
        <div class="hero-art">
          <img src="/assets/hero-mugs.png" alt="Conjunto de canecas personalizadas" />
        </div>
      </div>
    </section>

    <section id="sobre" class="section">
      <div class="container">
        <h2>Sobre</h2>
        <p>“Na SM Personalizados, transformamos suas ideias em canecas exclusivas e únicas. Trabalhamos com personalização de canecas de porcelana para presentear ou divulgar sua marca, ou simplesmente deixar o seu dia mais especial.”</p>
        <p class="small"><strong>Valores:</strong> Criatividade • Qualidade • Exclusividade</p>
      </div>
    </section>

    <section id="produtos" class="section gray">
      <div class="container">
        <h2>Produtos</h2>
        <div class="category-tabs" role="tablist" aria-label="Categorias">
          <button class="tab active" data-cat="todos">Todos</button>
          <button class="tab" data-cat="empresas">Para Empresas</button>
          <button class="tab" data-cat="presentes">Para Presentes</button>
          <button class="tab" data-cat="tematicas">Temáticas</button>
        </div>

        <div class="cards" id="cardsArea">
          <!-- Product cards inserted by JS for flexibility -->
        </div>

        <h3 style="margin-top:22px">Galeria</h3>
        <div class="gallery" id="galleryArea">
          <!-- gallery images inserted by JS -->
        </div>
      </div>
    </section>

    <section id="orcamento" class="section">
      <div class="container">
        <h2>Orçamento rápido</h2>
        <form id="quoteForm" class="form" enctype="multipart/form-data">
          <div class="grid">
            <div class="form-field">
              <label for="nome">Nome</label>
              <input id="nome" name="nome" type="text" placeholder="Seu nome" required/>
            </div>
            <div class="form-field">
              <label for="telefone">Telefone / WhatsApp</label>
              <input id="telefone" name="telefone" type="tel" placeholder="(51) 99140-0100" required/>
            </div>
            <div class="form-field">
              <label for="produto">Tipo</label>
              <select id="produto" name="produto">
                <option>Caneca Clássica 300ml</option>
                <option>Caneca Colorida</option>
                <option>Caneca Premium</option>
              </select>
            </div>
            <div class="form-field">
              <label for="quantidade">Quantidade</label>
              <input id="quantidade" name="quantidade" type="number" min="1" value="1" required/>
            </div>
          </div>
          <div class="form-field">
            <label for="mensagem">Mensagem</label>
            <textarea id="mensagem" name="mensagem" rows="3" placeholder="Conte sua ideia, prazo e cores"></textarea>
          </div>
          <div class="form-field">
            <label for="arquivo">Anexar arte (opcional)</label>
            <input id="arquivo" name="arquivo" type="file" accept=".png,.jpg,.jpeg,.pdf" />
          </div>
          <button class="btn primary" type="submit">Enviar orçamento</button>
          <p id="formStatus" class="status" role="status" aria-live="polite"></p>
        </form>
      </div>
    </section>

    <section id="contato" class="section gray">
      <div class="container contact">
        <div>
          <h2>Contato</h2>
          <ul class="contact-list">
            <li><strong>WhatsApp:</strong> <a id="whatsLink" href="#">(51) 99140-0100</a></li>
            <li><strong>Instagram:</strong> <a href="https://www.instagram.com/sm_personalizadosltda" target="_blank" rel="noopener">@sm_personalizadosltda</a></li>
            <li><strong>E-mail:</strong> <a href="mailto:contato@smpersonalizados.com.br">contato@smpersonalizados.com.br</a></li>
          </ul>
          <p class="small">Atendemos de segunda a sexta, 9h às 18h.</p>
        </div>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container">
      © 2025 SM Personalizados — Todos os direitos reservados
    </div>
  </footer>

  <a class="whatsapp-fab" id="btnWhatsFab" href="#" aria-label="Abrir WhatsApp">
    <img src="/assets/whats.svg" alt="WhatsApp" />
  </a>
</body>
</html>
:root{
  --rosa-claro: #FADADD;
  --rosa-medio: #E89AB4;
  --marrom: #A4756D;
  --texto: #333333;
  --fundo: #fff5f7;
  --radius: 14px;
}
*{box-sizing:border-box}
html,body{height:100%}
body{margin:0;font-family:'Poppins',system-ui,-apple-system,Segoe UI,Roboto,Inter,Arial,sans-serif;background:var(--fundo);color:var(--texto)}
.container{max-width:1100px;margin:0 auto;padding:0 20px}
.site-header{position:sticky;top:0;z-index:50;background:linear-gradient(180deg,var(--rosa-claro),var(--rosa-medio));color:#222;box-shadow:0 2px 10px rgba(0,0,0,.04)}
.header-wrap{display:flex;align-items:center;justify-content:space-between;padding:12px 0}
.brand{display:flex;align-items:center;gap:.8rem;color:var(--texto);text-decoration:none}
.brand .logo{height:56px;width:56px;object-fit:contain;border-radius:8px;background:transparent;padding:6px}
.brand-text{font-weight:700;font-family:'Montserrat',sans-serif;font-size:1.25rem;color:var(--marrom)}
.nav a{color:var(--marrom);text-decoration:none;font-weight:600;margin-left:16px}
.nav a:hover{text-decoration:underline;opacity:.95}
.hero{padding:44px 0;background:transparent}
.hero-grid{display:grid;grid-template-columns:1fr 460px;gap:28px;align-items:center}
.hero-copy h1{font-family:'Montserrat',sans-serif;font-size:2.05rem;margin:0 0 10px;color:var(--marrom)}
.hero-copy p{font-size:1.05rem;color:#5a4a49;margin:0 0 16px;line-height:1.6}
.cta-group{display:flex;gap:12px;margin:16px 0 12px}
.btn{display:inline-flex;align-items:center;justify-content:center;padding:12px 18px;border-radius:12px;font-weight:700;text-decoration:none;border:2px solid transparent;transition:.18s;font-family:'Montserrat',sans-serif}
.btn.primary{background:var(--marrom);color:#fff}
.btn.primary:hover{opacity:.95;transform:translateY(-2px)}
.btn.ghost{background:transparent;border:2px solid var(--marrom);color:var(--marrom)}
.trust{display:flex;flex-wrap:wrap;gap:12px;margin-top:10px;font-size:.95rem;color:#5b4b4a}
.hero-art img{max-width:100%;height:auto;border-radius:16px;box-shadow:0 8px 30px rgba(164,117,109,.08);background:#fff;padding:8px}
.section{padding:48px 0;background:transparent}
.section.gray{background:#fff}
h2{font-family:'Montserrat',sans-serif;font-size:1.6rem;margin:0 0 12px;color:var(--marrom)}
.cards{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
.card{background:#fff;border-radius:var(--radius);box-shadow:0 6px 18px rgba(0,0,0,.06);padding:12px;transition:transform .18s;display:flex;flex-direction:column;align-items:stretch}
.card:hover{transform:translateY(-6px)}
.card img{width:100%;height:180px;object-fit:cover;border-radius:12px;margin-bottom:10px}
.card h3{margin:0 0 6px;font-size:1.03rem;color:var(--marrom);font-family:'Montserrat',sans-serif}
.card p{margin:0 0 12px;color:#6b5958;flex:1}
.card .card-actions{display:flex;gap:8px;align-items:center}
.form{background:#fff;border-radius:16px;padding:16px;box-shadow:0 6px 20px rgba(0,0,0,.05)}
.grid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
.form-field{display:flex;flex-direction:column;gap:6px}
label{font-weight:600}
input,select,textarea{padding:10px;border:1px solid #efe6e8;border-radius:10px;font:inherit}
input:focus,select:focus,textarea:focus{outline:none;border-color:var(--marrom);box-shadow:0 0 0 4px rgba(164,117,109,.06)}
.status{margin-top:10px;color:#0b7a0b;font-weight:600}
.contact{display:flex;gap:24px;align-items:flex-start}
.contact-list{list-style:none;padding:0;margin:0;display:grid;gap:8px}
.contact-list a{color:var(--marrom);text-decoration:none;font-weight:600}
.contact-list a:hover{text-decoration:underline}
.site-footer{background:transparent;color:#5b4b4a;padding:22px 0;margin-top:18px;text-align:center}
.whatsapp-fab{position:fixed;right:18px;bottom:18px;height:56px;width:56px;border-radius:50%;background:#25D366;display:flex;align-items:center;justify-content:center;box-shadow:0 8px 20px rgba(0,0,0,.2);z-index:60}
.whatsapp-fab img{height:28px;width:28px;filter:brightness(0) invert(1)}
.category-tabs{display:flex;gap:12px;margin-bottom:16px;flex-wrap:wrap}
.tab{padding:8px 12px;border-radius:999px;border:1px solid transparent;background:transparent;font-weight:700;cursor:pointer}
.tab.active{background:var(--rosa-claro);border-color:var(--marrom);color:var(--marrom)}
.gallery{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
.gallery img{width:100%;height:180px;object-fit:cover;border-radius:12px}
.small{font-size:.9rem;color:#6b5958}
@media (max-width:900px){
  .hero-grid{grid-template-columns:1fr;gap:18px}
  .cards{grid-template-columns:1fr 1fr}
  .gallery{grid-template-columns:1fr 1fr}
}
@media (max-width:640px){
  .nav{display:none}
  .cards{grid-template-columns:1fr}
  .grid{grid-template-columns:1fr}
  .gallery{grid-template-columns:1fr}
  .brand-text{display:none}
}
// Configurações
const WHATS_NUMBER_E164 = "5551991400100"; // +55 51 99140-0100
const API_BASE = ""; // leave empty if backend served from same origin

const PRODUCTS = [
  { id: 'p1', title: 'Caneca Clássica 300ml', desc: 'Porcelana branca 300ml, personalizável com sua arte ou frase.', cat: 'todos' },
  { id: 'p2', title: 'Caneca Colorida', desc: 'Interior colorido e personalização externa em alta qualidade.', cat: 'presente' },
  { id: 'p3', title: 'Caneca Premium', desc: 'Porcelana premium com acabamento brilhante e detalhamento fino.', cat: 'empresas' }
];

const GALLERY = [
  '/assets/prod-classica.jpg',
  '/assets/prod-colorida.jpg',
  '/assets/prod-premium.jpg'
];

function toWhatsLink(msg = 'Olá! Gostaria de um orçamento de canecas.'){
  const text = encodeURIComponent(msg);
  return `https://wa.me/${WHATS_NUMBER_E164}?text=${text}`;
}

function initWhatsButtons(){
  const btnHero = document.getElementById('btnWhatsHero');
  const btnFab = document.getElementById('btnWhatsFab');
  const whatsLink = document.getElementById('whatsLink');
  const url = toWhatsLink();
  [btnHero, btnFab, whatsLink].forEach(el => { if(el){ el.href = url; el.target='_blank'; el.rel='noopener'; } });
}

function renderProducts(filter='todos'){
  const area = document.getElementById('cardsArea');
  area.innerHTML = '';
  const list = PRODUCTS.filter(p => filter === 'todos' || p.cat === filter || p.cat === 'todos');
  list.forEach(p => {
    const card = document.createElement('article');
    card.className = 'card';
    const img = document.createElement('img');
    // use a fallback if not exists (keeps layout)
    img.src = `/assets/${p.id}.jpg`;
    img.alt = p.title;
    const h3 = document.createElement('h3');
    h3.textContent = p.title;
    const pdesc = document.createElement('p');
    pdesc.textContent = p.desc;
    const actions = document.createElement('div');
    actions.className = 'card-actions';
    const btn = document.createElement('a');
    btn.className = 'btn primary';
    btn.href = toWhatsLink(`Olá, quero pedir: ${p.title} — Quantidade: 1 —`);
    btn.target = '_blank';
    btn.rel = 'noopener';
    btn.textContent = 'Peça pelo WhatsApp';
    actions.appendChild(btn);
    card.appendChild(img);
    card.appendChild(h3);
    card.appendChild(pdesc);
    card.appendChild(actions);
    area.appendChild(card);
  });
}

function renderGallery(){
  const g = document.getElementById('galleryArea');
  g.innerHTML = '';
  GALLERY.forEach(src => {
    const i = document.createElement('img');
    i.src = src;
    i.alt = 'Caneca personalizada';
    g.appendChild(i);
  });
}

function initTabs(){
  const tabs = document.querySelectorAll('.tab');
  tabs.forEach(t => {
    t.addEventListener('click', () => {
      tabs.forEach(x => x.classList.remove('active'));
      t.classList.add('active');
      const cat = t.dataset.cat;
      renderProducts(cat === 'presentes' ? 'presente' : (cat === 'tematicas' ? 'tematicas' : cat));
    })
  });
}

async function handleForm(e){
  e.preventDefault();
  const form = e.target;
  const status = document.getElementById('formStatus');
  status.style.color = '#0b7a0b';
  status.textContent = 'Enviando...';

  const formData = new FormData(form);
  try{
    const res = await fetch(`${API_BASE}/api/contact`, { method: 'POST', body: formData });
    if(!res.ok) throw new Error('Falha ao enviar');
    const data = await res.json();
    form.reset();
    status.textContent = data.message || 'Orçamento enviado com sucesso! Em breve entraremos em contato.';
  }catch(err){
    console.error(err);
    status.style.color = '#B00020';
    status.textContent = 'Não foi possível enviar. Tente pelo WhatsApp.';
  }
}

window.addEventListener('DOMContentLoaded', () => {
  initWhatsButtons();
  renderProducts('todos');
  renderGallery();
  initTabs();
  const form = document.getElementById('quoteForm');
  form.addEventListener('submit', handleForm);
});
// Configurações
const WHATS_NUMBER_E164 = "5551991400100"; // +55 51 99140-0100
const API_BASE = ""; // leave empty if backend served from same origin

const PRODUCTS = [
  { id: 'p1', title: 'Caneca Clássica 300ml', desc: 'Porcelana branca 300ml, personalizável com sua arte ou frase.', cat: 'todos' },
  { id: 'p2', title: 'Caneca Colorida', desc: 'Interior colorido e personalização externa em alta qualidade.', cat: 'presente' },
  { id: 'p3', title: 'Caneca Premium', desc: 'Porcelana premium com acabamento brilhante e detalhamento fino.', cat: 'empresas' }
];

const GALLERY = [
  '/assets/prod-classica.jpg',
  '/assets/prod-colorida.jpg',
  '/assets/prod-premium.jpg'
];

function toWhatsLink(msg = 'Olá! Gostaria de um orçamento de canecas.'){
  const text = encodeURIComponent(msg);
  return `https://wa.me/${WHATS_NUMBER_E164}?text=${text}`;
}

function initWhatsButtons(){
  const btnHero = document.getElementById('btnWhatsHero');
  const btnFab = document.getElementById('btnWhatsFab');
  const whatsLink = document.getElementById('whatsLink');
  const url = toWhatsLink();
  [btnHero, btnFab, whatsLink].forEach(el => { if(el){ el.href = url; el.target='_blank'; el.rel='noopener'; } });
}

function renderProducts(filter='todos'){
  const area = document.getElementById('cardsArea');
  area.innerHTML = '';
  const list = PRODUCTS.filter(p => filter === 'todos' || p.cat === filter || p.cat === 'todos');
  list.forEach(p => {
    const card = document.createElement('article');
    card.className = 'card';
    const img = document.createElement('img');
    // use a fallback if not exists (keeps layout)
    img.src = `/assets/${p.id}.jpg`;
    img.alt = p.title;
    const h3 = document.createElement('h3');
    h3.textContent = p.title;
    const pdesc = document.createElement('p');
    pdesc.textContent = p.desc;
    const actions = document.createElement('div');
    actions.className = 'card-actions';
    const btn = document.createElement('a');
    btn.className = 'btn primary';
    btn.href = toWhatsLink(`Olá, quero pedir: ${p.title} — Quantidade: 1 —`);
    btn.target = '_blank';
    btn.rel = 'noopener';
    btn.textContent = 'Peça pelo WhatsApp';
    actions.appendChild(btn);
    card.appendChild(img);
    card.appendChild(h3);
    card.appendChild(pdesc);
    card.appendChild(actions);
    area.appendChild(card);
  });
}

function renderGallery(){
  const g = document.getElementById('galleryArea');
  g.innerHTML = '';
  GALLERY.forEach(src => {
    const i = document.createElement('img');
    i.src = src;
    i.alt = 'Caneca personalizada';
    g.appendChild(i);
  });
}

function initTabs(){
  const tabs = document.querySelectorAll('.tab');
  tabs.forEach(t => {
    t.addEventListener('click', () => {
      tabs.forEach(x => x.classList.remove('active'));
      t.classList.add('active');
      const cat = t.dataset.cat;
      renderProducts(cat === 'presentes' ? 'presente' : (cat === 'tematicas' ? 'tematicas' : cat));
    })
  });
}

async function handleForm(e){
  e.preventDefault();
  const form = e.target;
  const status = document.getElementById('formStatus');
  status.style.color = '#0b7a0b';
  status.textContent = 'Enviando...';

  const formData = new FormData(form);
  try{
    const res = await fetch(`${API_BASE}/api/contact`, { method: 'POST', body: formData });
    if(!res.ok) throw new Error('Falha ao enviar');
    const data = await res.json();
    form.reset();
    status.textContent = data.message || 'Orçamento enviado com sucesso! Em breve entraremos em contato.';
  }catch(err){
    console.error(err);
    status.style.color = '#B00020';
    status.textContent = 'Não foi possível enviar. Tente pelo WhatsApp.';
  }
}

window.addEventListener('DOMContentLoaded', () => {
  initWhatsButtons();
  renderProducts('todos');
  renderGallery();
  initTabs();
  const form = document.getElementById('quoteForm');
  form.addEventListener('submit', handleForm);
});
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32"><path fill="#25D366" d="M16 .5C7.5.5.6 7.5.6 16c0 2.7.7 5.3 2.1 7.6L.5 31.5l8-2.1c2.2 1.2 4.7 1.9 7.3 1.9 8.5 0 15.4-7 15.4-15.5S24.5.5 16 .5z"/><path fill="#fff" d="M25 20.4c-.3.9-1.7 1.6-2.3 1.6-.6 0-1.3.2-4.4-1-3.7-1.5-6-5.2-6.2-5.5-.2-.3-1.5-2.1-1.5-4s1-2.8 1.4-3.2c.4-.4.9-.5 1.2-.5h.9c.3 0 .7.1 1 .8.4 1 .9 2.5 1 2.7.1.2.1.4 0 .6-.1.2-.2.4-.4.6s-.4.5-.6.7c-.2.2-.4.5-.2.9.2.4.9 1.5 1.9 2.4 1.3 1.1 2.4 1.6 2.8 1.8.4.2.7.2 1-.1.3-.3 1.1-1.2 1.4-1.6.3-.4.6-.3.9-.2.3.1 2.1 1 2.3 1.1.3.2.5.2.6.3.1.1.1.3 0 .5z"/></svg>
import express from "express";
import cors from "cors";
import helmet from "helmet";
import rateLimit from "express-rate-limit";
import multer from "multer";
import nodemailer from "nodemailer";
import path from "path";
import fs from "fs";
import dotenv from "dotenv";
dotenv.config();

const app = express();
const PORT = process.env.PORT || 3000;
const ORIGIN = process.env.CORS_ORIGIN || "*";

// Middlewares
app.use(helmet());
app.use(cors({ origin: ORIGIN }));
app.use(express.json());

// Rate limit basic
const limiter = rateLimit({ windowMs: 60 * 1000, max: 30 });
app.use("/api/", limiter);

// Static frontend (served by backend)
const __dirname = path.resolve();
app.use(express.static(path.join(__dirname, "frontend")));

// Upload config
const uploadDir = path.join(__dirname, "backend", "uploads");
if (!fs.existsSync(uploadDir)) fs.mkdirSync(uploadDir, { recursive: true });

const storage = multer.diskStorage({
  destination: (_req, _file, cb) => cb(null, uploadDir),
  filename: (_req, file, cb) => {
    const unique = Date.now() + "-" + Math.round(Math.random() * 1e9);
    const ext = path.extname(file.originalname);
    cb(null, file.fieldname + "-" + unique + ext);
  },
});

const upload = multer({
  storage,
  limits: { fileSize: 10 * 1024 * 1024 }, // 10MB
  fileFilter: (_req, file, cb) => {
    const ok = /\.(png|jpg|jpeg|pdf)$/i.test(file.originalname);
    cb(ok ? null : new Error("Arquivo inválido"));
  },
});

// Email transporter
const transporter = nodemailer.createTransport({
  host: process.env.SMTP_HOST,
  port: Number(process.env.SMTP_PORT || 587),
  secure: process.env.SMTP_SECURE === "true",
  auth: {
    user: process.env.SMTP_USER,
    pass: process.env.SMTP_PASS,
  },
});

app.post("/api/contact", upload.single("arquivo"), async (req, res) => {
  try {
    const { nome, email, telefone, mensagem, produto, quantidade } = req.body;

    if (!nome || !telefone) {
      return res.status(400).json({ message: "Nome e telefone são obrigatórios." });
    }

    const to = process.env.TO_EMAIL || "contato@smpersonalizados.com.br";
    const from = process.env.FROM_EMAIL || process.env.SMTP_USER || "no-reply@smpersonalizados.com.br";

    const text = [
      `Nova solicitação de orçamento:`, "",
      `Nome: ${nome}`,
      `Telefone: ${telefone}`,
      `E-mail: ${email || '-'}`,
      `Produto: ${produto || "-"}`,
      `Quantidade: ${quantidade || "-"}`,
      `Mensagem: ${mensagem || "-"}`,
    ].join("\n");

    const attachments = [];
    if (req.file) {
      attachments.push({
        filename: req.file.originalname,
        path: req.file.path,
      });
    }

    await transporter.sendMail({
      to,
      from,
      subject: "Novo orçamento - SM Personalizados",
      text,
      attachments,
    });

    res.json({ message: "Orçamento enviado com sucesso! Em breve entraremos em contato." });
  } catch (err) {
    console.error(err);
    res.status(500).json({ message: "Erro ao enviar. Contate via WhatsApp como alternativa." });
  }
});

// SPA/Static fallback
app.get("*", (_req, res) => {
  res.sendFile(path.join(__dirname, "frontend", "index.html"));
});

app.listen(PORT, () => {
  console.log("Servidor rodando em http://localhost:" + PORT);
});
