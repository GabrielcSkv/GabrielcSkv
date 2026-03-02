<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Seu Nome — Portfólio</title>
  <meta name="description" content="Portfólio de Seu Nome: projetos, habilidades e contato." />

  <style>
    :root{
      --bg:#0b0f17;
      --card:#101826;
      --muted:#91a4c2;
      --text:#eaf1ff;
      --line:rgba(255,255,255,.08);
      --accent:#7c5cff;
      --accent2:#34d399;
      --shadow: 0 20px 60px rgba(0,0,0,.45);
      --radius:16px;
    }
    *{ box-sizing:border-box; }
    html,body{ margin:0; padding:0; font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial; background:radial-gradient(1200px 700px at 20% -10%, rgba(124,92,255,.25), transparent 60%), radial-gradient(900px 600px at 80% 10%, rgba(52,211,153,.18), transparent 55%), var(--bg); color:var(--text); }
    a{ color:inherit; text-decoration:none; }
    .container{ width:min(1100px, 92vw); margin:0 auto; }

    /* Topbar */
    .topbar{
      position:sticky; top:0; z-index:10;
      backdrop-filter: blur(12px);
      background:rgba(11,15,23,.65);
      border-bottom:1px solid var(--line);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between;
      padding:14px 0;
      gap:14px;
    }
    .brand{
      display:flex; align-items:center; gap:10px; font-weight:700; letter-spacing:.2px;
    }
    .logo{
      width:34px; height:34px; border-radius:10px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      box-shadow: 0 12px 40px rgba(124,92,255,.25);
    }
    .navlinks{ display:flex; gap:14px; align-items:center; flex-wrap:wrap; }
    .navlinks a{
      padding:8px 10px; border-radius:10px; color:var(--muted);
      border:1px solid transparent;
    }
    .navlinks a:hover{ color:var(--text); border-color: var(--line); background:rgba(255,255,255,.03); }
    .cta{
      display:flex; gap:10px; align-items:center;
    }
    .btn{
      display:inline-flex; align-items:center; justify-content:center; gap:10px;
      padding:10px 14px; border-radius:12px;
      border:1px solid var(--line); background:rgba(255,255,255,.03);
      color:var(--text); cursor:pointer;
    }
    .btn:hover{ border-color: rgba(124,92,255,.45); }
    .btn.primary{
      background: linear-gradient(135deg, rgba(124,92,255,.95), rgba(52,211,153,.85));
      border: none;
      box-shadow: 0 18px 60px rgba(124,92,255,.18);
    }
    .btn.primary:hover{ filter:saturate(1.05) brightness(1.05); }

    /* Hero */
    .hero{
      padding: 56px 0 26px;
      display:grid;
      grid-template-columns: 1.2fr .8fr;
      gap: 22px;
      align-items:stretch;
    }
    @media (max-width: 900px){
      .hero{ grid-template-columns: 1fr; padding-top: 34px; }
    }
    .card{
      background: rgba(255,255,255,.03);
      border:1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }
    .hero-left{ padding: 28px; position:relative; overflow:hidden; }
    .pill{
      display:inline-flex; align-items:center; gap:10px;
      padding:8px 12px; border-radius:999px;
      border:1px solid var(--line);
      color: var(--muted);
      background: rgba(255,255,255,.02);
      font-size: 14px;
    }
    .dot{ width:8px; height:8px; border-radius:999px; background: var(--accent2); box-shadow:0 0 0 4px rgba(52,211,153,.12); }
    h1{
      margin:14px 0 10px; font-size: clamp(28px, 3.2vw, 44px);
      line-height:1.1;
    }
    .subtitle{
      margin: 0 0 18px;
      color: var(--muted);
      font-size: 16px;
      line-height:1.6;
      max-width: 60ch;
    }
    .hero-actions{ display:flex; gap:12px; flex-wrap:wrap; margin-top: 18px; }
    .chips{ display:flex; gap:8px; flex-wrap:wrap; margin-top: 18px; }
    .chip{
      font-size: 13px;
      padding: 8px 10px;
      border-radius: 999px;
      border: 1px solid var(--line);
      color: var(--muted);
      background: rgba(255,255,255,.02);
    }
    .hero-right{ padding: 18px; display:flex; flex-direction:column; gap:12px; }
    .profile{
      display:flex; gap:12px; align-items:center; padding: 14px;
      background: rgba(255,255,255,.02);
      border:1px solid var(--line);
      border-radius: 14px;
    }
    .avatar{
      width:54px; height:54px; border-radius: 14px;
      background: linear-gradient(135deg, rgba(255,255,255,.15), rgba(255,255,255,.02));
      border:1px solid var(--line);
      display:flex; align-items:center; justify-content:center;
      font-weight:700;
      color: rgba(255,255,255,.85);
    }
    .profile small{ color: var(--muted); display:block; margin-top:2px; }
    .stats{
      display:grid; grid-template-columns: 1fr 1fr; gap: 12px;
    }
    .stat{
      padding:14px; border-radius:14px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.02);
    }
    .stat b{ font-size: 18px; }
    .stat span{ display:block; color: var(--muted); margin-top:4px; font-size: 13px; }

    /* Sections */
    section{ padding: 22px 0; }
    .section-title{
      display:flex; align-items:flex-end; justify-content:space-between;
      gap:16px; margin-bottom: 12px;
    }
    .section-title h2{ margin:0; font-size: 20px; letter-spacing:.2px; }
    .section-title p{ margin:0; color: var(--muted); }

    /* Projects grid */
    .grid{
      display:grid;
      grid-template-columns: repeat(12, 1fr);
      gap: 14px;
    }
    .project{
      grid-column: span 4;
      overflow:hidden;
      border-radius: var(--radius);
      border: 1px solid var(--line);
      background: rgba(255,255,255,.03);
      transition: transform .15s ease, border-color .15s ease;
    }
    .project:hover{ transform: translateY(-4px); border-color: rgba(124,92,255,.45); }
    @media (max-width: 980px){ .project{ grid-column: span 6; } }
    @media (max-width: 640px){ .project{ grid-column: span 12; } }

    .thumb{
      aspect-ratio: 16/10;
      width:100%;
      display:block;
      object-fit: cover;
      border-bottom: 1px solid var(--line);
      background: #0e1523;
    }
    .project-body{ padding: 14px; }
    .project-body h3{ margin:0 0 6px; font-size: 16px; }
    .project-body p{ margin:0 0 12px; color: var(--muted); line-height: 1.5; font-size: 14px; }
    .tags{ display:flex; gap:8px; flex-wrap:wrap; }
    .tag{
      font-size: 12px;
      padding: 6px 8px;
      border-radius: 999px;
      border: 1px solid var(--line);
      color: var(--muted);
      background: rgba(255,255,255,.02);
    }
    .project-links{
      margin-top: 12px;
      display:flex; gap:10px; flex-wrap:wrap;
    }
    .link{
      font-size: 13px;
      padding: 8px 10px;
      border-radius: 12px;
      border: 1px solid var(--line);
      color: var(--text);
      background: rgba(255,255,255,.02);
    }
    .link:hover{ border-color: rgba(52,211,153,.45); }

    /* About + skills */
    .two-col{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap: 14px;
    }
    @media (max-width: 900px){ .two-col{ grid-template-columns: 1fr; } }
    .box{ padding: 18px; }
    .box p{ color: var(--muted); line-height: 1.7; margin: 10px 0 0; }
    .skills{ display:flex; gap:10px; flex-wrap:wrap; margin-top: 10px; }
    .skill{
      padding:10px 12px;
      border:1px solid var(--line);
      border-radius: 14px;
      background: rgba(255,255,255,.02);
      color: var(--text);
      font-size: 14px;
    }
    .skill small{ display:block; color: var(--muted); margin-top:4px; font-size: 12px; }

    /* Contact */
    .contact{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap: 14px;
      align-items:stretch;
    }
    @media (max-width: 900px){ .contact{ grid-template-columns: 1fr; } }
    .field{
      display:flex; flex-direction:column; gap:8px;
      margin-top: 12px;
    }
    input, textarea{
      width:100%;
      padding: 12px 12px;
      border-radius: 12px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.02);
      color: var(--text);
      outline:none;
    }
    input:focus, textarea:focus{ border-color: rgba(124,92,255,.55); }
    textarea{ min-height: 110px; resize: vertical; }
    .footer{
      padding: 26px 0 40px;
      color: var(--muted);
      border-top:1px solid var(--line);
      margin-top: 22px;
      font-size: 13px;
    }

    /* Modal */
    .modal-backdrop{
      position:fixed; inset:0;
      background: rgba(0,0,0,.6);
      display:none;
      align-items:center; justify-content:center;
      padding: 18px;
      z-index: 50;
    }
    .modal{
      width:min(900px, 96vw);
      border-radius: 18px;
      overflow:hidden;
      border:1px solid var(--line);
      background: rgba(16,24,38,.92);
      box-shadow: var(--shadow);
    }
    .modal header{
      display:flex; align-items:center; justify-content:space-between;
      padding: 12px 14px;
      border-bottom:1px solid var(--line);
    }
    .modal header b{ font-size: 14px; }
    .modal .content{ padding: 14px; }
    .modal img{ width:100%; height:auto; border-radius: 14px; border:1px solid var(--line); }
    .close{ padding: 8px 10px; border-radius: 12px; border:1px solid var(--line); background: rgba(255,255,255,.03); cursor:pointer; }
    .close:hover{ border-color: rgba(255,255,255,.18); }
  </style>
</head>

<body>
  <div class="topbar">
    <div class="container">
      <div class="nav">
        <a class="brand" href="#topo">
          <span class="logo" aria-hidden="true"></span>
          <span>Seu Nome</span>
        </a>

        <nav class="navlinks" aria-label="Navegação">
          <a href="#projetos">Projetos</a>
          <a href="#sobre">Sobre</a>
          <a href="#contato">Contato</a>
        </nav>

        <div class="cta">
          <a class="btn" href="https://www.linkedin.com" target="_blank" rel="noreferrer">LinkedIn</a>
          <a class="btn primary" href="#contato">Fale comigo</a>
        </div>
      </div>
    </div>
  </div>

  <main id="topo" class="container">
    <!-- HERO -->
    <div class="hero">
      <div class="card hero-left">
        <span class="pill"><span class="dot"></span> Disponível para freelas • São Paulo</span>
        <h1>Eu crio experiências e visuais que parecem simples — porque são bem pensados.</h1>
        <p class="subtitle">
          Sou <b>Seu Nome</b>, <b>sua profissão</b> focado(a) em <b>resultado</b>.
          Aqui estão alguns projetos com contexto, processo e entregáveis.
        </p>

        <div class="hero-actions">
          <a class="btn primary" href="#projetos">Ver projetos</a>
          <a class="btn" href="#contato">Orçamento</a>
          <button class="btn" id="btnDownload">Baixar CV (exemplo)</button>
        </div>

        <div class="chips">
          <span class="chip">Branding</span>
          <span class="chip">Design Digital</span>
          <span class="chip">UI/UX</span>
          <span class="chip">Conteúdo</span>
        </div>
      </div>

      <aside class="card hero-right">
        <div class="profile">
          <div class="avatar">SN</div>
          <div>
            <b>Seu Nome</b>
            <small>Profissão • Especialidade</small>
          </div>
        </div>

        <div class="stats">
          <div class="stat">
            <b>+12</b>
            <span>Projetos entregues</span>
          </div>
          <div class="stat">
            <b>4.9★</b>
            <span>Avaliação média</span>
          </div>
          <div class="stat">
            <b>3–10d</b>
            <span>Prazo típico</span>
          </div>
          <div class="stat">
            <b>100%</b>
            <span>Arquivos editáveis</span>
          </div>
        </div>
      </aside>
    </div>

    <!-- PROJECTS -->
    <section id="projetos">
      <div class="section-title">
        <div>
          <h2>Projetos</h2>
          <p>Seleção com imagens (clique para ampliar).</p>
        </div>
      </div>

      <div class="grid">
        <!-- Projeto 1 -->
        <article class="project" data-title="Identidade Visual — Cafeteria" data-img="https://images.unsplash.com/photo-1511920170033-f8396924c348?auto=format&fit=crop&w=1600&q=70">
          <img class="thumb" alt="Cafeteria — branding" src="https://images.unsplash.com/photo-1511920170033-f8396924c348?auto=format&fit=crop&w=1200&q=70">
          <div class="project-body">
            <h3>Identidade Visual — Cafeteria</h3>
            <p>Logo, paleta, tipografia e aplicações para embalagem e redes sociais.</p>
            <div class="tags">
              <span class="tag">Branding</span><span class="tag">Logo</span><span class="tag">Social</span>
            </div>
            <div class="project-links">
              <a class="link" href="#" onclick="return false;">Case</a>
              <a class="link" href="#" onclick="return false;">Behance</a>
            </div>
          </div>
        </article>

        <!-- Projeto 2 -->
        <article class="project" data-title="Landing Page — Produto" data-img="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=1600&q=70">
          <img class="thumb" alt="Equipe — landing page" src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=1200&q=70">
          <div class="project-body">
            <h3>Landing Page — Produto</h3>
            <p>Estrutura de conversão, copy curta e layout responsivo para lançamento.</p>
            <div class="tags">
              <span class="tag">Web</span><span class="tag">UI</span><span class="tag">Conversão</span>
            </div>
            <div class="project-links">
              <a class="link" href="#" onclick="return false;">Live</a>
              <a class="link" href="#" onclick="return false;">Figma</a>
            </div>
          </div>
        </article>

        <!-- Projeto 3 -->
        <article class="project" data-title="App — Finanças" data-img="https://images.unsplash.com/photo-1551288049-bebda4e38f71?auto=format&fit=crop&w=1600&q=70">
          <img class="thumb" alt="Dashboard — app finanças" src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?auto=format&fit=crop&w=1200&q=70">
          <div class="project-body">
            <h3>App — Finanças</h3>
            <p>Fluxos, telas-chave e protótipo navegável focado em clareza.</p>
            <div class="tags">
              <span class="tag">UX</span><span class="tag">Figma</span><span class="tag">Mobile</span>
            </div>
            <div class="project-links">
              <a class="link" href="#" onclick="return false;">Protótipo</a>
              <a class="link" href="#" onclick="return false;">Wireframes</a>
            </div>
          </div>
        </article>

        <!-- Projeto 4 -->
        <article class="project" data-title="Social Media — Campanha" data-img="https://images.unsplash.com/photo-1557804506-669a67965ba0?auto=format&fit=crop&w=1600&q=70">
          <img class="thumb" alt="Social media — campanha" src="https://images.unsplash.com/photo-1557804506-669a67965ba0?auto=format&fit=crop&w=1200&q=70">
          <div class="project-body">
            <h3>Social Media — Campanha</h3>
            <p>Peças para feed e stories com consistência e variações de formato.</p>
            <div class="tags">
              <span class="tag">Conteúdo</span><span class="tag">Ads</span><span class="tag">Templates</span>
            </div>
            <div class="project-links">
              <a class="link" href="#" onclick="return false;">Galeria</a>
              <a class="link" href="#" onclick="return false;">Resultados</a>
            </div>
          </div>
        </article>

        <!-- Projeto 5 -->
        <article class="project" data-title="Apresentação — Pitch" data-img="https://images.unsplash.com/photo-1553877522-43269d4ea984?auto=format&fit=crop&w=1600&q=70">
          <img class="thumb" alt="Apresentação — pitch" src="https://images.unsplash.com/photo-1553877522-43269d4ea984?auto=format&fit=crop&w=1200&q=70">
          <div class="project-body">
            <h3>Apresentação — Pitch</h3>
            <p>Storytelling, hierarquia de informação e design para impacto.</p>
            <div class="tags">
              <span class="tag">Slides</span><span class="tag">Storytelling</span><span class="tag">Brand</span>
            </div>
            <div class="project-links">
              <a class="link" href="#" onclick="return false;">PDF</a>
              <a class="link" href="#" onclick="return false;">Deck</a>
            </div>
          </div>
        </article>

        <!-- Projeto 6 -->
        <article class="project" data-title="E-commerce — Loja" data-img="https://images.unsplash.com/photo-1523275335684-37898b6baf30?auto=format&fit=crop&w=1600&q=70">
          <img class="thumb" alt="E-commerce — loja" src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?auto=format&fit=crop&w=1200&q=70">
          <div class="project-body">
            <h3>E-commerce — Loja</h3>
            <p>Home + produto + carrinho com foco em navegação e confiança.</p>
            <div class="tags">
              <span class="tag">Web</span><span class="tag">UI</span><span class="tag">E-commerce</span>
            </div>
            <div class="project-links">
              <a class="link" href="#" onclick="return false;">Demo</a>
              <a class="link" href="#" onclick="return false;">Componentes</a>
            </div>
          </div>
        </article>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="sobre">
      <div class="section-title">
        <div>
          <h2>Sobre</h2>
          <p>Um resumo do seu perfil + skills.</p>
        </div>
      </div>

      <div class="two-col">
        <div class="card box">
          <h3 style="margin:0;">Quem eu sou</h3>
          <p>
            Escreva aqui um parágrafo curto falando do seu foco, experiência e diferencial.
            Ex: “Trabalho com design e produto, transformando objetivos de negócio em interfaces claras.”
          </p>
          <p>
            Você pode incluir números (ex: +X projetos), segmentos (ex: saúde, varejo) e seu estilo de trabalho.
          </p>
        </div>

        <div class="card box">
          <h3 style="margin:0;">Habilidades</h3>
          <div class="skills">
            <div class="skill">Figma <small>UI/UX • protótipos</small></div>
            <div class="skill">Illustrator <small>marca • vetores</small></div>
            <div class="skill">Photoshop <small>tratamento • peças</small></div>
            <div class="skill">Web <small>HTML/CSS • noções</small></div>
            <div class="skill">Gestão <small>prazos • alinhamentos</small></div>
          </div>
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contato">
      <div class="section-title">
        <div>
          <h2>Contato</h2>
          <p>Deixe fácil para a pessoa te chamar.</p>
        </div>
      </div>

      <div class="contact">
        <div class="card box">
          <h3 style="margin:0;">Vamos conversar</h3>
          <p>
            Email: <b>seuemail@email.com</b><br/>
            WhatsApp: <b>(11) 99999-9999</b><br/>
            Cidade: <b>São Paulo</b>
          </p>
          <p>
            Dica: aqui você pode colocar disponibilidade, tipo de projeto e faixa de orçamento.
          </p>
          <div class="hero-actions">
            <a class="btn primary" href="mailto:seuemail@email.com?subject=Quero%20um%20or%C3%A7amento">Enviar email</a>
            <a class="btn" href="https://wa.me/5511999999999" target="_blank" rel="noreferrer">WhatsApp</a>
          </div>
        </div>

        <form class="card box" onsubmit="return fakeSend(event)">
          <h3 style="margin:0;">Mensagem (exemplo)</h3>
          <div class="field">
            <label for="nome" style="color:var(--muted); font-size:13px;">Seu nome</label>
            <input id="nome" placeholder="Ex: Ana" required />
          </div>
          <div class="field">
            <label for="email" style="color:var(--muted); font-size:13px;">Seu email</label>
            <input id="email" type="email" placeholder="ana@email.com" required />
          </div>
          <div class="field">
            <label for="msg" style="color:var(--muted); font-size:13px;">O que você precisa?</label>
            <textarea id="msg" placeholder="Conte um pouco do projeto..." required></textarea>
          </div>
          <div class="hero-actions">
            <button class="btn primary" type="submit">Enviar</button>
            <button class="btn" type="reset">Limpar</button>
          </div>
          <p id="formStatus" style="margin:10px 0 0; color:var(--muted); font-size:13px;"></p>
        </form>
      </div>
    </section>

    <div class="footer">
      © <span id="year"></span> Seu Nome — Portfólio. Feito com HTML/CSS.
    </div>
  </main>

  <!-- MODAL (zoom do projeto) -->
  <div class="modal-backdrop" id="backdrop" role="dialog" aria-modal="true" aria-label="Projeto">
    <div class="modal">
      <header>
        <b id="modalTitle">Projeto</b>
        <button class="close" id="closeModal">Fechar</button>
      </header>
      <div class="content">
        <img id="modalImg" alt="Imagem do projeto" />
      </div>
    </div>
  </div>

  <script>
    // Ano no footer
    document.getElementById("year").textContent = new Date().getFullYear();

    // Modal de projeto
    const backdrop = document.getElementById("backdrop");
    const modalTitle = document.getElementById("modalTitle");
    const modalImg = document.getElementById("modalImg");
    const closeModalBtn = document.getElementById("closeModal");

    function openModal(title, img){
      modalTitle.textContent = title;
      modalImg.src = img;
      backdrop.style.display = "flex";
      document.body.style.overflow = "hidden";
    }
    function closeModal(){
      backdrop.style.display = "none";
      document.body.style.overflow = "auto";
    }

    document.querySelectorAll(".project").forEach(card => {
      card.addEventListener("click", () => {
        openModal(card.dataset.title, card.dataset.img);
      });
    });
    closeModalBtn.addEventListener("click", closeModal);
    backdrop.addEventListener("click", (e) => {
      if(e.target === backdrop) closeModal();
    });
    window.addEventListener("keydown", (e) => {
      if(e.key === "Escape") closeModal();
    });

    // Botão "Baixar CV" (exemplo)
    document.getElementById("btnDownload").addEventListener("click", () => {
      alert("Aqui você pode linkar um PDF real do seu currículo (ex: /cv.pdf).");
    });

    // Form fake
    function fakeSend(e){
      e.preventDefault();
      const status = document.getElementById("formStatus");
      status.textContent = "Mensagem enviada (exemplo). Troque por integração real se quiser.";
      return false;
    }
  </script>
</body>
</html>
