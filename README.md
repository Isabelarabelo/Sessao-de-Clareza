<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sessão de Clareza Estratégica – Isabela Rabelo</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --cream: #F7F4EF;
    --warm-dark: #1C1A17;
    --warm-mid: #5C5649;
    --accent: #B5853A;
    --accent-light: #E8D9BE;
    --line: rgba(92,86,73,0.18);
    --serif: 'Playfair Display', Georgia, serif;
    --sans: 'DM Sans', sans-serif;
  }

  html { scroll-behavior: smooth; }

  body {
    font-family: var(--sans);
    background-color: var(--cream);
    color: var(--warm-dark);
    font-size: 16px;
    line-height: 1.7;
    -webkit-font-smoothing: antialiased;
  }

  .container {
    max-width: 780px;
    margin: 0 auto;
    padding: 0 2rem;
  }

  .hero {
    padding: 100px 0 80px;
    border-bottom: 1px solid var(--line);
  }

  .hero-label {
    font-family: var(--sans);
    font-size: 11px;
    font-weight: 500;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 32px;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .hero-label::before {
    content: '';
    display: inline-block;
    width: 28px;
    height: 1px;
    background: var(--accent);
  }

  .hero h1 {
    font-family: var(--serif);
    font-size: clamp(2.4rem, 6vw, 3.8rem);
    font-weight: 400;
    line-height: 1.15;
    color: var(--warm-dark);
    margin-bottom: 24px;
    letter-spacing: -0.01em;
  }

  .hero h1 em {
    font-style: italic;
    color: var(--accent);
  }

  .hero-sub {
    font-size: 17px;
    color: var(--warm-mid);
    max-width: 540px;
    line-height: 1.75;
    font-weight: 300;
  }

  section {
    padding: 72px 0;
    border-bottom: 1px solid var(--line);
  }

  .section-label {
    font-size: 10px;
    font-weight: 500;
    letter-spacing: 0.22em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 20px;
  }

  h2 {
    font-family: var(--serif);
    font-size: clamp(1.5rem, 4vw, 2.1rem);
    font-weight: 400;
    line-height: 1.3;
    color: var(--warm-dark);
    margin-bottom: 28px;
  }

  p { color: var(--warm-mid); font-weight: 300; font-size: 16px; }

  .para-quem-grid { margin-top: 40px; display: grid; gap: 1px; background: var(--line); border: 1px solid var(--line); border-radius: 4px; overflow: hidden; }

  .para-quem-item { background: var(--cream); padding: 22px 28px; display: flex; align-items: flex-start; gap: 16px; transition: background 0.2s; }
  .para-quem-item:hover { background: #F0EBE1; }

  .check { width: 20px; height: 20px; min-width: 20px; border: 1.5px solid var(--accent); border-radius: 50%; display: flex; align-items: center; justify-content: center; margin-top: 3px; }
  .check::after { content: ''; width: 6px; height: 6px; background: var(--accent); border-radius: 50%; }
  .para-quem-item p { color: var(--warm-dark); font-size: 15px; font-weight: 400; }

  .destravar-list { margin-top: 40px; display: grid; grid-template-columns: 1fr 1fr; gap: 24px; }
  @media (max-width: 560px) { .destravar-list { grid-template-columns: 1fr; } }

  .destravar-item { padding: 28px 24px; border: 1px solid var(--line); border-radius: 4px; }
  .destravar-num { font-family: var(--serif); font-size: 36px; font-weight: 400; color: var(--accent-light); line-height: 1; margin-bottom: 12px; }
  .destravar-item p { font-size: 14px; color: var(--warm-dark); font-weight: 400; line-height: 1.65; }

  .entregaveis-grid { margin-top: 48px; display: grid; gap: 20px; }

  .entregavel { display: grid; grid-template-columns: 56px 1fr; gap: 24px; align-items: start; padding: 28px 28px 28px 24px; border: 1px solid var(--line); border-radius: 4px; background: #fff; }

  .entregavel-num { font-family: var(--serif); font-size: 13px; font-weight: 600; color: var(--accent); padding-top: 4px; text-align: center; width: 40px; height: 40px; border: 1.5px solid var(--accent); border-radius: 50%; display: flex; align-items: center; justify-content: center; }

  .entregavel h3 { font-family: var(--serif); font-size: 17px; font-weight: 600; color: var(--warm-dark); margin-bottom: 8px; line-height: 1.4; }
  .entregavel p { font-size: 14px; color: var(--warm-mid); font-weight: 300; line-height: 1.7; }

  .resultado-grid { margin-top: 40px; display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
  @media (max-width: 560px) { .resultado-grid { grid-template-columns: 1fr; } }

  .resultado-item { background: var(--warm-dark); color: var(--cream); padding: 24px 22px; border-radius: 4px; }
  .resultado-item p { color: rgba(247,244,239,0.85); font-size: 15px; font-weight: 300; }
  .resultado-item strong { font-family: var(--serif); font-size: 18px; font-weight: 600; display: block; margin-bottom: 6px; color: #fff; font-style: italic; }

  .cta-section { padding: 80px 0 100px; border-bottom: 1px solid var(--line); }

  .cta-price { display: flex; align-items: baseline; gap: 8px; margin-bottom: 8px; }
  .cta-price .label { font-size: 13px; color: var(--warm-mid); text-transform: uppercase; letter-spacing: 0.1em; font-weight: 500; }
  .cta-price .value { font-family: var(--serif); font-size: 2.4rem; font-weight: 600; color: var(--warm-dark); }
  .cta-note { font-size: 13px; color: var(--warm-mid); font-style: italic; }

  .cta-btn {
    display: inline-block;
    background: var(--accent);
    color: #fff;
    text-decoration: none;
    padding: 18px 48px;
    font-family: var(--sans);
    font-size: 13px;
    font-weight: 500;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    border-radius: 3px;
    transition: background 0.2s, transform 0.15s;
  }
  .cta-btn:hover { background: #9A6E2E; transform: translateY(-1px); }

  .quote-section { padding: 60px 0; border-bottom: 1px solid var(--line); }
  blockquote { font-family: var(--serif); font-size: clamp(1.1rem, 3vw, 1.45rem); font-style: italic; color: var(--warm-mid); line-height: 1.6; padding-left: 28px; border-left: 2px solid var(--accent); font-weight: 400; }

  .sobre-section { padding: 72px 0 100px; border-bottom: none; }
  .sobre-inner { display: grid; grid-template-columns: 200px 1fr; gap: 48px; align-items: start; }
  @media (max-width: 600px) { .sobre-inner { grid-template-columns: 1fr; } }

  .sobre-photo { width: 180px; height: 180px; border-radius: 4px; object-fit: cover; object-position: center top; }

  .sobre-text h3 { font-family: var(--serif); font-size: 1.6rem; font-weight: 600; color: var(--warm-dark); margin-bottom: 6px; }
  .sobre-text .sobre-tagline { font-size: 14px; color: var(--accent); font-weight: 500; letter-spacing: 0.05em; margin-bottom: 20px; }
  .sobre-text p { font-size: 15px; color: var(--warm-mid); font-weight: 300; line-height: 1.8; margin-bottom: 12px; }
  .sobre-text p:last-child { margin-bottom: 0; }
</style>
</head>
<body>
<div class="container">

  <header class="hero">
    <div class="hero-label">Sessão Individual · Posicionamento Estratégico</div>
    <h1>Clareza para quem já<br>tem repertório, mas ainda<br>não tem <em>direção.</em></h1>
    <p class="hero-sub">Uma sessão conduzida por perguntas estratégicas para organizar sua identidade, definir seu cliente ideal e iniciar com intenção real — não tentativa.</p>
  </header>

  <section class="quote-section">
    <blockquote>
      "O problema não é falta de esforço ou conhecimento — é excesso de informação, insegurança na comunicação e dificuldade em atrair o cliente certo."
    </blockquote>
  </section>

  <section>
    <div class="section-label">Para quem é</div>
    <h2>Você se reconhece<br>nesse cenário?</h2>
    <div class="para-quem-grid">
      <div class="para-quem-item"><span class="check"></span><p>Sente que sua comunicação não reflete quem você é de verdade</p></div>
      <div class="para-quem-item"><span class="check"></span><p>Atrai clientes desalinhados com a sua proposta</p></div>
      <div class="para-quem-item"><span class="check"></span><p>Tem dificuldade em se posicionar com segurança</p></div>
      <div class="para-quem-item"><span class="check"></span><p>Produz conteúdo sem clareza de direção</p></div>
      <div class="para-quem-item"><span class="check"></span><p>Quer parar de recomeçar e estruturar algo consistente</p></div>
    </div>
  </section>

  <section>
    <div class="section-label">O que trabalhamos</div>
    <h2>O que vamos<br>destravar juntos</h2>
    <p>Durante a sessão, geramos clareza prática e acionável sobre cinco dimensões do seu posicionamento.</p>
    <div class="destravar-list">
      <div class="destravar-item"><div class="destravar-num">01</div><p>Quem você é profissionalmente hoje</p></div>
      <div class="destravar-item"><div class="destravar-num">02</div><p>Qual cliente faz sentido atrair — e qual você precisa parar de atrair</p></div>
      <div class="destravar-item"><div class="destravar-num">03</div><p>Onde existe desalinhamento entre sua identidade e sua comunicação</p></div>
      <div class="destravar-item"><div class="destravar-num">04</div><p>Qual direção seguir para se posicionar com mais coerência</p></div>
      <div class="destravar-item"><div class="destravar-num">05</div><p>O que priorizar nos próximos meses para evoluir sua marca pessoal</p></div>
      <div class="destravar-item"><div class="destravar-num" style="font-size:28px;color:#D9C9A8;">↳</div><p style="font-style:italic;color:var(--warm-mid);">Organizar, alinhar e direcionar o que já existe — não criar algo novo.</p></div>
    </div>
  </section>

  <section>
    <div class="section-label">Entregáveis</div>
    <h2>O que você recebe<br>após a sessão</h2>
    <p>Três documentos estratégicos prontos para você começar a aplicar.</p>
    <div class="entregaveis-grid">
      <div class="entregavel">
        <div class="entregavel-num">01</div>
        <div><h3>Documento de Posicionamento Estratégico e Intuitivo</h3><p>Direcionamento claro sobre identidade, temas prioritários, estilo de comunicação, linguagem e plataformas mais alinhadas ao seu momento atual.</p></div>
      </div>
      <div class="entregavel">
        <div class="entregavel-num">02</div>
        <div><h3>Mapa de Cliente Ideal</h3><p>Definição objetiva de quem você deve atrair, como essa pessoa pensa, sente e decide — evitando desgaste com clientes desalinhados e comunicações genéricas.</p></div>
      </div>
      <div class="entregavel">
        <div class="entregavel-num">03</div>
        <div><h3>Plano de Ação para 45 Dias</h3><p>Passo a passo prático para começar a aplicar o posicionamento definido, trazendo foco, constância e coerência para sua marca pessoal.</p></div>
      </div>
    </div>
  </section>

  <section>
    <div class="section-label">Resultado esperado</div>
    <h2>O que muda<br>ao final do processo</h2>
    <div class="resultado-grid">
      <div class="resultado-item"><strong>Clareza</strong><p>Sobre quem você é e como quer se posicionar no mercado</p></div>
      <div class="resultado-item"><strong>Segurança</strong><p>Para se comunicar com autenticidade e intenção</p></div>
      <div class="resultado-item"><strong>Direção</strong><p>Estratégica e prática para iniciar sua próxima fase</p></div>
      <div class="resultado-item"><strong>Menos ruído</strong><p>Menos dúvida, menos dispersão — mais foco e coerência</p></div>
    </div>
  </section>

  <section class="cta-section">
    <div class="section-label">Próximo passo</div>
    <h2>Se essa sessão faz sentido<br>para o seu momento</h2>
    <p style="max-width:480px; margin-bottom:40px;">Seguimos com o agendamento. Uma conversa é suficiente para começar a clareza que você precisa.</p>
    <div class="cta-price">
      <span class="label">Investimento</span>
      <span class="value">R$ 1.297</span>
    </div>
    <p class="cta-note" style="margin-bottom:32px;">Sessão individual · Entregáveis inclusos · Processo completo</p>
    <a href="mailto:contato@isabelarabelo.com.br" class="cta-btn">Quero agendar minha sessão</a>
  </section>

  <section class="sobre-section">
    <div class="section-label">Sobre mim</div>
    <div class="sobre-inner">
      <img class="sobre-photo" src="https://upload.wikimedia.org/wikipedia/commons/8/89/Portrait_Placeholder.png" alt="Isabela Rabelo" onerror="this.style.background='#E8D9BE';this.removeAttribute('src')">
      <div class="sobre-text">
        <h3>Isabela Rabelo</h3>
        <p class="sobre-tagline">Designer · Marketing · Branding · Posicionamento</p>
        <p>Eu sou Isabela Rabelo. Sou graduada em design de moda, onde trabalhei por anos na área de desenvolvimento e criação de roupas e acessórios, pós-graduada em Marketing estratégico, empreendedora e estudiosa do comportamento humano.</p>
        <p>Sou apaixonada pela construção e história de marcas fortes e coerentes e tudo que envolve esse universo. Outra paixão é o desenvolvimento pessoal e como ele reflete nas nossas ações e decisões profissionais.</p>
        <p>Atuo como consultora e mentora de marketing, branding e posicionamento, ajudando pessoas e empresas a construírem uma comunicação de marca clara, estratégica e alinhada à sua essência.</p>
        <p>Minha atuação une visão criativa, pensamento estratégico e experiência prática como empreendedora, traduzindo identidade em posicionamento intuitivo e intencional, comunicação e direção de marca — sem fórmulas prontas. Atuo também no planejamento e produção de conteúdo estratégico.</p>
      </div>
    </div>
  </section>

</div>
</body>
</html>
