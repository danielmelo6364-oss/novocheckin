<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>💎 GÉOR — Check-in de Produtos</title>
<style>
*{box-sizing:border-box;margin:0;padding:0;}
:root{--rose:#c9748a;--rose-light:#f7e8ec;--rose-dark:#9e4f63;--dark:#1a1a2e;--brown:#4a3728;--text:#2d2d2d;--muted:#9e8575;--bg:#fdf5f7;}
body{font-family:'Segoe UI',sans-serif;background:var(--bg);color:var(--text);min-height:100vh;padding:16px;}
.container{max-width:1200px;margin:0 auto;}
header{background:linear-gradient(135deg,var(--dark),var(--rose-dark));color:#fff;padding:24px;border-radius:16px;margin-bottom:24px;}
.h-title{font-size:32px;font-weight:900;margin-bottom:4px;}
.h-sub{font-size:13px;opacity:.85;}
.tabs{display:flex;gap:8px;margin-bottom:24px;flex-wrap:wrap;}
.tab-btn{padding:12px 20px;border:none;border-radius:10px;background:#fff;color:var(--rose-dark);font-weight:700;cursor:pointer;font-size:14px;}
.tab-btn.active{background:linear-gradient(135deg,var(--rose),var(--rose-dark));color:#fff;}
.tab-content{display:none;}
.tab-content.active{display:block;}
.card{background:#fff;border-radius:16px;padding:24px;box-shadow:0 4px 20px rgba(0,0,0,.08);margin-bottom:20px;}
.card h2{font-size:18px;font-weight:700;color:var(--brown);margin-bottom:16px;padding-bottom:12px;border-bottom:2px solid var(--rose-light);}
.form-group{margin-bottom:16px;}
.form-group label{display:block;font-size:12px;font-weight:700;color:var(--rose-dark);margin-bottom:6px;text-transform:uppercase;}
input[type=text],input[type=number],select,textarea{width:100%;padding:11px 14px;border:1.5px solid #e0d0d5;border-radius:10px;font-size:14px;color:var(--text);background:#fdf5f7;font-family:inherit;}
input:focus,select:focus,textarea:focus{outline:none;border-color:var(--rose);background:#fff;}
.grid2{display:grid;grid-template-columns:1fr 1fr;gap:16px;}
@media(max-width:768px){.grid2{grid-template-columns:1fr;}}
.foto-upload{border:2px dashed #e0c0cc;border-radius:12px;padding:24px;text-align:center;cursor:pointer;background:#fdf5f7;}
.foto-upload:hover{border-color:var(--rose);}
.foto-upload input{display:none;}
.foto-icon{font-size:32px;margin-bottom:8px;}
.foto-text{font-size:12px;color:var(--muted);}
#preview-img{width:100%;max-height:200px;object-fit:cover;border-radius:10px;margin-top:12px;display:none;}
.cores-container{display:flex;flex-direction:column;gap:12px;margin-bottom:16px;}
.cor-item{background:#fdf5f7;border:1.5px solid #e0d0d5;border-radius:10px;padding:12px;}
.cor-item-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:8px;}
.cor-item-nome{font-weight:700;color:var(--rose-dark);}
.cor-item-btn{background:#dc3545;color:#fff;border:none;border-radius:4px;padding:4px 8px;cursor:pointer;font-size:11px;font-weight:700;}
.cor-qtd-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;}
.cor-qtd-grid input{font-size:12px;padding:8px;}
.cor-qtd-grid label{font-size:10px;color:var(--muted);margin-bottom:2px;}
.cor-input{display:flex;gap:8px;align-items:flex-end;}
.cor-input input{flex:1;}
.cor-input button{background:linear-gradient(135deg,var(--rose),var(--rose-dark));color:#fff;border:none;padding:10px 16px;border-radius:8px;cursor:pointer;font-weight:700;font-size:13px;}
.btn-primary{width:100%;padding:13px;border:none;border-radius:10px;background:linear-gradient(135deg,var(--rose),var(--rose-dark));color:#fff;font-size:15px;font-weight:700;cursor:pointer;}
.btn-primary:hover{opacity:.9;}
.produtos-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:16px;}
.produto-card{background:#fff;border-radius:12px;padding:16px;box-shadow:0 2px 12px rgba(0,0,0,.08);border-left:4px solid var(--rose);}
.produto-card img{width:100%;height:160px;object-fit:cover;border-radius:8px;margin-bottom:12px;}
.produto-card .no-img{width:100%;height:160px;background:var(--rose-light);border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:48px;margin-bottom:12px;}
.produto-card h3{font-size:14px;font-weight:700;margin-bottom:4px;}
.produto-card .ref{font-size:11px;color:var(--muted);margin-bottom:8px;}
.produto-card .tipo{display:inline-block;background:var(--rose-light);color:var(--rose-dark);padding:2px 8px;border-radius:6px;font-size:10px;font-weight:700;margin-bottom:8px;}
.produto-card .preco{font-size:16px;font-weight:800;color:var(--rose-dark);margin-bottom:8px;}
.cor-info{font-size:11px;color:var(--muted);margin-bottom:4px;padding:4px;background:var(--rose-light);border-radius:4px;}
.btn-delete{background:#dc3545;color:#fff;border:none;padding:8px 12px;border-radius:6px;cursor:pointer;font-size:12px;font-weight:700;width:100%;}
.stats-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:12px;margin-bottom:16px;}
.stat-box{background:linear-gradient(135deg,var(--rose-light),#fff);border-left:4px solid var(--rose);border-radius:10px;padding:16px;text-align:center;}
.stat-box .num{font-size:28px;font-weight:800;color:var(--rose-dark);}
.stat-box .lbl{font-size:11px;color:var(--muted);margin-top:4px;}
.empty{text-align:center;padding:40px 20px;color:var(--muted);}
.empty-icon{font-size:48px;margin-bottom:12px;}
.toast{position:fixed;bottom:24px;right:24px;background:var(--dark);color:#fff;padding:12px 20px;border-radius:10px;font-size:13px;font-weight:600;opacity:0;transform:translateY(8px);transition:all .3s;z-index:999;}
.toast.show{opacity:1;transform:translateY(0);}
</style>
</head>
<body>

<div class="container">
  <header>
    <div class="h-title">💎 GÉOR — Check-in de Produtos</div>
    <div class="h-sub">Registre variações de cores com estoque e gôndola</div>
  </header>

  <div class="tabs">
    <button class="tab-btn active" onclick="abrirAba('checkin')">📦 Check-in</button>
    <button class="tab-btn" onclick="abrirAba('produtos')">🗂️ Produtos</button>
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
          <div class="foto-text">Toque para tirar foto ou selecionar</div>
          <img id="preview-img" alt=""/>
        </div>
      </div>

      <div class="form-group">
        <label>Nome / Descrição *</label>
        <input type="text" id="f-nome" placeholder="Ex: Anel Solitário"/>
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
        <label>Variações de Cores com Estoque *</label>
        <div class="cores-container" id="cores-list"></div>
        <div class="cor-input">
          <input type="text" id="cor-input" placeholder="Ex: Ouro"/>
          <button type="button" onclick="window.adicionarCor()">+ Adicionar</button>
        </div>
      </div>

      <div class="form-group">
        <label>Observações</label>
        <textarea id="f-obs" placeholder="Tamanho, coleção, material..." style="min-height:80px;"></textarea>
      </div>

      <button class="btn-primary" type="button" onclick="window.registrarProduto()">✅ Registrar Check-in</button>
    </div>
  </div>

  <!-- ABA PRODUTOS -->
  <div id="produtos" class="tab-content">
    <div class="card">
      <h2>🗂️ Produtos Registrados</h2>
      <div class="stats-grid" id="stats-produtos"></div>
      <div class="produtos-grid" id="produtos-grid"></div>
      <div id="produtos-empty" class="empty" style="display:none;">
        <div class="empty-icon">📦</div>
        <p>Nenhum produto registrado</p>
      </div>
    </div>
  </div>
</div>

<div id="toast" class="toast"></div>

<script src="https://www.gstatic.com/firebasejs/10.7.0/firebase-app.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.7.0/firebase-database.js"></script>

<script>
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
const database = firebase.database();

let coresTemp = [];
let fotoB64 = null;

function toast(msg) {
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  setTimeout(() => t.classList.remove('show'), 3000);
}

function abrirAba(aba) {
  document.querySelectorAll('.tab-content').forEach(el => el.classList.remove('active'));
  document.querySelectorAll('.tab-btn').forEach(el => el.classList.remove('active'));
  document.getElementById(aba).classList.add('active');
  event.target.classList.add('active');
  if (aba === 'produtos') carregarProdutos();
}

document.getElementById('foto-input').addEventListener('change', function(e) {
  const file = e.target.files[0];
  if (!file) return;
  const reader = new FileReader();
  reader.onload = function(event) {
    fotoB64 = event.target.result;
    document.getElementById('preview-img').src = fotoB64;
    document.getElementById('preview-img').style.display = 'block';
    toast('✅ Foto adicionada!');
  };
  reader.readAsDataURL(file);
});

window.adicionarCor = function() {
  const cor = document.getElementById('cor-input').value.trim();
  if (!cor) {
    toast('⚠️ Digite uma cor');
    return;
  }
  if (coresTemp.find(c => c.nome === cor)) {
    toast('⚠️ Cor já existe');
    return;
  }
  coresTemp.push({ nome: cor, gondola: 0, estoque: 0 });
  renderizarCores();
  document.getElementById('cor-input').value = '';
};

window.removerCor = function(idx) {
  coresTemp.splice(idx, 1);
  renderizarCores();
};

window.atualizarCor = function(idx, campo, valor) {
  coresTemp[idx][campo] = parseInt(valor) || 0;
};

function renderizarCores() {
  const container = document.getElementById('cores-list');
  container.innerHTML = coresTemp.map((cor, i) => `
    <div class="cor-item">
      <div class="cor-item-header">
        <div class="cor-item-nome">${cor.nome}</div>
        <button type="button" class="cor-item-btn" onclick="window.removerCor(${i})">✕</button>
      </div>
      <div class="cor-qtd-grid">
        <div>
          <label>Gôndola</label>
          <input type="number" min="0" value="${cor.gondola}" onchange="window.atualizarCor(${i}, 'gondola', this.value)"/>
        </div>
        <div>
          <label>Estoque</label>
          <input type="number" min="0" value="${cor.estoque}" onchange="window.atualizarCor(${i}, 'estoque', this.value)"/>
        </div>
      </div>
    </div>
  `).join('');
}

window.registrarProduto = function() {
  const nome = document.getElementById('f-nome').value.trim();
  const ref = document.getElementById('f-ref').value.trim();
  const tipo = document.getElementById('f-tipo').value;

  if (!nome) { toast('⚠️ Informe o nome'); return; }
  if (!ref) { toast('⚠️ Informe o código'); return; }
  if (!tipo) { toast('⚠️ Selecione o tipo'); return; }
  if (coresTemp.length === 0) { toast('⚠️ Adicione uma cor'); return; }

  const produto = {
    data: new Date().toISOString(),
    nome: nome,
    ref: ref,
    tipo: tipo,
    fornecedor: document.getElementById('f-forn').value.trim(),
    custo: parseFloat(document.getElementById('f-custo').value) || 0,
    preco: parseFloat(document.getElementById('f-preco').value) || 0,
    obs: document.getElementById('f-obs').value.trim(),
    cores: JSON.parse(JSON.stringify(coresTemp)),
    foto: fotoB64
  };

  database.ref('produtos').push(produto).then(function() {
    document.getElementById('f-nome').value = '';
    document.getElementById('f-ref').value = '';
    document.getElementById('f-tipo').value = '';
    document.getElementById('f-forn').value = '';
    document.getElementById('f-custo').value = '';
    document.getElementById('f-preco').value = '';
    document.getElementById('f-obs').value = '';
    document.getElementById('preview-img').style.display = 'none';
    document.getElementById('foto-input').value = '';
    coresTemp = [];
    renderizarCores();
    fotoB64 = null;
    toast('✅ Produto registrado!');
  }).catch(function(error) {
    toast('❌ Erro: ' + error.message);
  });
};

function carregarProdutos() {
  database.ref('produtos').once('value', function(snapshot) {
    const dados = snapshot.val();
    const lista = dados ? Object.entries(dados).map(([key, val]) => ({id: key, ...val})) : [];

    const stats = document.getElementById('stats-produtos');
    const grid = document.getElementById('produtos-grid');
    const empty = document.getElementById('produtos-empty');

    if (lista.length === 0) {
      empty.style.display = 'block';
      grid.innerHTML = '';
      stats.innerHTML = '';
      return;
    }

    empty.style.display = 'none';
    const total = lista.length;
    const totalItens = lista.reduce((a, p) => a + (p.cores || []).reduce((b, c) => b + (c.gondola || 0) + (c.estoque || 0), 0), 0);
    const totalValor = lista.reduce((a, p) => a + ((p.preco || 0) * ((p.cores || []).reduce((b, c) => b + (c.gondola || 0) + (c.estoque || 0), 0))), 0);

    stats.innerHTML = `
      <div class="stat-box"><div class="num">${total}</div><div class="lbl">Produtos</div></div>
      <div class="stat-box"><div class="num">${totalItens}</div><div class="lbl">Itens</div></div>
      <div class="stat-box"><div class="num">R$ ${totalValor.toFixed(2).replace('.', ',')}</div><div class="lbl">Valor</div></div>`;

    grid.innerHTML = lista.map(p => `
      <div class="produto-card">
        ${p.foto ? `<img src="${p.foto}" alt="${p.nome}"/>` : `<div class="no-img">💍</div>`}
        <h3>${p.nome}</h3>
        <div class="ref">${p.ref}</div>
        <div class="tipo">${p.tipo}</div>
        <div class="preco">R$ ${(p.preco || 0).toFixed(2).replace('.', ',')}</div>
        <div style="margin-top:12px;border-top:1px solid #f0e0e5;padding-top:12px;">
          ${(p.cores || []).map(c => `<div class="cor-info"><strong>${c.nome}</strong> | 🛒 ${c.gondola || 0} | 📦 ${c.estoque || 0}</div>`).join('')}
        </div>
        <button class="btn-delete" style="margin-top:8px;" onclick="window.deletarProduto('${p.id}')">🗑️ Deletar</button>
      </div>
    `).join('');
  });
}

window.deletarProduto = function(id) {
  if (!confirm('Deletar este produto?')) return;
  database.ref('produtos/' + id).remove().then(function() {
    toast('✅ Deletado!');
    carregarProdutos();
  }).catch(function(error) {
    toast('❌ Erro: ' + error.message);
  });
};
</script>

</body>
</html>
