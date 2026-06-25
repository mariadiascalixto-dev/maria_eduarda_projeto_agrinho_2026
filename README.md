# maria_eduarda_projeto_agrinho_2026 
public/index.html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Futuro Sustentável – Agricultura Sustentável</title>
  <meta name="description" content="Site escolar sobre agricultura sustentável: práticas, tecnologias e um quiz rápido." />
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header class="header">
    <div class="container header__inner">
      <a href="#inicio" class="header__logo">🌱 Futuro Sustentável</a>
      <nav class="nav">
        <a href="#inicio">Início</a>
        <a href="#sobre">O que é?</a>
        <a href="#praticas">Práticas</a>
        <a href="#tecnologias">Tecnologias</a>
        <a href="#quiz">Quiz</a>
      </nav>
    </div>
  </header>
  <main>
    <section id="inicio" class="hero">
      <div class="container hero__content">
        <span class="badge">Trabalho de IA · 1º ano ADM</span>
        <h1>Agricultura Sustentável</h1>
        <p>Produzir alimentos hoje sem comprometer o amanhã do nosso planeta.</p>
        <a href="#sobre" class="btn">Saiba mais</a>
      </div>
    </section>
    <section id="sobre" class="section">
      <div class="container">
        <h2>O que é agricultura sustentável?</h2>
        <p class="lead">
          A agricultura sustentável busca produzir alimentos de forma responsável,
          preservando os recursos naturais. Com o uso de tecnologias e práticas
          ecológicas, é possível aumentar a produção sem prejudicar o meio ambiente.
        </p>
      </div>
    </section>
    <section id="praticas" class="section section--alt">
      <div class="container">
        <h2>Práticas sustentáveis</h2>
        <div class="grid grid--4">
          <article class="card reveal">
            <div class="card__icon">🌾</div>
            <h3>Rotação de culturas</h3>
            <p>Alternar plantios diferentes na mesma área para manter o solo fértil.</p>
          </article>
          <article class="card reveal">
            <div class="card__icon">💧</div>
            <h3>Irrigação eficiente</h3>
            <p>Sistemas como gotejamento economizam água e levam a quantidade certa às plantas.</p>
          </article>
          <article class="card reveal">
            <div class="card__icon">🍃</div>
            <h3>Adubação orgânica</h3>
            <p>Uso de compostos naturais no lugar de adubos químicos, protegendo o solo.</p>
          </article>
          <article class="card reveal">
            <div class="card__icon">🐞</div>
            <h3>Controle biológico</h3>
            <p>Insetos e fungos do bem combatem pragas sem agrotóxicos.</p>
          </article>
        </div>
      </div>
    </section>
    <section id="tecnologias" class="section">
      <div class="container">
        <h2>Tecnologias no campo</h2>
        <div class="grid grid--3">
          <article class="card reveal">
            <div class="card__icon">📡</div>
            <h3>Sensores no solo</h3>
            <p>Medem umidade e nutrientes em tempo real para evitar desperdícios.</p>
          </article>
          <article class="card reveal">
            <div class="card__icon">☀️</div>
            <h3>Energia solar</h3>
            <p>Painéis solares alimentam bombas e equipamentos sem poluir.</p>
          </article>
          <article class="card reveal">
            <div class="card__icon">🚁</div>
            <h3>Drones agrícolas</h3>
            <p>Monitoram plantações e aplicam insumos só onde é preciso.</p>
          </article>
        </div>
      </div>
    </section>
    <section id="quiz" class="section section--alt">
      <div class="container">
        <h2>Quiz rápido</h2>
        <p class="lead">Teste o que você aprendeu sobre agricultura sustentável.</p>
        <form id="quiz-form" class="quiz"></form>
        <div id="quiz-result" class="quiz__result" hidden></div>
      </div>
    </section>
  </main>
  <footer class="footer">
    <div class="container">
      <p>Feito por <strong>Maria Eduarda</strong> · 1º ano ADM · <span id="year"></span></p>
    </div>
  </footer>
  <script src="script.js"></script>
</body>
</html>
