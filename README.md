# 4-Bimestre-projeto-2
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Livraria Horizonte Azul</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Barra Superior de Acessibilidade e Volume -->
    <nav class="barra-controles" aria-label="Controles de Leitura e Volume">
        <div class="grupo-controle">
            <span>Texto:</span>
            <button id="btnAumenta" class="btn-icone" title="Aumentar letra">A+</button>
            <button id="btnDiminui" class="btn-icone" title="Diminuir letra">A-</button>
        </div>

        <div class="grupo-controle">
            <span id="iconeVolume">🔊</span>
            <label for="controleVolume">Volume:</label>
            <input type="range" id="controleVolume" min="0" max="1" step="0.1" value="1">
            <button id="btnPararTudo" class="btn-parar" title="Parar leitura">⏹️ Parar</button>
        </div>
    </nav>

    <!-- Cabeçalho -->
    <header class="cabecalho">
        <h1>📚 Livraria Horizonte Azul</h1>
        <p>Histórias incríveis ao alcance dos seus olhos e ouvidos</p>
    </header>

    <!-- Catálogo de Livros -->
    <main class="container">
        <h2 class="titulo-secao">Destaques da Semana</h2>

        <div class="grade-livros">
            
            <!-- Livro 1 -->
            <article class="card-livro">
                <div class="capa-simulada">📖</div>
                <h3>O Pequeno Príncipe</h3>
                <p class="autor">Antoine de Saint-Exupéry</p>
                <p class="sinopse" id="sinopse-1">
                    Um piloto cai com seu avião no deserto do Saara e encontra um jovem príncipe vindo de um pequeno asteroide, que compartilha lições profundas sobre amizade, amor e o verdadeiro sentido da vida.
                </p>
                <div class="acoes-card">
                    <button class="btn-ouvir" onclick="lerSinopse('sinopse-1', this)">
                        🔊 Ouvir Sinopse
                    </button>
                    <span class="preco">R$ 34,90</span>
                    <button class="btn-comprar" onclick="comprarLivro('O Pequeno Príncipe')">
                        🛒 Comprar
                    </button>
                </div>
            </article>

            <!-- Livro 2 -->
            <article class="card-livro">
                <div class="capa-simulada">📘</div>
                <h3>Dom Casmurro</h3>
                <p class="autor">Machado de Assis</p>
                <p class="sinopse" id="sinopse-2">
                    Bentinho narra sua juventude e o intenso romance com Capitu, marcado por memórias nostálgicas e pela eterna dúvida sobre a fidelidade de seu grande amor.
                </p>
                <div class="acoes-card">
                    <button class="btn-ouvir" onclick="lerSinopse('sinopse-2', this)">
                        🔊 Ouvir Sinopse
                    </button>
                    <span class="preco">R$ 29,90</span>
                    <button class="btn-comprar" onclick="comprarLivro('Dom Casmurro')">
                        🛒 Comprar
                    </button>
                </div>
            </article>

            <!-- Livro 3 -->
            <article class="card-livro">
                <div class="capa-simulada">📙</div>
                <h3>A Revolução dos Bichos</h3>
                <p class="autor">George Orwell</p>
                <p class="sinopse" id="sinopse-3">
                    Os animais de uma fazenda se rebelam contra seus donos humanos em busca de igualdade e liberdade, mas logo descobrem que o poder pode corromper até os antigos companheiros.
                </p>
                <div class="acoes-card">
                    <button class="btn-ouvir" onclick="lerSinopse('sinopse-3', this)">
                        🔊 Ouvir Sinopse
                    </button>
                    <span class="preco">R$ 39,90</span>
                    <button class="btn-comprar" onclick="comprarLivro('A Revolução dos Bichos')">
                        🛒 Comprar
                    </button>
                </div>
            </article>

        </div>
    </main>

    <!-- Notificação simples de compra -->
    <div id="avisoCompra" class="aviso-compra"></div>

    <footer class="rodape">
        <p>Livraria Horizonte Azul &copy; 2026 - Leitura acessível para todos</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
