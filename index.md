<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NeuralHub — Inteligência Artificial</title>
  <meta name="description" content="NeuralHub é um site sobre Inteligência Artificial, Machine Learning e Deep Learning." />

  <style>
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: radial-gradient(circle at top, #020617, #000000);
      color: #f8fafc;
    }

    /* ===== MENU TOPO ===== */
    .topbar {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(0, 0, 0, 0.9);
      backdrop-filter: blur(10px);
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 40px;
      z-index: 1000;
      box-shadow: 0 0 25px rgba(34, 211, 238, 0.15);
    }

    .topbar .logo {
      font-size: 1.4rem;
      font-weight: bold;
      color: #22d3ee;
      text-shadow: 0 0 12px #22d3ee;
    }

    .topbar ul {
      list-style: none;
      display: flex;
      margin: 0;
      padding: 0;
    }

    .topbar ul li {
      margin-left: 25px;
    }

    .topbar ul li a {
      text-decoration: none;
      color: #e5e7eb;
      font-weight: 500;
      transition: all 0.3s ease;
    }

    .topbar ul li a:hover {
      color: #22d3ee;
      text-shadow: 0 0 10px #22d3ee;
    }

    /* ===== HEADER ===== */
    header {
      padding: 140px 20px 80px;
      text-align: center;
    }

    header h1 {
      font-size: 3rem;
      margin-bottom: 10px;
      text-shadow: 0 0 20px #22d3ee;
    }

    header p {
      font-size: 1.2rem;
      color: #94a3b8;
    }

    /* ===== SECTIONS ===== */
    section {
      max-width: 1000px;
      margin: auto;
      padding: 40px 20px;
    }

    .card {
      background: rgba(255,255,255,0.04);
      border-radius: 18px;
      padding: 28px;
      margin-bottom: 28px;
      box-shadow: 0 0 30px rgba(34,211,238,0.12);
      animation: fadeUp 1s ease;
    }

    .card h2 {
      margin-top: 0;
      color: #22d3ee;
      text-shadow: 0 0 10px #22d3ee;
    }

    /* ===== CONTATO ===== */
    form input, form textarea {
      width: 100%;
      padding: 12px;
      margin-bottom: 15px;
      border-radius: 10px;
      border: none;
      background: #020617;
      color: #f8fafc;
    }

    form button {
      background: #22d3ee;
      color: #000;
      border: none;
      padding: 12px 25px;
      border-radius: 10px;
      font-weight: bold;
      cursor: pointer;
      transition: 0.3s;
    }

    form button:hover {
      background: #38bdf8;
      box-shadow: 0 0 15px #22d3ee;
    }

    footer {
      text-align: center;
      padding: 30px;
      color: #94a3b8;
      border-top: 1px solid rgba(255,255,255,0.1);
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>

<body>

<!-- MENU -->
<nav class="topbar">
  <div class="logo">NeuralHub</div>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#ia">IA</a></li>
    <li><a href="sobre.html">Sobre</a></li>
    <li><a href="#contato">Contato</a></li>
  </ul>
</nav>

<!-- HOME -->
<header id="home">
  <h1>NeuralHub</h1>
  <p>Explorando Inteligência Artificial, Machine Learning e Deep Learning</p>
</header>

<!-- IA -->
<section id="ia">
  <div class="card">
    <h2>🧠 Inteligência Artificial</h2>
    <p>A Inteligência Artificial permite que sistemas aprendam, raciocinem e criem soluções inovadoras para problemas complexos.</p>
  </div>

  <div class="card">
    <h2>🤖 Machine Learning</h2>
    <p>Machine Learning é o estudo de algoritmos que aprendem padrões a partir de dados e melhoram com o tempo.</p>
  </div>

  <div class="card">
    <h2>🧠 Deep Learning</h2>
    <p>Deep Learning utiliza redes neurais profundas para visão computacional, linguagem natural e IA generativa.</p>
  </div>
</section>

<!-- CONTATO -->
<section id="contato">
  <div class="card">
    <h2>📩 Contato</h2>
    <p>Email: <strong>denise@gmail.com</strong></p>

    <form>
      <input type="text" placeholder="Seu nome" required />
      <input type="email" placeholder="Seu email" required />
      <textarea rows="4" placeholder="Sua mensagem"></textarea>
      <button type="submit">Enviar</button>
    </form>
  </div>
</section>

<footer>
  NeuralHub © 2025 • Inteligência Artificial e Machine Learning
</footer>

<!-- IDIOMA AUTOMÁTICO -->
<script>
  (function () {
    const lang = navigator.language || navigator.userLanguage;
    const isEnglish = lang.startsWith("en");

    if (isEnglish && !window.location.pathname.includes("index-en")) {
      window.location.href = "index-en.html";
    }
  })();
</script>

</body>
</html>
