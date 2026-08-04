<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GÉOR – Controle de Estoque</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background: linear-gradient(135deg, #a8597e 0%, #6b3d5c 100%); min-height: 100vh; padding: 20px; }
        .container { max-width: 1200px; margin: 0 auto; background: white; border-radius: 15px; box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2); }
        .header { background: linear-gradient(135deg, #a8597e 0%, #6b3d5c 100%); color: white; padding: 30px; text-align: center; }
        .header h1 { font-size: 28px; margin-bottom: 5px; }
        .content { padding: 30px; }
        h2 { color: #a8597e; margin: 30px 0 20px 0; border-bottom: 2px solid #a8597e; padding-bottom: 10px; }
        .form-group { margin-bottom: 15px; }
        .form-group label { display: block; margin-bottom: 5px; font-weight: 600; color: #a8597e; font-size: 14px; }
        .form-group input, .form-group select, .form-group textarea { width: 100%; padding: 10px; border: 1px solid #ddd; border-radius: 5px; font-size: 14px; }
        .form-group input:focus, .form-group select:focus, .form-group textarea:focus { outline: none; border-color: #a8597e; box-shadow: 0 0 0 3px rgba(168, 89, 126, 0.1); }
        .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; }
        .form-row.three { grid-template-columns: 1fr 1fr 1fr; gap: 15px; }
        .button { background: linear-gradient(135deg, #a8597e 0%, #6b3d5c 100%); color: white; padding: 10px 20px; border: none; border-radius: 5px; cursor: pointer; font-weight: 600; }
        .button:hover { transform: translateY(-2px); }
        .button.danger { background: #e74c3c; }
        .button.success { background: #27ae60; }
        .button.add { width: 100%; margin-top: 10px; }
        .variations { background: #f9f9f9; padding: 15px; border-radius: 5px; margin: 15px 0; border-left: 4px solid #a8597e; }
        .variation-item { background: white; padding: 10px; border-radius: 5px; margin-bottom: 10px; display: grid; grid-template-columns: 1fr 1fr 1fr auto; gap: 10px; align-items: center; border-left: 3px solid #a8597e; }
        .variation-item p { margin: 0; color: #333; font-size: 13px; }
        .variation-item strong { color: #a8597e; }
        .product-item { background: #f9f9f9; padding: 15px; border-radius: 8px; margin-bottom: 15px; border-left: 4px solid #a8597e; }
        .product-item h3 { color: #a8597e; margin-bottom: 8px; }
        .product-item p { color: #666; font-size: 12px; margin-bottom: 5px; }
        .color-badge { display: inline-block; padding: 5px 10px; background: white; border: 1px solid #a8597e; border-radius: 3px; font-size: 11px; margin-right: 5px; margin-bottom: 5px; }
        .history-item { background: #f9f9f9; padding: 12px; border-radius: 5px; margin-bottom: 10px; border-left: 4px solid #a8597e; }
        .history-item .timestamp { color: #999; font-size: 11px; margin-bottom: 3px; }
        .history-item .action { color: #333; font-weight: 600; font-size: 13px; }
        .history-item .details { color: #666; font-size: 12px; margin-top: 3px; }
        .empty-state { text-align: center; padding: 30px; color: #999; }
        .alert { padding: 12px; border-radius: 5px; margin-bottom: 15px; }
        .alert.success { background: #d4edda; color: #155724; }
        .alert.error { background: #f8d7da; color: #721c24; }
        .search-box { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-bottom: 15px; }
        .search-box input, .search-box select { padding: 10px; border: 1px solid #ddd; border-radius: 5px; }
        .form-cadastro { background: #f9f9f9; padding: 15px; border-radius: 8px; margin-bottom: 20px; }
        .input-cor-estoque { display: grid; grid-template-columns: 1fr 1fr 1fr auto; gap: 10px; margin-bottom: 10px; align-items: flex-end; }
        .input-cor-estoque input { padding: 10px; border: 1px solid #ddd; border-radius: 5px; }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>💎 GÉOR – Controle de Estoque</h1>
            <p>Bolo Mania</p>
        </div>

        <div class="content">
            <!-- CADASTRO -->
            <h2>✏️ Cadastro de Produto</h2>
            <div id="checkinAlert"></div>

            <div class="form-cadastro">
                <div class="form-group">
                    <label>NOME / DESCRIÇÃO *</label>
                    <input type="text" id="produtoNome" placeholder="Ex: Anel Solitário">
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label>CÓDIGO *</label>
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

                <div class="variations">
                    <h3 style="color: #a8597e; margin-bottom: 15px; font-size: 16px;">CORES E ESTOQUE *</h3>

                    <!-- INPUTS PARA ADICIONAR COR -->
                    <div class="input-cor-estoque">
                        <input type="text" id="corInput" placeholder="Nome da cor" maxlength="30">
                        <input type="number" id="estoqueInput" placeholder="Estoque" min="0" value="0">
                        <input type="number" id="gondolaInput" placeholder="Gôndola" min="0" value="0">
                        <button class="button success" onclick="adicionarVariacao()">✓ Adicionar</button>
                    </div>

                    <!-- LISTA DE CORES ADICIONADAS -->
                    <div id="variacoesList"></div>
                </div>

                <button class="button" onclick="salvarProduto()" style="width: 100%;">✅ Salvar Produto</button>
            </div>

            <!-- PRODUTOS -->
            <h2>📦 Produtos Cadastrados</h2>
            <div class="search-box">
                <input type="text" id="searchProduto" placeholder="🔍 Buscar por nome ou código..." onkeyup="filtrarProdutos()">
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
            <div id="produtosList"></div>

            <!-- REPOSIÇÃO -->
            <h2>🔄 Reposição de Estoque</h2>
            <div id="reposicaoAlert"></div>
            <div class="form-cadastro">
                <div class="form-group">
                    <label>Selecione o Produto *</label>
                    <select id="reposicaoProduto" onchange="carregarCoresReposicao()">
                        <option value="">-- Escolha um produto --</option>
                    </select>
                </div>

                <div class="form-group">
                    <label>Selecione a Cor *</label>
                    <select id="reposicaoCor" onchange="carregarDadosReposicao()">
                        <option value="">-- Escolha uma cor --</option>
                    </select>
                </div>

                <div id="dadosReposicao" style="display: none; background: white; padding: 12px; border-radius: 5px; margin-bottom: 15px; border-left: 4px solid #ffc107;">
                    <p><strong>Estoque Atual:</strong> <span id="estoqueReposicao">0</span> unidades</p>
                    <p><strong>Gôndola Atual:</strong> <span id="gondolaReposicao">0</span> unidades</p>
                </div>

                <div class="form-group">
                    <label>Quantidade que Saiu do Estoque *</label>
                    <input type="number" id="quantidadeReposicao" placeholder="0" min="0">
                </div>

                <button class="button" onclick="registrarReposicao()" style="width: 100%;">🔄 Registrar Reposição</button>
            </div>

            <!-- HISTÓRICO -->
            <h2>📜 Histórico de Movimentos</h2>
            <div id="historicoList"></div>
        </div>
    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/10.7.0/firebase-app.js";
        import { getDatabase, ref, push, set, onValue, remove } from "https://www.gstatic.com/firebasejs/10.7.0/firebase-database.js";

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

        // SINCRONIZAR PRODUTOS EM TEMPO REAL
        onValue(ref(database, 'produtos'), (snapshot) => {
            if (snapshot.exists()) {
                produtos = snapshot.val();
            } else {
                produtos = {};
            }
            atualizarSelectReposicao();
            filtrarProdutos();
        });

        // SINCRONIZAR HISTÓRICO EM TEMPO REAL
        onValue(ref(database, 'historico'), (snapshot) => {
            if (snapshot.exists()) {
                historico = Object.values(snapshot.val()).sort((a, b) => new Date(b.data) - new Date(a.data));
            } else {
                historico = [];
            }
            atualizarHistorico();
        });

        window.adicionarVariacao = function() {
            const cor = document.getElementById('corInput').value.trim();
            const estoque = parseInt(document.getElementById('estoqueInput').value) || 0;
            const gondola = parseInt(document.getElementById('gondolaInput').value) || 0;

            if (!cor) {
                alert('Digite o nome da cor!');
                return;
            }

            // Verificar se a cor já existe
            if (variacoesCadastro.some(v => v.cor.toLowerCase() === cor.toLowerCase())) {
                alert('Esta cor já foi adicionada!');
                return;
            }

            variacoesCadastro.push({ cor, estoque, gondola });

            // Limpar inputs
            document.getElementById('corInput').value = '';
            document.getElementById('estoqueInput').value = '0';
            document.getElementById('gondolaInput').value = '0';
            document.getElementById('corInput').focus();

            renderizarVariacoes();
        };

        function renderizarVariacoes() {
            const container = document.getElementById('variacoesList');
            container.innerHTML = '';

            if (variacoesCadastro.length === 0) {
                container.innerHTML = '<p style="color: #999; text-align: center; padding: 10px;">Nenhuma cor adicionada ainda</p>';
                return;
            }

            variacoesCadastro.forEach((v, index) => {
                const div = document.createElement('div');
                div.className = 'variation-item';
                div.innerHTML = `
                    <p><strong>${v.cor}</strong></p>
                    <p>Estoque: <strong>${v.estoque}</strong></p>
                    <p>Gôndola: <strong>${v.gondola}</strong></p>
                    <button class="button danger" onclick="variacoesCadastro.splice(${index}, 1); renderizarVariacoes();">✕ Remover</button>
                `;
                container.appendChild(div);
            });
        }

        window.salvarProduto = function() {
            const nome = document.getElementById('produtoNome').value.trim();
            const codigo = document.getElementById('produtoCodigo').value.trim();
            const tipo = document.getElementById('produtoTipo').value;
            const custo = parseFloat(document.getElementById('produtoCusto').value) || 0;
            const venda = parseFloat(document.getElementById('produtoVenda').value) || 0;
            const alert = document.getElementById('checkinAlert');

            if (!nome || !codigo || !tipo || variacoesCadastro.length === 0) {
                alert.innerHTML = '<div class="alert error">Preencha todos os campos obrigatórios e adicione pelo menos uma cor!</div>';
                return;
            }

            const produtoId = Date.now().toString();
            const variacoes = {};

            variacoesCadastro.forEach(v => {
                variacoes[v.cor] = { cor: v.cor, estoque: v.estoque, gondola: v.gondola };
            });

            set(ref(database, `produtos/${produtoId}`), {
                id: produtoId,
                nome, codigo, tipo, custo, venda,
                dataCadastro: new Date().toISOString(),
                variacoes
            }).then(() => {
                alert.innerHTML = '<div class="alert success">✅ Produto salvo com sucesso!</div>';
                document.getElementById('produtoNome').value = '';
                document.getElementById('produtoCodigo').value = '';
                document.getElementById('produtoTipo').value = '';
                document.getElementById('produtoCusto').value = '';
                document.getElementById('produtoVenda').value = '';
                variacoesCadastro = [];
                renderizarVariacoes();
                setTimeout(() => { alert.innerHTML = ''; }, 3000);
            }).catch(error => {
                alert.innerHTML = `<div class="alert error">❌ Erro: ${error.message}</div>`;
            });
        };

        window.filtrarProdutos = function() {
            const termo = document.getElementById('searchProduto').value.toLowerCase();
            const tipo = document.getElementById('filterTipo').value;
            const produtosList = document.getElementById('produtosList');

            produtosList.innerHTML = '';

            let encontrados = Object.values(produtos).filter(p => {
                const nomeMatch = p.nome.toLowerCase().includes(termo) || p.codigo.toLowerCase().includes(termo);
                const tipoMatch = !tipo || p.tipo === tipo;
                return nomeMatch && tipoMatch;
            });

            if (encontrados.length === 0) {
                produtosList.innerHTML = '<div class="empty-state">Nenhum produto encontrado.</div>';
                return;
            }

            encontrados.forEach(produto => {
                let totalEstoque = 0, totalGondola = 0, cores = '';
                Object.values(produto.variacoes).forEach(v => {
                    cores += `<div class="color-badge">${v.cor}: E${v.estoque} | G${v.gondola}</div>`;
                    totalEstoque += v.estoque;
                    totalGondola += v.gondola;
                });

                const div = document.createElement('div');
                div.className = 'product-item';
                div.innerHTML = `
                    <h3>${produto.nome}</h3>
                    <p><strong>Código:</strong> ${produto.codigo}</p>
                    <p><strong>Tipo:</strong> ${produto.tipo}</p>
                    <p><strong>Preço:</strong> R$ ${produto.custo.toFixed(2)} (custo) | R$ ${produto.venda.toFixed(2)} (venda)</p>
                    <p><strong>Estoque Total:</strong> ${totalEstoque} | <strong>Gôndola Total:</strong> ${totalGondola}</p>
                    <p><strong>Cores:</strong></p>
                    <div>${cores}</div>
                    <button class="button danger" onclick="deletarProduto('${produto.id}')" style="margin-top: 10px; width: 100%;">🗑️ Deletar</button>
                `;
                produtosList.appendChild(div);
            });
        };

        function atualizarSelectReposicao() {
            const select = document.getElementById('reposicaoProduto');
            select.innerHTML = '<option value="">-- Escolha um produto --</option>';
            Object.values(produtos).forEach(p => {
                const option = document.createElement('option');
                option.value = p.id;
                option.textContent = `${p.nome} (${p.codigo})`;
                select.appendChild(option);
            });
        }

        window.carregarCoresReposicao = function() {
            const produtoId = document.getElementById('reposicaoProduto').value;
            const corSelect = document.getElementById('reposicaoCor');
            corSelect.innerHTML = '<option value="">-- Escolha uma cor --</option>';
            if (produtoId && produtos[produtoId]) {
                Object.keys(produtos[produtoId].variacoes).forEach(cor => {
                    const option = document.createElement('option');
                    option.value = cor;
                    option.textContent = cor;
                    corSelect.appendChild(option);
                });
            }
            document.getElementById('dadosReposicao').style.display = 'none';
        };

        window.carregarDadosReposicao = function() {
            const produtoId = document.getElementById('reposicaoProduto').value;
            const cor = document.getElementById('reposicaoCor').value;
            if (produtoId && cor && produtos[produtoId]) {
                const v = produtos[produtoId].variacoes[cor];
                document.getElementById('estoqueReposicao').textContent = v.estoque;
                document.getElementById('gondolaReposicao').textContent = v.gondola;
                document.getElementById('dadosReposicao').style.display = 'block';
            }
        };

        window.registrarReposicao = function() {
            const produtoId = document.getElementById('reposicaoProduto').value;
            const cor = document.getElementById('reposicaoCor').value;
            const quantidade = parseInt(document.getElementById('quantidadeReposicao').value) || 0;
            const alert = document.getElementById('reposicaoAlert');

            if (!produtoId || !cor || quantidade <= 0) {
                alert.innerHTML = '<div class="alert error">Preencha todos os campos!</div>';
                return;
            }

            const v = produtos[produtoId].variacoes[cor];
            if (quantidade > v.estoque) {
                alert.innerHTML = '<div class="alert error">Quantidade maior que o estoque!</div>';
                return;
            }

            const novoEstoque = v.estoque - quantidade;
            const novaGondola = v.gondola + quantidade;

            set(ref(database, `produtos/${produtoId}/variacoes/${cor}`), {
                cor, estoque: novoEstoque, gondola: novaGondola
            }).then(() => {
                push(ref(database, 'historico'), {
                    id: Date.now().toString(),
                    data: new Date().toISOString(),
                    tipo: 'Reposição',
                    produto: produtos[produtoId].nome,
                    cor, quantidade,
                    estoqueAnterior: v.estoque,
                    estoqueNovo: novoEstoque,
                    gondolaAnterior: v.gondola,
                    gondolaNova: novaGondola
                }).then(() => {
                    alert.innerHTML = '<div class="alert success">✅ Reposição registrada!</div>';
                    document.getElementById('quantidadeReposicao').value = '';
                    document.getElementById('reposicaoProduto').value = '';
                    document.getElementById('reposicaoCor').value = '';
                    document.getElementById('dadosReposicao').style.display = 'none';
                    setTimeout(() => { alert.innerHTML = ''; }, 3000);
                });
            }).catch(error => {
                alert.innerHTML = `<div class="alert error">❌ Erro: ${error.message}</div>`;
            });
        };

        window.deletarProduto = function(produtoId) {
            if (confirm('Deletar este produto?')) {
                remove(ref(database, `produtos/${produtoId}`));
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
                    div.innerHTML = `<div class="timestamp">${data.toLocaleString('pt-BR')}</div><div class="action">${item.produto} - ${item.cor}</div><div class="details">Tipo: ${item.tipo} | Quantidade: ${item.quantidade} | Estoque: ${item.estoqueAnterior} → ${item.estoqueNovo} | Gôndola: ${item.gondolaAnterior} → ${item.gondolaNova}</div>`;
                    historicoList.appendChild(div);
                });
            }
        }
    </script>
</body>
</html>
