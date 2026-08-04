<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GÉOR – Check-in de Produtos</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #a8597e 0%, #6b3d5c 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            background: white;
            border-radius: 15px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
            overflow: hidden;
        }

        .header {
            background: linear-gradient(135deg, #a8597e 0%, #6b3d5c 100%);
            color: white;
            padding: 30px;
            text-align: center;
        }

        .header h1 {
            font-size: 28px;
            margin-bottom: 5px;
        }

        .header p {
            font-size: 14px;
            opacity: 0.9;
        }

        .content {
            padding: 30px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: #a8597e;
            font-size: 14px;
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 14px;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #a8597e;
            box-shadow: 0 0 0 3px rgba(168, 89, 126, 0.1);
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .button {
            background: linear-gradient(135deg, #a8597e 0%, #6b3d5c 100%);
            color: white;
            padding: 12px 30px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            font-weight: 600;
            transition: transform 0.2s ease;
        }

        .button:hover {
            transform: translateY(-2px);
        }

        .button.danger {
            background: #e74c3c;
        }

        .button.danger:hover {
            background: #c0392b;
        }

        .button.add {
            width: 100%;
            margin-top: 10px;
        }

        .button.reposicao {
            background: #27ae60;
            padding: 8px 16px;
            font-size: 14px;
        }

        .button.reposicao:hover {
            background: #229954;
        }

        .variations-container {
            background: #f9f9f9;
            padding: 20px;
            border-radius: 5px;
            margin-top: 20px;
            border-left: 4px solid #a8597e;
        }

        .variation-item {
            background: white;
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 15px;
            display: grid;
            grid-template-columns: 1fr 1fr 1fr auto;
            gap: 10px;
            align-items: flex-end;
        }

        .variation-item input {
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        .alert {
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 20px;
        }

        .alert.success {
            background: #d4edda;
            color: #155724;
        }

        .alert.error {
            background: #f8d7da;
            color: #721c24;
        }

        .section-divider {
            margin: 40px 0;
            padding: 20px 0;
            border-top: 2px solid #eee;
        }

        .section-divider h2 {
            color: #a8597e;
            margin-bottom: 20px;
        }

        .search-box {
            margin-bottom: 20px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .search-box input,
        .search-box select {
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 14px;
        }

        .products-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .product-card {
            background: white;
            border: 1px solid #eee;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        }

        .product-card h3 {
            color: #a8597e;
            margin-bottom: 10px;
            font-size: 18px;
        }

        .product-card p {
            color: #666;
            font-size: 13px;
            margin-bottom: 8px;
        }

        .product-card .label {
            font-weight: 600;
            color: #333;
        }

        .color-info {
            background: #f9f9f9;
            padding: 10px;
            border-radius: 5px;
            margin: 10px 0;
            font-size: 13px;
        }

        .color-info strong {
            color: #a8597e;
        }

        .empty-state {
            text-align: center;
            padding: 40px;
            color: #999;
        }

        .history-item {
            background: #f9f9f9;
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 15px;
            border-left: 4px solid #a8597e;
        }

        .history-item .timestamp {
            color: #999;
            font-size: 12px;
            margin-bottom: 5px;
        }

        .history-item .action {
            color: #333;
            font-weight: 600;
        }

        .history-item .details {
            color: #666;
            font-size: 13px;
            margin-top: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>💎 GÉOR – Check-in de Produtos</h1>
            <p>Controle de Estoque e Gôndola - Bolo Mania</p>
        </div>

        <div class="content">
            <!-- CADASTRO DE PRODUTOS -->
            <h2>✏️ Cadastro de Produto</h2>
            <div id="cadastroAlert"></div>

            <div style="background: #f9f9f9; padding: 20px; border-radius: 8px; margin-bottom: 30px;">
                <div class="form-group">
                    <label>NOME / DESCRIÇÃO *</label>
                    <input type="text" id="produtoNome" placeholder="Ex: Anel Solitário">
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label>CÓDIGO / PROPRIETÁRIO *</label>
                        <input type="text" id="produtoCodigo" placeholder="Ex: GR-001">
                    </div>
                    <div class="form-group">
                        <label>TIPO *</label>
                        <select id="produtoTipo">
                            <option value="">Selecione...</option>
                            <option value="Prata 925">Prata 925</option>
                            <option value="Semijoia">Semijoia</option>
                            <option value="Bijouteria">Bijouteria</option>
                            <option value="Óculos">Óculos</option>
                            <option value="Relógio">Relógio</option>
                            <option value="Aço Inoxidável">Aço Inoxidável</option>
                            <option value="Folheado">Folheado</option>
                            <option value="Bolsa">Bolsa</option>
                        </select>
                    </div>
                </div>

                <div class="form-group">
                    <label>FORNECEDOR</label>
                    <input type="text" id="produtoFornecedor" placeholder="Nome do fornecedor">
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label>PREÇO DE CUSTO (R$)</label>
                        <input type="number" id="produtoCusto" placeholder="0,00" step="0.01" min="0">
                    </div>
                    <div class="form-group">
                        <label>PREÇO DE VENDA (R$)</label>
                        <input type="number" id="produtoVenda" placeholder="0,00" step="0.01" min="0">
                    </div>
                </div>

                <div class="variations-container">
                    <h3>VARIAÇÕES DE CORES COM ESTOQUE *</h3>
                    <div id="variacoesList"></div>
                    <button class="button add" onclick="adicionarVariacao()">+ Adicionar Cor</button>
                </div>

                <div class="form-group">
                    <label>OBSERVAÇÕES</label>
                    <textarea id="produtoObservacoes" placeholder="Tamanho, coleção, material..." rows="3"></textarea>
                </div>

                <button class="button" onclick="salvarProduto()" style="width: 100%; margin-top: 20px;">✅ Salvar Produto</button>
            </div>

            <!-- FILTRO E LISTAGEM -->
            <div class="section-divider">
                <h2>📦 Produtos Cadastrados</h2>
                <div class="search-box">
                    <input type="text" id="searchNome" placeholder="🔍 Buscar por nome..." onkeyup="filtrarProdutos()">
                    <select id="filterTipo" onchange="filtrarProdutos()">
                        <option value="">Filtrar por tipo...</option>
                        <option value="Prata 925">Prata 925</option>
                        <option value="Semijoia">Semijoia</option>
                        <option value="Bijouteria">Bijouteria</option>
                        <option value="Óculos">Óculos</option>
                        <option value="Relógio">Relógio</option>
                        <option value="Aço Inoxidável">Aço Inoxidável</option>
                        <option value="Folheado">Folheado</option>
                        <option value="Bolsa">Bolsa</option>
                    </select>
                </div>
                <div id="produtosList" class="products-container"></div>
            </div>

            <!-- HISTÓRICO -->
            <div class="section-divider">
                <h2>📜 Histórico de Movimentos</h2>
                <div id="historicoList"></div>
            </div>
        </div>
    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/10.7.0/firebase-app.js";
        import { getDatabase, ref, push, set, onValue } from "https://www.gstatic.com/firebasejs/10.7.0/firebase-database.js";

        const firebaseConfig = {
            apiKey: "AIzaSyDnMsL-dhv3uM2tP3B-IcJUFHVo1MmoW2k",
            authDomain: "checkin-4760f.firebaseapp.com",
            databaseURL: "https://checkin-4760f-default-rtdb.firebaseio.com",
            projectId: "checkin-4760f",
            storageBucket: "checkin-4760f.firebasestorage.app",
            messagingSenderId: "207981324873",
            appId: "1:207981324873:web:41709da7ffc12cc4966d98",
            measurementId: "G-T2K2EPDTVN"
        };

        const app = initializeApp(firebaseConfig);
        const database = getDatabase(app);

        let produtos = {};
        let historico = [];
        let variacoesCadastro = [];
        let produtosFiltrados = {};

        function carregarDados() {
            const produtosRef = ref(database, 'produtos');
            onValue(produtosRef, (snapshot) => {
                if (snapshot.exists()) {
                    produtos = snapshot.val();
                    produtosFiltrados = JSON.parse(JSON.stringify(produtos));
                } else {
                    produtos = {};
                    produtosFiltrados = {};
                }
                atualizarInterface();
            });

            const historicoRef = ref(database, 'historico');
            onValue(historicoRef, (snapshot) => {
                if (snapshot.exists()) {
                    historico = Object.values(snapshot.val());
                    historico.sort((a, b) => new Date(b.data) - new Date(a.data));
                } else {
                    historico = [];
                }
                atualizarHistorico();
            });
        }

        window.adicionarVariacao = function() {
            variacoesCadastro.push({ cor: '', estoque: 0, gondola: 0 });
            renderizarVariacoes();
        };

        function renderizarVariacoes() {
            const container = document.getElementById('variacoesList');
            container.innerHTML = '';
            variacoesCadastro.forEach((v, index) => {
                const div = document.createElement('div');
                div.className = 'variation-item';
                div.innerHTML = `
                    <input type="text" placeholder="Cor" value="${v.cor}" onchange="variacoesCadastro[${index}].cor = this.value">
                    <input type="number" placeholder="Estoque" value="${v.estoque}" min="0" onchange="variacoesCadastro[${index}].estoque = parseInt(this.value) || 0">
                    <input type="number" placeholder="Gôndola" value="${v.gondola}" min="0" onchange="variacoesCadastro[${index}].gondola = parseInt(this.value) || 0">
                    <button class="button danger" onclick="variacoesCadastro.splice(${index}, 1); renderizarVariacoes();">✕</button>
                `;
                container.appendChild(div);
            });
        }

        window.salvarProduto = function() {
            const nome = document.getElementById('produtoNome').value.trim();
            const codigo = document.getElementById('produtoCodigo').value.trim();
            const tipo = document.getElementById('produtoTipo').value;
            const fornecedor = document.getElementById('produtoFornecedor').value.trim();
            const custo = parseFloat(document.getElementById('produtoCusto').value) || 0;
            const venda = parseFloat(document.getElementById('produtoVenda').value) || 0;
            const observacoes = document.getElementById('produtoObservacoes').value.trim();
            const alert = document.getElementById('cadastroAlert');

            if (!nome || !codigo || !tipo || variacoesCadastro.length === 0) {
                alert.innerHTML = '<div class="alert error">Por favor, preencha os campos obrigatórios!</div>';
                return;
            }

            const produtoId = Date.now().toString();
            const produtoData = {
                id: produtoId,
                nome, codigo, tipo, fornecedor, custo, venda, observacoes,
                dataCadastro: new Date().toISOString(),
                variacoes: {}
            };

            variacoesCadastro.forEach(v => {
                if (v.cor) {
                    produtoData.variacoes[v.cor] = { cor: v.cor, estoque: v.estoque, gondola: v.gondola };
                }
            });

            set(ref(database, `produtos/${produtoId}`), produtoData).then(() => {
                alert.innerHTML = '<div class="alert success">✅ Produto salvo com sucesso!</div>';
                document.getElementById('produtoNome').value = '';
                document.getElementById('produtoCodigo').value = '';
                document.getElementById('produtoTipo').value = '';
                document.getElementById('produtoFornecedor').value = '';
                document.getElementById('produtoCusto').value = '';
                document.getElementById('produtoVenda').value = '';
                document.getElementById('produtoObservacoes').value = '';
                variacoesCadastro = [];
                renderizarVariacoes();
                setTimeout(() => { alert.innerHTML = ''; }, 3000);
            }).catch(error => {
                alert.innerHTML = `<div class="alert error">❌ Erro: ${error.message}</div>`;
            });
        };

        window.filtrarProdutos = function() {
            const nome = document.getElementById('searchNome').value.toLowerCase();
            const tipo = document.getElementById('filterTipo').value;
            produtosFiltrados = {};

            Object.values(produtos).forEach(produto => {
                const matchNome = produto.nome.toLowerCase().includes(nome);
                const matchTipo = !tipo || produto.tipo === tipo;
                if (matchNome && matchTipo) {
                    produtosFiltrados[produto.id] = produto;
                }
            });
            atualizarInterface();
        };

        window.reporEstoque = function(produtoId, cor) {
            const produto = produtos[produtoId];
            const variacao = produto.variacoes[cor];

            const quantidade = prompt(`Quantas unidades entram em gôndola?\nEstoque atual: ${variacao.estoque}\nGôndola atual: ${variacao.gondola}`);

            if (quantidade === null || quantidade === '') return;

            const qtd = parseInt(quantidade);
            if (isNaN(qtd) || qtd <= 0) {
                alert('Quantidade inválida!');
                return;
            }

            if (qtd > variacao.estoque) {
                alert('Quantidade maior que o estoque!');
                return;
            }

            const novoEstoque = variacao.estoque - qtd;
            const novaGondola = variacao.gondola + qtd;

            set(ref(database, `produtos/${produtoId}/variacoes/${cor}`), {
                cor, estoque: novoEstoque, gondola: novaGondola
            }).then(() => {
                const historicoEntry = {
                    id: Date.now().toString(),
                    data: new Date().toISOString(),
                    produto: produto.nome,
                    cor,
                    quantidade: qtd,
                    estoqueAnterior: variacao.estoque,
                    estoqueNovo: novoEstoque,
                    gondolaAnterior: variacao.gondola,
                    gondolaNova: novaGondola
                };
                push(ref(database, 'historico'), historicoEntry);
            });
        };

        function atualizarInterface() {
            const produtosList = document.getElementById('produtosList');
            produtosList.innerHTML = '';

            if (Object.keys(produtosFiltrados).length === 0) {
                produtosList.innerHTML = '<div class="empty-state" style="grid-column: 1/-1;">Nenhum produto encontrado.</div>';
            } else {
                Object.values(produtosFiltrados).forEach(produto => {
                    let totalEstoque = 0, totalGondola = 0;
                    let coresHtml = '';

                    Object.values(produto.variacoes).forEach(variacao => {
                        totalEstoque += variacao.estoque;
                        totalGondola += variacao.gondola;
                        coresHtml += `
                            <div class="color-info">
                                <strong>${variacao.cor}</strong><br>
                                Estoque: ${variacao.estoque} | Gôndola: ${variacao.gondola}
                                <button class="button reposicao" onclick="reporEstoque('${produto.id}', '${variacao.cor}')" style="margin-top: 8px; width: 100%;">🔄 Repor</button>
                            </div>
                        `;
                    });

                    const card = document.createElement('div');
                    card.className = 'product-card';
                    card.innerHTML = `
                        <h3>${produto.nome}</h3>
                        <p><span class="label">Código:</span> ${produto.codigo}</p>
                        <p><span class="label">Tipo:</span> ${produto.tipo}</p>
                        ${produto.fornecedor ? `<p><span class="label">Fornecedor:</span> ${produto.fornecedor}</p>` : ''}
                        <p><span class="label">Preço:</span> R$ ${produto.custo.toFixed(2)} (custo) | R$ ${produto.venda.toFixed(2)} (venda)</p>
                        <p><span class="label">Total Estoque:</span> ${totalEstoque} | <span class="label">Total Gôndola:</span> ${totalGondola}</p>
                        ${produto.observacoes ? `<p><span class="label">Observações:</span> ${produto.observacoes}</p>` : ''}
                        <div style="margin-top: 15px; border-top: 1px solid #eee; padding-top: 15px;">
                            <strong style="color: #a8597e;">Cores:</strong>
                            ${coresHtml}
                        </div>
                        <button class="button danger" onclick="deletarProduto('${produto.id}')" style="width: 100%; margin-top: 15px;">🗑️ Deletar</button>
                    `;
                    produtosList.appendChild(card);
                });
            }
        }

        window.deletarProduto = function(produtoId) {
            if (confirm('Tem certeza que deseja deletar este produto?')) {
                set(ref(database, `produtos/${produtoId}`), null);
            }
        };

        function atualizarHistorico() {
            const historicoList = document.getElementById('historicoList');
            historicoList.innerHTML = '';

            if (historico.length === 0) {
                historicoList.innerHTML = '<div class="empty-state">Nenhum movimento registrado.</div>';
            } else {
                historico.forEach(item => {
                    const data = new Date(item.data);
                    const div = document.createElement('div');
                    div.className = 'history-item';
                    div.innerHTML = `
                        <div class="timestamp">${data.toLocaleString('pt-BR')}</div>
                        <div class="action">${item.produto} - ${item.cor}</div>
                        <div class="details">
                            Quantidade movida: ${item.quantidade} unidades<br>
                            Estoque: ${item.estoqueAnterior} → ${item.estoqueNovo}<br>
                            Gôndola: ${item.gondolaAnterior} → ${item.gondolaNova}
                        </div>
                    `;
                    historicoList.appendChild(div);
                });
            }
        }

        carregarDados();
    </script>
</body>
</html>
