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

        .content {
            padding: 30px;
        }

        .section {
            margin-bottom: 40px;
        }

        .section h2 {
            color: #a8597e;
            margin-bottom: 20px;
            font-size: 22px;
            border-bottom: 2px solid #a8597e;
            padding-bottom: 10px;
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
            font-size: 14px;
        }

        .filters {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-bottom: 20px;
        }

        .product-item {
            background: #f9f9f9;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 15px;
            border-left: 4px solid #a8597e;
        }

        .product-item h3 {
            color: #a8597e;
            margin-bottom: 10px;
        }

        .product-item p {
            color: #666;
            font-size: 13px;
            margin-bottom: 8px;
        }

        .product-item .label {
            font-weight: 600;
            color: #333;
        }

        .color-badge {
            display: inline-block;
            padding: 6px 12px;
            background: white;
            border-radius: 3px;
            font-size: 12px;
            margin-right: 5px;
            margin-bottom: 5px;
            border-left: 3px solid #a8597e;
        }

        .product-actions {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }

        .product-actions button {
            flex: 1;
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

        .empty-state {
            text-align: center;
            padding: 40px;
            color: #999;
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

        .reposicao-form {
            background: #fff3cd;
            padding: 20px;
            border-radius: 8px;
            border-left: 4px solid #ffc107;
            margin-top: 15px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>💎 GÉOR – Check-in de Produtos</h1>
            <p>Controle de Estoque e Gôndola</p>
        </div>

        <div class="content">
            <!-- SEÇÃO CADASTRO -->
            <div class="section">
                <h2>✏️ Cadastro de Produto</h2>
                <div id="checkinAlert"></div>

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

                <button class="button" onclick="salvarProduto()" style="width: 100%; margin-top: 20px;">✅ Salvar Produto</button>
            </div>

            <!-- SEÇÃO PRODUTOS -->
            <div class="section">
                <h2>📦 Produtos Cadastrados</h2>

                <div class="filters">
                    <div class="form-group">
                        <label>🔍 Buscar por nome...</label>
                        <input type="text" id="searchNome" placeholder="Digite o nome do produto" onkeyup="filtrarProdutos()">
                    </div>
                    <div class="form-group">
                        <label>🏷️ Filtrar por tipo...</label>
                        <select id="filterTipo" onchange="filtrarProdutos()">
                            <option value="">Todos os tipos</option>
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

                <div id="produtosList"></div>
            </div>

            <!-- SEÇÃO HISTÓRICO -->
            <div class="section">
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

        function carregarDados() {
            const produtosRef = ref(database, 'produtos');
            onValue(produtosRef, (snapshot) => {
                if (snapshot.exists()) {
                    produtos = snapshot.val();
                } else {
                    produtos = {};
                }
                filtrarProdutos();
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
            const alert = document.getElementById('checkinAlert');

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
            const produtosList = document.getElementById('produtosList');

            produtosList.innerHTML = '';

            let produtosEncontrados = Object.values(produtos).filter(produto => {
                const nomeMatch = produto.nome.toLowerCase().includes(nome) || produto.codigo.toLowerCase().includes(nome);
                const tipoMatch = !tipo || produto.tipo === tipo;
                return nomeMatch && tipoMatch;
            });

            if (produtosEncontrados.length === 0) {
                produtosList.innerHTML = '<div class="empty-state">Nenhum produto encontrado.</div>';
                return;
            }

            produtosEncontrados.forEach(produto => {
                let totalEstoque = 0, totalGondola = 0, cores = '';
                Object.values(produto.variacoes).forEach(variacao => {
                    cores += `<div class="color-badge">${variacao.cor} (E: ${variacao.estoque} | G: ${variacao.gondola})</div>`;
                    totalEstoque += variacao.estoque;
                    totalGondola += variacao.gondola;
                });

                const div = document.createElement('div');
                div.className = 'product-item';
                div.innerHTML = `
                    <h3>${produto.nome}</h3>
                    <p><span class="label">Código:</span> ${produto.codigo}</p>
                    <p><span class="label">Tipo:</span> ${produto.tipo}</p>
                    ${produto.fornecedor ? `<p><span class="label">Fornecedor:</span> ${produto.fornecedor}</p>` : ''}
                    <p><span class="label">Preço:</span> R$ ${produto.custo.toFixed(2)} (custo) | R$ ${produto.venda.toFixed(2)} (venda)</p>
                    ${produto.observacoes ? `<p><span class="label">Observações:</span> ${produto.observacoes}</p>` : ''}
                    <p><span class="label">Estoque Total:</span> ${totalEstoque} | <span class="label">Gôndola Total:</span> ${totalGondola}</p>
                    <p><span class="label">Cores:</span></p>
                    <div>${cores}</div>
                    <div class="product-actions">
                        <button class="button" onclick="abrirReposicao('${produto.id}')">🔄 Repor Estoque</button>
                        <button class="button danger" onclick="deletarProduto('${produto.id}')">🗑️ Deletar</button>
                    </div>
                    <div id="reposicao-${produto.id}" style="display: none;" class="reposicao-form">
                        <div class="form-group">
                            <label>Selecione a Cor *</label>
                            <select id="cor-${produto.id}" onchange="carregarDadosReposicao('${produto.id}')">
                                <option value="">-- Escolha uma cor --</option>
                                ${Object.keys(produto.variacoes).map(cor => `<option value="${cor}">${cor}</option>`).join('')}
                            </select>
                        </div>
                        <div id="dados-${produto.id}" style="display: none; background: white; padding: 10px; border-radius: 5px; margin-bottom: 10px;">
                            <p><strong>Estoque Atual:</strong> <span id="estoque-${produto.id}">0</span></p>
                            <p><strong>Gôndola Atual:</strong> <span id="gondola-${produto.id}">0</span></p>
                        </div>
                        <div class="form-group">
                            <label>Quantidade que Saiu do Estoque *</label>
                            <input type="number" id="qtd-${produto.id}" placeholder="0" min="0">
                        </div>
                        <button class="button" onclick="registrarSaida('${produto.id}')">📤 Registrar Saída</button>
                        <button class="button secondary" onclick="fecharReposicao('${produto.id}')" style="margin-top: 10px; width: 100%;">Cancelar</button>
                    </div>
                `;
                produtosList.appendChild(div);
            });
        };

        window.abrirReposicao = function(produtoId) {
            document.getElementById(`reposicao-${produtoId}`).style.display = 'block';
        };

        window.fecharReposicao = function(produtoId) {
            document.getElementById(`reposicao-${produtoId}`).style.display = 'none';
        };

        window.carregarDadosReposicao = function(produtoId) {
            const cor = document.getElementById(`cor-${produtoId}`).value;
            if (cor && produtos[produtoId]) {
                const variacao = produtos[produtoId].variacoes[cor];
                document.getElementById(`estoque-${produtoId}`).textContent = variacao.estoque;
                document.getElementById(`gondola-${produtoId}`).textContent = variacao.gondola;
                document.getElementById(`dados-${produtoId}`).style.display = 'block';
            }
        };

        window.registrarSaida = function(produtoId) {
            const cor = document.getElementById(`cor-${produtoId}`).value;
            const quantidade = parseInt(document.getElementById(`qtd-${produtoId}`).value) || 0;

            if (!cor || quantidade <= 0) {
                alert('Preencha todos os campos!');
                return;
            }

            const variacao = produtos[produtoId].variacoes[cor];
            if (quantidade > variacao.estoque) {
                alert('Quantidade maior que o estoque!');
                return;
            }

            const novoEstoque = variacao.estoque - quantidade;
            set(ref(database, `produtos/${produtoId}/variacoes/${cor}`), {
                cor, estoque: novoEstoque, gondola: variacao.gondola
            }).then(() => {
                const historicoEntry = {
                    id: Date.now().toString(),
                    data: new Date().toISOString(),
                    produto: produtos[produtoId].nome,
                    cor, quantidade,
                    estoqueAnterior: variacao.estoque,
                    estoqueNovo: novoEstoque
                };
                push(ref(database, 'historico'), historicoEntry).then(() => {
                    alert('Saída registrada com sucesso!');
                    fecharReposicao(produtoId);
                    document.getElementById(`qtd-${produtoId}`).value = '';
                    document.getElementById(`cor-${produtoId}`).value = '';
                });
            });
        };

        window.deletarProduto = function(produtoId) {
            if (confirm('Deletar este produto?')) {
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
                        <div class="details">Saída: ${item.quantidade} unidades | Estoque: ${item.estoqueAnterior} → ${item.estoqueNovo}</div>
                    `;
                    historicoList.appendChild(div);
                });
            }
        }

        carregarDados();
    </script>
</body>
</html>
