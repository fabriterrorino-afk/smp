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
