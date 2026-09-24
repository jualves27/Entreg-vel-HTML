# Entreg-vel-HTML
Estrutura base e formulário de inscrição de um mini vlog de receitas culinárias:



<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título do Site</title>

    <!-- CSS: -->
    <link rel="stylesheet" href="style.css">

</head>
<body>
    <h1>O meu site estilizado</h1>
</body>
</html
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog Cantinho do Canteiro | Receitas & Dicas</title>
</head>
<body>

    <!-- Cabeçalho Principal -->
    <header>
        <h1>🍳 Cantinho do Canteiro - Receitas do Dia</h1>
        <nav>
            <ul>
                <li><a href="#inicio">Início</a></li>
                <li><a href="#receitas">Receitas</a></li>
                <li><a href="#inscricao">Inscrição</a></li>
            </ul>
        </nav>
    </header>

    <!-- Conteúdo Principal -->
    <main>
        
        <!-- Seção de Publicações/Receitas -->
        <section id="receitas">
            <h2>Últimas Receitas do Blog</h2>
            
            <article id="inicio">
                <h3>Panqueca Americana Fofinha de Baunilha</h3>
                <p>Publicado em <time datetime="2026-09-23">23 de Setembro de 2026</time></p>
                <p>Aprenda o segredo para fazer panquecas super fofinhas e crocantes nas bordas. Uma receita simples, rápida e perfeita para o café da manhã de fim de semana!</p>
            </article>

            <article>
                <h3>Ovos Benedict Tradicionais com Molho Holandês</h3>
                <p>Publicado em <time datetime="2026-09-18">18 de Setembro de 2026</time></p>
                <p>Passo a passo completo para fazer o ovo poché no ponto certo e emulsionar o molho holandês sem empelotar.</p>
            </article>
        </section>

        <!-- Seção do Formulário de Inscrição -->
        <section id="inscricao">
            <h2>Formulário de Inscrição na Newsletter Gastronômica</h2>
            <p>Cadastre-se para receber um e-book gratuito com 10 receitas de brunch e novos posts semanais!</p>

            <form action="#" method="get">
                
                <fieldset>
                    <legend>Dados do Leitor</legend>

                    <p>
                        <label for="nome">Nome Completo:</label><br>
                        <input type="text" id="nome" name="nome" placeholder="Digite seu nome completo" required>
                    </p>

                    <p>
                        <label for="email">E-mail de Contato:</label><br>
                        <input type="email" id="email" name="email" placeholder="seuemail@exemplo.com" required>
                    </p>

                    <p>
                        <label for="nivel">Seu nível na cozinha:</label><br>
                        <select id="nivel" name="nivel">
                            <option value="iniciante">Iniciante</option>
                            <option value="intermediario">Intermediário</option>
                            <option value="avancado">Avançado / Chef Amador</option>
                        </select>
                    </p>
                </fieldset>

                <fieldset>
                    <legend>Preferências Culinárias</legend>

                    <p>Quais tipos de receita você prefere receber?</p>

                    <p>
                        <input type="checkbox" id="doces" name="preferencias" value="doces">
                        <label for="doces">Doces e Sobremesas</label>
                    </p>

                    <p>
                        <input type="checkbox" id="salgados" name="preferencias" value="salgados">
                        <label for="salgados">Opções Salgadas e Lanches</label>
                    </p>

                    <p>
                        <input type="checkbox" id="fit" name="preferencias" value="saudavel">
                        <label for="fit">Receitas Saudáveis e Funcionais</label>
                    </p>
                </fieldset>

                <p>
                    <button type="submit">Quero Me Inscrever</button>
                    <button type="reset">Limpar Dados</button>
                </p>

            </form>
        </section>

    </main>

    <!-- Barra Lateral -->
    <aside>
        <h2>Sobre o Blog</h2>
        <p>O Cantinho do Canteiro é um espaço dedicado aos amantes da culinária prática, focado em ensinar técnicas simples para transformar refeições diárias em momentos especiais.</p>
        <p>Siga no Instagram: <strong>@cantinho.culinaria</strong></p>
    </aside>

    <!-- Rodapé -->
    <footer>
        <p>&copy; 2026 Cantinho do Canteiro. Todos os direitos reservados.</p>
    </footer>
</body>
</html>

/* ==========================================================================
   Configurações Gerais e Variáveis
   ========================================================================== */
:root {
    --primary-color: #e67e22;      /* Laranja acolhedor */
    --primary-hover: #d35400;
    --secondary-color: #7f8c8d;    /* Cinzento neutro */
    --bg-color: #f8f9fa;           /* Fundo levemente acinzentado */
    --card-bg: #ffffff;            /* Fundo dos cartões */
    --text-color: #2c3e50;         /* Texto num tom escuro suave */
    --border-color: #e2e8f0;
    --radius: 8px;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: var(--bg-color);
    color: var(--text-color);
    line-height: 1.6;
}

/* ==========================================================================
   Cabeçalho e Navegação
   ========================================================================== */
header {
    background-color: #fff;
    border-bottom: 2px solid var(--border-color);
    padding: 1rem 2rem;
    box-shadow: 0 2px 4px rgba(0,0,0,0.02);
}

.header-container {
    max-width: 1100px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 1rem;
}

header h1 {
    font-size: 1.6rem;
    color: var(--primary-color);
}

nav ul {
    list-style: none;
    display: flex;
    gap: 1.5rem;
}

nav a {
    text-decoration: none;
    color: var(--text-color);
    font-weight: 600;
    transition: color 0.2s;
}

nav a:hover {
    color: var(--primary-color);
}

/* ==========================================================================
   Estrutura de Layout (Main + Aside)
   ========================================================================== */
.main-container {
    max-width: 1100px;
    margin: 2rem auto;
    padding: 0 1rem;
    display: grid;
    grid-template-columns: 1fr;
    gap: 2rem;
}

/* Layout em telas maiores (Desktop) */
@media (min-width: 768px) {
    .main-container {
        grid-template-columns: 2.5fr 1fr;
    }
}

/* Estilo de Cartões Genericamente */
.card {
    background-color: var(--card-bg);
    padding: 1.5rem;
    border-radius: var(--radius);
    border: 1px solid var(--border-color);
    margin-bottom: 1.5rem;
    box-shadow: 0 2px 5px rgba(0,0,0,0.03);
}

.card h2 {
    color: var(--primary-color);
    margin-bottom: 1rem;
    border-bottom: 2px solid var(--bg-color);
    padding-bottom: 0.5rem;
}

.card h3 {
    margin-bottom: 0.2rem;
}

.meta {
    font-size: 0.85rem;
    color: var(--secondary-color);
    margin-bottom: 0.8rem;
}

/* ==========================================================================
   Estilização do Formulário
   ========================================================================== */
fieldset {
    border: 1px solid var(--border-color);
    border-radius: var(--radius);
    padding: 1.2rem;
    margin: 1.2rem 0;
}

legend {
    font-weight: bold;
    color: var(--primary-color);
    padding: 0 0.5rem;
}

.form-group {
    margin-bottom: 1rem;
}

.form-group label {
    display: block;
    margin-bottom: 0.3rem;
    font-weight: 500;
}

input[type="text"],
input[type="email"],
select {
    width: 100%;
    padding: 0.6rem;
    border: 1px solid var(--border-color);
    border-radius: 4px;
    font-size: 0.95rem;
    outline: none;
}

input[type="text"]:focus,
input[type="email"]:focus,
select:focus {
    border-color: var(--primary-color);
}

.checkbox-group {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    margin-bottom: 0.5rem;
}

/* Botões */
.form-buttons {
    display: flex;
    gap: 1rem;
    margin-top: 1rem;
}

.btn {
    padding: 0.6rem 1.2rem;
    border: none;
    border-radius: 4px;
    font-weight: bold;
    cursor: pointer;
    transition: background 0.2s;
}

.btn-primary {
    background-color: var(--primary-color);
    color: #fff;
}

.btn-primary:hover {
    background-color: var(--primary-hover);
}

.btn-secondary {
    background-color: var(--secondary-color);
    color: #fff;
}

.btn-secondary:hover {
    background-color: #6c757d;
}

/* ==========================================================================
   Barra Lateral e Rodapé
   ========================================================================== */
aside hr {
    border: 0;
    height: 1px;
    background: var(--border-color);
    margin: 1rem 0;
}

footer {
    text-align: center;
    padding: 1.5rem;
    background-color: #fff;
    border-top: 1px solid var(--border-color);
    margin-top: 2rem;
    font-size: 0.9rem;
    color: var(--secondary-color);
}
