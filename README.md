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

root {
  --green-900: #1b4332;
  --green-700: #2d6a4f;
  --green-500: #52b788;
  --green-100: #d8f3dc;
  --sand: #f7f4ea;
  --text: #1f2d28;
  --muted: #5b6b63;
  --white: #ffffff;
  --shadow: 0 6px 20px rgba(27, 67, 50, 0.08);
  --radius: 14px;
}
* { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }
body {
  font-family: system-ui, -apple-system, "Segoe UI", Roboto, sans-serif;
  color: var(--text);
  background: var(--sand);
  line-height: 1.6;
}
.container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 1.25rem;
}
/* Header */
.header {
  position: sticky;
  top: 0;
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(8px);
  border-bottom: 1px solid var(--green-100);
  z-index: 10;
}
.header__inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.9rem 1.25rem;
}
.header__logo {
  font-weight: 700;
  color: var(--green-900);
  text-decoration: none;
  font-size: 1.1rem;
}
.nav {
  display: flex;
  gap: 1.25rem;
  flex-wrap: wrap;
}
.nav a {
  color: var(--green-900);
  text-decoration: none;
  font-weight: 500;
  font-size: 0.95rem;
}
.nav a:hover { color: var(--green-500); }
/* Hero */
.hero {
  background:
    linear-gradient(rgba(27, 67, 50, 0.55), rgba(27, 67, 50, 0.55)),
    url("https://images.unsplash.com/photo-1500595046743-cd271d694d30?auto=format&fit=crop&w=1600&q=80") center/cover no-repeat;
  color: var(--white);
  padding: 6rem 0;
  text-align: center;
}
.hero__content { max-width: 720px; margin: 0 auto; }
.badge {
  display: inline-block;
  background: rgba(255, 255, 255, 0.15);
  border: 1px solid rgba(255, 255, 255, 0.4);
  padding: 0.3rem 0.8rem;
  border-radius: 999px;
  font-size: 0.85rem;
  margin-bottom: 1rem;
}
.hero h1 {
  font-size: clamp(2rem, 5vw, 3.5rem);
  margin-bottom: 1rem;
}
.hero p {
  font-size: 1.15rem;
  margin-bottom: 1.75rem;
  opacity: 0.95;
}
.btn {
  display: inline-block;
  background: var(--green-500);
  color: var(--white);
  text-decoration: none;
  padding: 0.85rem 1.6rem;
  border-radius: var(--radius);
  font-weight: 600;
  border: none;
  cursor: pointer;
  transition: transform 0.15s ease, background 0.15s ease;
}
.btn:hover { background: var(--green-700); transform: translateY(-2px); }
/* Sections */
.section { padding: 4rem 0; }
.section--alt { background: var(--green-100); }
.section h2 {
  color: var(--green-900);
  font-size: clamp(1.5rem, 3vw, 2.2rem);
  margin-bottom: 1.25rem;
}
.lead { color: var(--muted); font-size: 1.05rem; max-width: 760px; }
/* Grid + Cards */
.grid {
  display: grid;
  gap: 1.25rem;
  margin-top: 2rem;
}
.grid--3 { grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); }
.grid--4 { grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); }
.card {
  background: var(--white);
  padding: 1.5rem;
  border-radius: var(--radius);
  box-shadow: var(--shadow);
  border: 1px solid rgba(45, 106, 79, 0.08);
  opacity: 0;
  transform: translateY(20px);
  transition: opacity 0.5s ease, transform 0.5s ease;
}
.card.is-visible { opacity: 1; transform: translateY(0); }
.card__icon { font-size: 2rem; margin-bottom: 0.75rem; }
.card h3 { color: var(--green-700); margin-bottom: 0.5rem; }
.card p { color: var(--muted); font-size: 0.95rem; }
/* Quiz */
.quiz { margin-top: 2rem; display: grid; gap: 1.5rem; }
.quiz__question {
  background: var(--white);
  padding: 1.25rem 1.5rem;
  border-radius: var(--radius);
  box-shadow: var(--shadow);
}
.quiz__question h3 {
  color: var(--green-900);
  margin-bottom: 0.75rem;
  font-size: 1.05rem;
}
.quiz__options { display: grid; gap: 0.5rem; }
.quiz__option {
  display: flex;
  align-items: center;
  gap: 0.6rem;
  padding: 0.6rem 0.8rem;
  border: 1px solid var(--green-100);
  border-radius: 10px;
  cursor: pointer;
  transition: background 0.15s ease;
}
.quiz__option:hover { background: var(--green-100); }
.quiz__option input { accent-color: var(--green-700); }
.quiz__actions { display: flex; gap: 0.75rem; flex-wrap: wrap; }
.quiz__result {
  margin-top: 1.5rem;
  background: var(--white);
  padding: 1.25rem 1.5rem;
  border-radius: var(--radius);
  box-shadow: var(--shadow);
  border-left: 5px solid var(--green-500);
}
/* Footer */
.footer {
  background: var(--green-900);
  color: var(--white);
  text-align: center;
  padding: 1.5rem 0;
  margin-top: 2rem;
}
.footer strong { color: var(--green-100); }
@media (max-width: 600px) {
  .nav { gap: 0.75rem; }
  .nav a { font-size: 0.85rem; }
  .hero { padding: 4rem 0; }

public/script.js
// Ano atual no rodapé
document.getElementById("year").textContent = new Date().getFullYear();
// Animação dos cards ao aparecer na tela
const observer = new IntersectionObserver(
  (entries) => {
    entries.forEach((entry) => {
      if (entry.isIntersecting) {
        entry.target.classList.add("is-visible");
        observer.unobserve(entry.target);
      }
    });
  },
  { threshold: 0.15 }
);
document.querySelectorAll(".reveal").forEach((el) => observer.observe(el));
// Quiz
const perguntas = [
  {
    q: "O que é agricultura sustentável?",
    opcoes: [
      "Produzir o máximo possível, sem se preocupar com o meio ambiente.",
      "Produzir alimentos preservando os recursos naturais.",
      "Plantar apenas em estufas fechadas.",
    ],
    correta: 1,
  },
  {
    q: "Qual prática ajuda a manter o solo fértil?",
    opcoes: [
      "Rotação de culturas",
      "Uso intenso de agrotóxicos",
      "Queimar a vegetação",
    ],
    correta: 0,
  },
  {
    q: "Qual tecnologia ajuda a economizar água na lavoura?",
    opcoes: [
      "Irrigação por gotejamento",
      "Inundar o terreno todos os dias",
      "Regar somente à noite e à vontade",
    ],
    correta: 0,
  },
];
const form = document.getElementById("quiz-form");
const result = document.getElementById("quiz-result");
function renderQuiz() {
  form.innerHTML = "";
  result.hidden = true;
  result.innerHTML = "";
  perguntas.forEach((p, i) => {
    const bloco = document.createElement("div");
    bloco.className = "quiz__question";
    bloco.innerHTML = `
      <h3>${i + 1}. ${p.q}</h3>
      <div class="quiz__options">
        ${p.opcoes
          .map(
            (op, j) => `
          <label class="quiz__option">
            <input type="radio" name="q${i}" value="${j}" />
            <span>${op}</span>
          </label>`
          )
          .join("")}
      </div>
    `;
    form.appendChild(bloco);
  });
  const acoes = document.createElement("div");
  acoes.className = "quiz__actions";
  acoes.innerHTML = `<button type="submit" class="btn">Ver resultado</button>`;
  form.appendChild(acoes);
}
form.addEventListener("submit", (e) => {
  e.preventDefault();
  let acertos = 0;
  perguntas.forEach((p, i) => {
    const escolha = form.querySelector(`input[name="q${i}"]:checked`);
    if (escolha && Number(escolha.value) === p.correta) acertos++;
  });
  const total = perguntas.length;
  let msg = "";
  if (acertos === total) msg = "🌟 Excelente! Você é uma defensora do planeta!";
  else if (acertos >= total / 2) msg = "🌱 Muito bem! Você está no caminho certo.";
  else msg = "💡 Continue estudando — todo gesto sustentável conta!";
  result.innerHTML = `
    <h3>Você acertou ${acertos} de ${total}</h3>
    <p>${msg}</p>
    <button type="button" class="btn" id="quiz-reset" style="margin-top:1rem;">Refazer quiz</button>
  `;
  result.hidden = false;
  result.scrollIntoView({ behavior: "smooth", block: "center" });
  document.getElementById("quiz-reset").addEventListener("click", renderQuiz);
});
renderQuiz();

