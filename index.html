<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GÉOR - Check-in de Produtos</title>
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
            max-width: 1200px;
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

        .tabs {
            display: flex;
            border-bottom: 2px solid #eee;
            background: #f9f9f9;
        }

        .tab-button {
            flex: 1;
            padding: 15px;
            border: none;
            background: none;
            cursor: pointer;
            font-size: 16px;
            font-weight: 500;
            color: #666;
            transition: all 0.3s ease;
            border-bottom: 3px solid transparent;
        }

        .tab-button.active {
            color: #a8597e;
            border-bottom-color: #a8597e;
        }

        .tab-button:hover {
            background: #f0f0f0;
        }

        .tab-content {
            display: none;
            padding: 30px;
            animation: fadeIn 0.3s ease;
        }

        .tab-content.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
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
            font-family: inherit;
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

        .form-row.three {
            grid-template-columns: 1fr 1fr 1fr;
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

        .button:active {
            transform: translateY(0);
        }

        .button.secondary {
            background: #f0f0f0;
            color: #333;
        }

        .button.secondary:hover {
            background: #e0e0e0;
        }

        .button.danger {
            background: #e74c3c;
        }

        .button.danger:hover {
            background: #c0392b;
        }

        .button.add {
            background: #a8597e;
            width: 100%;
            margin-top: 10px;
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
            border-left: 4px solid #a8597e;
            display: grid;
            grid-template-columns: 1fr 1fr 1fr auto;
            gap: 10px;
            align-items: flex-end;
        }

        .variation-item input {
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 14px;
        }

        .products-list {
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
            transition: transform 0.2s ease;
        }

        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.15);
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
            line-height: 1.5;
        }

        .product-card .label {
            font-weight: 600;
            color: #333;
        }

        .color-badge {
            display: inline-block;
            padding: 6px 12px;
            background: #f0f0f0;
            border-radius: 3px;
            font-size: 12px;
            margin-right: 5px;
            margin-bottom: 5px;
            border-left: 3px solid #a8597e;
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
            margin-bottom: 5px;
        }

        .history-item .details {
            color: #666;
            font-size: 13px;
        }

        .empty-state {
            text-align: center;
            padding: 40px;
            color: #999;
        }

        .alert {
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 20px;
            font-weight: 500;
        }

        .alert.success {
            background: #d4edda;
            color: #155724;
            border: 1px solid #c3e6cb;
        }

        .alert.error {
            background: #f8d7da;
            color: #721c24;
            border: 1px solid #f5c6cb;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .stat-card {
            background: linear-gradient(135deg, #a8597e 0%, #6b3d5c 100%);
            color: white;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
        }

        .stat-card .number {
            font-size: 32px;
            font-weight: bold;
            margin-bottom: 5px;
        }

        .stat-card .label {
            font-size: 14px;
            opacity: 0.9;
        }

        .checkin-form {
            background: #f9f9f9;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 20px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        table th, table td {
            padding: 12px;
            text-align: left;
            border: 1px solid #ddd;
        }

        table th {
            background: #f0f0f0;
            font-weight: 600;
            color: #333;
        }

        table tr:hover {
            background: #f9f9f9;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>💎 GÉOR – Check-in de Produtos</h1>
            <p>Cadastre variações de cores com estoque e gôndola</p>
        </div>

        <div class="tabs">
            <button class="tab-button active" onclick="switchTab('checkin')">✅ Check-in</button>
            <button class="tab-button" onclick="switchTab('produtos')">📦 Produtos</button>
            <button class="tab-button" onclick="switchTab('relatorio')">📊 Relatório</button>
            <button class="tab-button" onclick="switchTab('historico')">📜 Histórico</button>
        </div>

        <!-- ABA CHECK-IN -->
        <div id="checkin" class="tab-content active">
            <h2>✏️ Novo Registro de Produto</h2>
            <div id="checkinAlert"></div>

            <div class="checkin-form">
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
                            <option value="Bolo">Bolo</option>
                            <option value="Doce">Doce</option>
                            <option value="Salgado">Salgado</option>
                            <option value="Bebida">Bebida</option>
                            <option value="Acessório">Acessório</option>
                            <option value="Outro">Outro</option>
                        </select>
                    </div>
                </div>

                <div class="form-group">
                    <label>NÃO SE TRATA DE</label>
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
                    <textarea id="produtoObservacoes" placeholder="Tamanho, coleção, material..." rows="4"></textarea>
                </div>

                <button class="button" onclick="salvarProduto()" style="width: 100%; margin-top: 20px;">✅ Check-in do Registrador</button>
            </div>
        </div>

        <!-- ABA PRODUTOS -->
        <div id="produtos" class="tab-content">
            <h2>📦 Produtos Cadastrados</h2>
            <div id="produtosList" class="products-list"></div>
        </div>

        <!-- ABA RELATÓRIO -->
        <div id="relatorio" class="tab-content">
            <h2>📊 Relatório de Estoque</h2>
            <div id="stats" class="stats"></div>
            <div id="relatorioContent"></div>
        </div>

        <!-- ABA HISTÓRICO -->
        <div id="historico" class="tab-content">
            <h2>📜 Histórico de Movimentos</h2>
            <div id="historicoList"></div>
        </div>
    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/10.7.0/firebase-app.js";
        import { getDatabase, ref, push, set, get, onValue } from "https://www.gstatic.com/firebasejs/10.7.0/firebase-database.js";

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

        // Carregar dados do Firebase
        function carregarDados() {
            const produtosRef = ref(database, 'produtos');
            onValue(produtosRef, (snapshot) => {
                if (snapshot.exists()) {
                    produtos = snapshot.val();
                } else {
                    produtos = {};
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

        window.switchTab = function(tab) {
            document.querySelectorAll('.tab-content').forEach(el => el.classList.remove('active'));
            document.querySelectorAll('.tab-button').forEach(el => el.classList.remove('active'));
            document.getElementById(tab).classList.add('active');
            event.target.classList.add('active');

            if (tab === 'relatorio') {
                atualizarRelatorio();
            }
        };

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
            const alert = document.getElementById('checkinAlert');

            if (!nome || !codigo || !tipo || variacoesCadastro.length === 0) {
                alert.innerHTML = '<div class="alert error">Por favor, preencha os campos obrigatórios e adicione pelo menos uma variação de cor.</div>';
                return;
            }

            const produtoId = Date.now().toString();
            const produtoData = {
                id: produtoId,
                nome: nome,
                codigo: codigo,
                tipo: tipo,
                fornecedor: fornecedor,
                custo: custo,
                venda: venda,
                observacoes: observacoes,
                dataCadastro: new Date().toISOString(),
                variacoes: {}
            };

            variacoesCadastro.forEach((v) => {
                if (v.cor) {
                    produtoData.variacoes[v.cor] = {
                        cor: v.cor,
                        estoque: v.estoque,
                        gondola: v.gondola
                    };
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
            }).catch((error) => {
                alert.innerHTML = `<div class="alert error">❌ Erro ao salvar: ${error.message}</div>`;
            });
        };

        function atualizarInterface() {
            const produtosList = document.getElementById('produtosList');
            produtosList.innerHTML = '';

            if (Object.keys(produtos).length === 0) {
                produtosList.innerHTML = '<div class="empty-state"><p>Nenhum produto cadastrado ainda.</p></div>';
            } else {
                Object.values(produtos).forEach(produto => {
                    const card = document.createElement('div');
                    card.className = 'product-card';
                    let coresHtml = '';
                    let totalEstoque = 0;
                    let totalGondola = 0;

                    Object.values(produto.variacoes).forEach(variacao => {
                        coresHtml += `<div class="color-badge">${variacao.cor}: E${variacao.estoque} | G${variacao.gondola}</div>`;
                        totalEstoque += variacao.estoque;
                        totalGondola += variacao.gondola;
                    });

                    card.innerHTML = `
                        <h3>${produto.nome}</h3>
                        <p><span class="label">Código:</span> ${produto.codigo}</p>
                        <p><span class="label">Tipo:</span> ${produto.tipo}</p>
                        ${produto.fornecedor ? `<p><span class="label">Fornecedor:</span> ${produto.fornecedor}</p>` : ''}
                        <p><span class="label">Preço:</span> R$ ${produto.custo.toFixed(2)} (custo) | R$ ${produto.venda.toFixed(2)} (venda)</p>
                        ${produto.observacoes ? `<p><span class="label">Observações:</span> ${produto.observacoes}</p>` : ''}
                        <p><span class="label">Estoque Total:</span> ${totalEstoque} | <span class="label">Gôndola Total:</span> ${totalGondola}</p>
                        <p><span class="label">Cores:</span></p>
                        <div>${coresHtml}</div>
                        <button class="button danger" onclick="deletarProduto('${produto.id}')" style="margin-top: 10px; width: 100%;">🗑️ Deletar</button>
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
                historicoList.innerHTML = '<div class="empty-state"><p>Nenhum movimento registrado ainda.</p></div>';
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

        function atualizarRelatorio() {
            const statsDiv = document.getElementById('stats');
            const relatorioContent = document.getElementById('relatorioContent');

            let totalProdutos = Object.keys(produtos).length;
            let totalEstoque = 0;
            let totalGondola = 0;
            let totalMovimentos = historico.length;

            Object.values(produtos).forEach(produto => {
                Object.values(produto.variacoes).forEach(variacao => {
                    totalEstoque += variacao.estoque;
                    totalGondola += variacao.gondola;
                });
            });

            statsDiv.innerHTML = `
                <div class="stat-card">
                    <div class="number">${totalProdutos}</div>
                    <div class="label">Produtos Cadastrados</div>
                </div>
                <div class="stat-card">
                    <div class="number">${totalEstoque}</div>
                    <div class="label">Total em Estoque</div>
                </div>
                <div class="stat-card">
                    <div class="number">${totalGondola}</div>
                    <div class="label">Total em Gôndola</div>
                </div>
                <div class="stat-card">
                    <div class="number">${totalMovimentos}</div>
                    <div class="label">Movimentos Registrados</div>
                </div>
            `;

            relatorioContent.innerHTML = '';
            if (Object.keys(produtos).length === 0) {
                relatorioContent.innerHTML = '<div class="empty-state"><p>Nenhum produto para exibir.</p></div>';
            } else {
                Object.values(produtos).forEach(produto => {
                    const div = document.createElement('div');
                    div.style.marginBottom = '20px';
                    let html = `<h3>${produto.nome}</h3><table>
                        <tr>
                            <th>Cor</th>
                            <th>Estoque</th>
                            <th>Gôndola</th>
                            <th>Total</th>
                        </tr>`;

                    Object.values(produto.variacoes).forEach(variacao => {
                        html += `<tr>
                            <td>${variacao.cor}</td>
                            <td>${variacao.estoque}</td>
                            <td>${variacao.gondola}</td>
                            <td>${variacao.estoque + variacao.gondola}</td>
                        </tr>`;
                    });

                    html += '</table>';
                    div.innerHTML = html;
                    relatorioContent.appendChild(div);
                });
            }
        }

        // Inicializar
        carregarDados();
    </script>
</body>
</html>
