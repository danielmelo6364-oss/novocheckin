<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>💎 GÉOR — Check-in de Produtos</title>
<style>
*{box-sizing:border-box;margin:0;padding:0;}
:root{
  --rose:#c9748a;--rose-light:#f7e8ec;--rose-dark:#9e4f63;
  --gold:#b8860b;--dark:#1a1a2e;--brown:#4a3728;
  --text:#2d2d2d;--muted:#9e8575;--bg:#fdf5f7;
}
body{font-family:'Segoe UI',sans-serif;background:var(--bg);color:var(--text);min-height:100vh;padding:16px;}
.container{max-width:1200px;margin:0 auto;}
header{background:linear-gradient(135deg,var(--dark),var(--rose-dark));color:#fff;padding:24px;border-radius:16px;margin-bottom:24px;box-shadow:0 8px 24px rgba(0,0,0,.2);}
.h-title{font-size:32px;font-weight:900;letter-spacing:2px;margin-bottom:4px;}
.h-sub{font-size:13px;opacity:.85;}
.tabs{display:flex;gap:8px;margin-bottom:24px;flex-wrap:wrap;}
.tab-btn{padding:12px 20px;border:none;border-radius:10px;background:#fff;color:var(--rose-dark);font-weight:700;cursor:pointer;font-size:14px;transition:all .2s;box-shadow:0 2px 8px rgba(0,0,0,.06);}
.tab-btn.active{background:linear-gradient(135deg,var(--rose),var(--rose-dark));color:#fff;}
.tab-btn:hover{transform:translateY(-2px);}
.tab-content{display:none;}
.tab-content.active{display:block;}
.card{background:#fff;border-radius:16px;padding:24px;box-shadow:0 4px 20px rgba(0,0,0,.08);margin-bottom:20px;}
.card h2{font-size:18px;font-weight:700;color:var(--brown);margin-bottom:16px;padding-bottom:12px;border-bottom:2px solid var(--rose-light);}
.form-group{margin-bottom:16px;}
.form-group label{display:block;font-size:12px;font-weight:700;color:var(--rose-dark);margin-bottom:6px;text-transform:uppercase;letter-spacing:.5px;}
input[type=text],input[type=number],input[type=date],select,textarea{width:100%;padding:11px 14px;border:1.5px solid #e0d0d5;border-radius:10px;font-size:14px;color:var(--text);background:#fdf5f7;transition:border-color .2s;font-family:inherit;}
input:focus,select:focus,textarea:focus{outline:none;border-color:var(--rose);background:#fff;}
.grid2{display:grid;grid-template-columns:1fr 1fr;gap:16px;}
.grid3{display:grid;grid-template-columns:1fr 1fr 1fr;gap:16px;}
@media(max-width:768px){.grid2,.grid3{grid-template-columns:1fr;}}
.foto-upload{border:2px dashed #e0c0cc;border-radius:12px;padding:24px;text-align:center;cursor:pointer;background:#fdf5f7;transition:all .2s;}
.foto-upload:hover{border-color:var(--rose);background:#fff;}
.foto-upload input{display:none;}
.foto-icon{font-size:32px;margin-bottom:8px;}
.foto-text{font-size:12px;color:var(--muted);}
#preview-img{width:100%;max-height:200px;object-fit:cover;border-radius:10px;margin-top:12px;display:none;}
.cores-container{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:12px;}
.cor-item{display:flex;align-items:center;gap:8px;background:#fff;border:1.5px solid #e0d0d5;border-radius:8px;padding:8px 12px;font-size:13px;}
.cor-item button{background:#dc3545;color:#fff;border:none;border-radius:4px;padding:2px 8px;cursor:pointer;font-size:11px;font-weight:700;}
.cor-input{display:flex;gap:8px;align-items:flex-end;}
.cor-input input{flex:1;}
.cor-input button{background:linear-gradient(135deg,var(--rose),var(--rose-dark));color:#fff;border:none;padding:10px 16px;border-radius:8px;cursor:pointer;font-weight:700;font-size:13px;}
.btn-primary{width:100%;padding:13px;border:none;border-radius:10px;background:linear-gradient(135deg,var(--rose),var(--rose-dark));color:#fff;font-size:15px;font-weight:700;cursor:pointer;box-shadow:0 4px 14px rgba(201,116,138,.35);transition:transform .1s;}
.btn-primary:hover{transform:translateY(-2px);}
.produtos-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:16px;}
.produto-card{background:#fff;border-radius:12px;padding:16px;box-shadow:0 2px 12px rgba(0,0,0,.08);border-left:4px solid var(--rose);}
.produto-card img{width:100%;height:160px;object-fit:cover;border-radius:8px;margin-bottom:12px;}
.produto-card .no-img{width:100%;height:160px;background:var(--rose-light);border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:48px;margin-bottom:12px;}
.produto-card h3{font-size:14px;font-weight:700;margin-bottom:4px;}
.produto-card .ref{font-size:11px;color:var(--muted);font-family:monospace;margin-bottom:8px;}
.produto-card .tipo{display:inline-block;background:var(--rose-light);color:var(--rose-dark);padding:2px 8px;border-radius:6px;font-size:10px;font-weight:700;margin-bottom:8px;}
.produto-card .cores-list{font-size:11px;color:var(--muted);margin-bottom:8px;}
.produto-card .preco{font-size:16px;font-weight:800;color:var(--rose-dark);margin-bottom:8px;}
.produto-card .btns{display:flex;gap:6px;}
.btn-sm{flex:1;padding:8px;border:none;border-radius:6px;font-size:12px;font-weight:700;cursor:pointer;transition:all .2s;}
.btn-delete{background:#dc3545;color:#fff;}
.btn-sm:hover{transform:translateY(-1px);}
.stats-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:12px;margin-bottom:16px;}
.stat-box{background:linear-gradient(135deg,var(--rose-light),#fff);border-left:4px solid var(--rose);border-radius:10px;padding:16px;text-align:center;}
.stat-box .num{font-size:28px;font-weight:800;color:var(--rose-dark);}
.stat-box .lbl{font-size:11px;color:var(--muted);margin-top:4px;text-transform:uppercase;}
.empty{text-align:center;padding:40px 20px;color:var(--muted);}
.empty-icon{font-size:48px;margin-bottom:12px;}
.toast{position:fixed;bottom:24px;right:24px;background:var(--dark);color:#fff;padding:12px 20px;border-radius:10px;font-size:13px;font-weight:600;opacity:0;transform:translateY(8px);transition:all .3s;z-index:999;pointer-events:none;}
.toast.show{opacity:1;transform:translateY(0);}
.relatorio-filtros{display:flex;gap:12px;flex-wrap:wrap;margin-bottom:16px;align-items:flex-end;}
.relatorio-filtros .form-group{margin-bottom:0;flex:1;min-width:150px;}
.relatorio-table{width:100%;border-collapse:collapse;font-size:13px;}
.relatorio-table th{background:var(--rose-light);color:var(--rose-dark);padding:12px;text-align:left;font-weight:700;border-bottom:2px solid var(--rose);}
.relatorio-table td{padding:12px;border-bottom:1px solid #f0e0e5;}
.relatorio-table tr:hover td{background:#fdf5f7;}
</style>
</head>
<body>

<div class="container">
  <header>
    <div class="h-title">💎 GÉOR — Check-in de Produtos</div>
    <div class="h-sub">Registre suas semijoias, bijuterias e acessórios com variações de cores</div>
  </header>

  <div class="tabs">
    <button class="tab-btn active" onclick="abrirAba('checkin')">📦 Check-in</button>
    <button class="tab-btn" onclick="abrirAba('produtos')">🗂️ Produtos</button>
    <button class="tab-btn" onclick="abrirAba('relatorio')">📊 Relatório</button>
  </div>

  <!-- ABA CHECK-IN -->
  <div id="checkin" class="tab-content active">
    <div class="card">
      <h2>📸 Novo Registro de Produto</h2>

      <div class="form-group">
        <label>Foto do Produto</label>
        <div class="foto-upload" onclick="document.getElementById('foto-input').click()">
          <input type="file" id="foto-input" accept="image/*" capture="environment"/>
          <div class="foto-icon">📷</div>
          <div class="foto-text">Clique para adicionar foto</div>
          <img id="preview-img" alt=""/>
        </div>
      </div>

      <div class="form-group">
        <label>Nome / Descrição *</label>
        <input type="text" id="f-nome" placeholder="Ex: Anel Solitário Banhado a Ouro"/>
      </div>

      <div class="grid2">
        <div class="form-group">
          <label>Código / Referência *</label>
          <input type="text" id="f-ref" placeholder="Ex: GR-001"/>
        </div>
        <div class="form-group">
          <label>Tipo *</label>
          <select id="f-tipo">
            <option value="">Selecione...</option>
            <option>Bijuteria</option>
            <option>Prata 925</option>
            <option>Semijoia</option>
            <option>Bolsa</option>
            <option>Óculos</option>
            <option>Relógios</option>
          </select>
        </div>
      </div>

      <div class="form-group">
        <label>Fornecedor</label>
        <input type="text" id="f-forn" placeholder="Nome do fornecedor"/>
      </div>

      <div class="grid2">
        <div class="form-group">
          <label>Preço de Custo (R$)</label>
          <input type="number" id="f-custo" min="0" step="0.01" placeholder="0,00"/>
        </div>
        <div class="form-group">
          <label>Preço de Venda (R$)</label>
          <input type="number" id="f-preco" min="0" step="0.01" placeholder="0,00"/>
        </div>
      </div>

      <div class="form-group">
        <label>Variações de Cores *</label>
        <div class="cores-container" id="cores-list"></div>
        <div class="cor-input">
          <input type="text" id="cor-input" placeholder="Ex: Ouro, Prata, Rose..."/>
          <button type="button" onclick="adicionarCor()">+ Adicionar</button>
        </div>
      </div>

      <div class="grid3">
        <div class="form-group">
          <label>Qtd. Gôndola</label>
          <input type="number" id="f-gondola" min="0" placeholder="0"/>
        </div>
        <div class="form-group">
          <label>Qtd. Estoque</label>
          <input type="number" id="f-estoque" min="0" placeholder="0"/>
        </div>
        <div class="form-group">
          <label>Alertar abaixo de</label>
          <input type="number" id="f-alerta" min="0" placeholder="5"/>
        </div>
      </div>

      <div class="form-group">
        <label>Observações</label>
        <textarea id="f-obs" placeholder="Tamanho, coleção, material..." style="min-height:80px;"></textarea>
      </div>

      <button class="btn-primary" type="button" onclick="registrarProduto()">✅ Registrar Check-in</button>
    </div>
  </div>

  <!-- ABA PRODUTOS -->
  <div id="produtos" class="tab-content">
    <div class="card">
      <h2>🗂️ Produtos Registrados</h2>

      <div class="relatorio-filtros">
        <div class="form-group" style="flex:1;min-width:150px;">
          <label>Filtrar por Tipo</label>
          <select id="filtro-tipo" onchange="renderProdutos()">
            <option value="">Todos</option>
            <option>Bijuteria</option>
            <option>Prata 925</option>
            <option>Semijoia</option>
            <option>Bolsa</option>
            <option>Óculos</option>
            <option>Relógios</option>
          </select>
        </div>
        <div class="form-group" style="flex:1;min-width:150px;">
          <label>Buscar</label>
          <input type="text" id="filtro-busca" placeholder="Nome ou código..." onkeyup="renderProdutos()"/>
        </div>
      </div>

      <div class="stats-grid" id="stats-produtos"></div>
      <div class="produtos-grid" id="produtos-grid"></div>
      <div id="produtos-empty" class="empty" style="display:none;">
        <div class="empty-icon">📦</div>
        <p>Nenhum produto registrado ainda</p>
      </div>
    </div>
  </div>

  <!-- ABA RELATÓRIO -->
  <div id="relatorio" class="tab-content">
    <div class="card">
      <h2>📊 Relatório de Produtos</h2>

      <div class="stats-grid" id="stats-relatorio"></div>

      <div style="overflow-x:auto;">
        <table class="relatorio-table" id="relatorio-table">
          <thead>
            <tr>
              <th>Data</th>
              <th>Código</th>
              <th>Produto</th>
              <th>Tipo</th>
              <th>Cores</th>
              <th>Gôndola</th>
              <th>Estoque</th>
              <th>Preço Venda</th>
            </tr>
          </thead>
          <tbody id="relatorio-tbody"></tbody>
        </table>
      </div>
    </div>
  </div>
</div>

<div id="toast" class="toast"></div>

<script src="https://www.gstatic.com/firebasejs/10.7.0/firebase-app.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.7.0/firebase-database.js"></script>

<script>
// ══════════ FIREBASE CONFIG ══════════
const firebaseConfig = {
  apiKey: "AIzaSyDnMsL-dhv3uM2tP3B-IcJUFHVo1MmoW2k",
  authDomain: "checkin-4760f.firebaseapp.com",
  projectId: "checkin-4760f",
  storageBucket: "checkin-4760f.firebasestorage.app",
  messagingSenderId: "207981324873",
  appId: "1:207981324873:web:00ccce2c26033b3f966d98",
  databaseURL: "https://checkin-4760f-default-rtdb.firebaseio.com"
};

firebase.initializeApp(firebaseConfig);
const db = firebase.database();

let coresTemp = [];
const moeda = v => 'R$ ' + parseFloat(v || 0).toFixed(2).replace('.', ',');
const fmtData = s => new Date(s).toLocaleDateString('pt-BR');
let fotoB64 = null;

function toast(msg, dur = 3000) {
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  setTimeout(() => t.classList.remove('show'), dur);
}

function abrirAba(aba) {
  document.querySelectorAll('.tab-content').forEach(el => el.classList.remove('active'));
  document.querySelectorAll('.tab-btn').forEach(el => el.classList.remove('active'));
  document.getElementById(aba).classList.add('active');
  event.target.classList.add('active');

  if (aba === 'produtos') renderProdutos();
  if (aba === 'relatorio') gerarRelatorio();
}

// ══════════ FOTO ══════════
document.getElementById('foto-input').addEventListener('change', function(e) {
  const f = e.target.files[0];
  if (!f) return;
  const r = new FileReader();
  r.onload = ev => {
    fotoB64 = ev.target.result;
    const img = document.getElementById('preview-img');
    img.src = fotoB64;
    img.style.display = 'block';
  };
  r.readAsDataURL(f);
});

// ══════════ CORES ══════════
function adicionarCor() {
  const cor = document.getElementById('cor-input').value.trim();
  if (!cor) {
    toast('⚠️ Digite uma cor');
    return;
  }
  if (coresTemp.includes(cor)) {
    toast('⚠️ Cor já adicionada');
    return;
  }
  coresTemp.push(cor);
  renderCores();
  document.getElementById('cor-input').value = '';
}

function removerCor(idx) {
  coresTemp.splice(idx, 1);
  renderCores();
}

function renderCores() {
  const el = document.getElementById('cores-list');
  el.innerHTML = coresTemp.map((cor, i) => `
    <div class="cor-item">
      ${cor}
      <button type="button" onclick="removerCor(${i})">✕</button>
    </div>
  `).join('');
}

// ══════════ REGISTRAR ══════════
async function registrarProduto() {
  const nome = document.getElementById('f-nome').value.trim();
  const ref = document.getElementById('f-ref').value.trim();
  const tipo = document.getElementById('f-tipo').value;
  const forn = document.getElementById('f-forn').value.trim();
  const custo = parseFloat(document.getElementById('f-custo').value) || 0;
  const preco = parseFloat(document.getElementById('f-preco').value) || 0;
  const gondola = parseInt(document.getElementById('f-gondola').value) || 0;
  const estoque = parseInt(document.getElementById('f-estoque').value) || 0;
  const alerta = parseInt(document.getElementById('f-alerta').value) || 5;
  const obs = document.getElementById('f-obs').value.trim();

  if (!nome) { toast('⚠️ Informe o nome'); return; }
  if (!ref) { toast('⚠️ Informe o código'); return; }
  if (!tipo) { toast('⚠️ Selecione o tipo'); return; }
  if (coresTemp.length === 0) { toast('⚠️ Adicione uma cor'); return; }
  if (gondola === 0 && estoque === 0) { toast('⚠️ Informe uma quantidade'); return; }

  const produto = {
    data: new Date().toISOString(),
    nome, ref, tipo, forn, custo, preco, gondola, estoque, alerta, obs,
    cores: coresTemp,
    foto: fotoB64 || null
  };

  try {
    await db.ref('produtos').push(produto);
    document.getElementById('f-nome').value = '';
    document.getElementById('f-ref').value = '';
    document.getElementById('f-tipo').value = '';
    document.getElementById('f-forn').value = '';
    document.getElementById('f-custo').value = '';
    document.getElementById('f-preco').value = '';
    document.getElementById('f-gondola').value = '';
    document.getElementById('f-estoque').value = '';
    document.getElementById('f-alerta').value = '';
    document.getElementById('f-obs').value = '';
    document.getElementById('preview-img').style.display = 'none';
    document.getElementById('foto-input').value = '';
    coresTemp = [];
    renderCores();
    fotoB64 = null;
    toast('✅ Produto registrado!');
  } catch (err) {
    toast('❌ Erro: ' + err.message);
  }
}

// ══════════ RENDER PRODUTOS ══════════
function renderProdutos() {
  const tipo = document.getElementById('filtro-tipo').value;
  const busca = document.getElementById('filtro-busca').value.toLowerCase();

  db.ref('produtos').once('value', (snapshot) => {
    const dados = snapshot.val();
    let lista = dados ? Object.entries(dados).map(([key, val]) => ({firebaseId: key, ...val})) : [];

    if (tipo) lista = lista.filter(p => p.tipo === tipo);
    if (busca) lista = lista.filter(p => p.nome.toLowerCase().includes(busca) || p.ref.toLowerCase().includes(busca));

    const stats = document.getElementById('stats-produtos');
    const grid = document.getElementById('produtos-grid');
    const empty = document.getElementById('produtos-empty');

    if (!lista.length) {
      empty.style.display = 'block';
      grid.innerHTML = '';
      stats.innerHTML = '';
      return;
    }

    empty.style.display = 'none';
    const total = lista.length;
    const totalItens = lista.reduce((a, p) => a + p.gondola + p.estoque, 0);
    const totalValor = lista.reduce((a, p) => a + (p.preco || 0) * (p.gondola + p.estoque), 0);

    stats.innerHTML = `
      <div class="stat-box"><div class="num">${total}</div><div class="lbl">Produtos</div></div>
      <div class="stat-box"><div class="num">${totalItens}</div><div class="lbl">Itens</div></div>
      <div class="stat-box"><div class="num">${moeda(totalValor)}</div><div class="lbl">Valor Total</div></div>`;

    grid.innerHTML = lista.map(p => `
      <div class="produto-card">
        ${p.foto ? `<img src="${p.foto}" alt="${p.nome}"/>` : `<div class="no-img">💍</div>`}
        <h3>${p.nome}</h3>
        <div class="ref">${p.ref}</div>
        <div class="tipo">${p.tipo}</div>
        <div class="cores-list">🎨 ${p.cores.join(', ')}</div>
        <div class="preco">${moeda(p.preco)}</div>
        <div style="font-size:11px;color:var(--muted);margin-bottom:8px;">🛒 ${p.gondola} | 📦 ${p.estoque}</div>
        <div class="btns">
          <button class="btn-sm btn-delete" onclick="deletarProduto('${p.firebaseId}')">🗑️ Deletar</button>
        </div>
      </div>
    `).join('');
  });
}

async function deletarProduto(id) {
  if (!confirm('Deletar este produto?')) return;
  try {
    await db.ref(`produtos/${id}`).remove();
    toast('✅ Deletado!');
    renderProdutos();
  } catch (err) {
    toast('❌ Erro ao deletar');
  }
}

// ══════════ RELATÓRIO ══════════
function gerarRelatorio() {
  db.ref('produtos').once('value', (snapshot) => {
    const dados = snapshot.val();
    let lista = dados ? Object.entries(dados).map(([key, val]) => ({firebaseId: key, ...val})) : [];

    const stats = document.getElementById('stats-relatorio');
    const total = lista.length;
    const totalItens = lista.reduce((a, p) => a + p.gondola + p.estoque, 0);
    const totalValor = lista.reduce((a, p) => a + (p.preco || 0) * (p.gondola + p.estoque), 0);

    stats.innerHTML = `
      <div class="stat-box"><div class="num">${total}</div><div class="lbl">Produtos</div></div>
      <div class="stat-box"><div class="num">${totalItens}</div><div class="lbl">Itens</div></div>
      <div class="stat-box"><div class="num">${moeda(totalValor)}</div><div class="lbl">Valor Total</div></div>`;

    const tbody = document.getElementById('relatorio-tbody');
    tbody.innerHTML = lista.map(p => `
      <tr>
        <td>${fmtData(p.data)}</td>
        <td>${p.ref}</td>
        <td>${p.nome}</td>
        <td>${p.tipo}</td>
        <td>${p.cores.join(', ')}</td>
        <td>${p.gondola}</td>
        <td>${p.estoque}</td>
        <td>${moeda(p.preco)}</td>
      </tr>
    `).join('');
  });
}
</script>

</body>
</html>
