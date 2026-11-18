<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>DUDU22Filmes · Sua coleção de filmes</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header class="hero">
  <nav><span class="logo">DUDU22<b>Filmes</b></span><button class="btn" onclick="abrir()">+ Novo filme</button></nav>
  <div class="hero-txt">
    <p class="tag">Em cartaz · Novembro 2026</p>
    <h1>Sua coleção de filmes, <span>do seu jeito.</span></h1>
    <p class="sub">Cadastre, avalie, edite e organize o que você quer ver e o que já assistiu.</p>
  </div>
  <div class="stats">
    <div><strong id="s-total">0</strong><span>filmes</span></div>
    <div><strong id="s-vistos">0</strong><span>assistidos</span></div>
    <div><strong id="s-nota">–</strong><span>nota média</span></div>
  </div>
</header>

<main>
  <div class="tools">
    <input id="busca" type="search" placeholder="Buscar por título ou gênero..." oninput="render()">
    <div class="chips" id="chips">
      <button class="chip on" data-f="todos">Todos</button>
      <button class="chip" data-f="quero">Quero ver</button>
      <button class="chip" data-f="visto">Assistidos</button>
    </div>
    <select id="ordem" onchange="render()">
      <option value="recente">Mais recentes</option>
      <option value="nota">Maior nota</option>
      <option value="titulo">A–Z</option>
    </select>
  </div>
  <section id="grade" class="grade"></section>
  <p id="vazio" class="vazio" hidden>Nenhum filme encontrado. Que tal adicionar um?</p>
</main>

<dialog id="modal">
  <form id="form" onsubmit="salvar(event)">
    <h2 id="m-titulo">Novo filme</h2>
    <label>Título<input id="f-titulo" required maxlength="60"></label>
    <div class="duas">
      <label>Gênero<input id="f-genero" required maxlength="25" placeholder="Ação, Drama..."></label>
      <label>Ano<input id="f-ano" type="number" min="1900" max="2100" value="2026" required></label>
    </div>
    <label>Nota: <b id="f-nota-v">7</b>/10<input id="f-nota" type="range" min="0" max="10" value="7" oninput="document.getElementById('f-nota-v').textContent=this.value"></label>
    <label>Status
      <select id="f-status"><option value="quero">Quero ver</option><option value="visto">Já assisti</option></select>
    </label>
    <div class="acoes">
      <button type="button" class="btn ghost" onclick="fechar()">Cancelar</button>
      <button class="btn">Salvar</button>
    </div>
  </form>
</dialog>

<div id="toast" class="toast"></div>
<footer>© 2026 DUDU22Filmes · Dados salvos no seu navegador</footer>
<script src="script.js"></script>
</body>
</html>
