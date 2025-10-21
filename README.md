# Nome da pasta principal do projeto
project_name = "ONG-Platform"

# Estrutura de pastas
folders = [
    "css",
    "js",
    "img"
]

# Conteúdo dos arquivos HTML
index_html = """<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ONG Exemplo - Página Inicial</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <img src="img/logo.png" alt="Logo ONG Exemplo" width="150">
        <nav>
            <ul>
                <li><a href="index.html">Início</a></li>
                <li><a href="projetos.html">Projetos</a></li>
                <li><a href="cadastro.html">Cadastro</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h2>Sobre a ONG</h2>
            <p>Missão: Ajudar comunidades carentes.<br>Visão: Um mundo mais justo.<br>Valores: Transparência, ética e solidariedade.</p>
        </section>
        <section>
            <h2>Equipe</h2>
            <p>Conheça nossa equipe dedicada de voluntários e colaboradores.</p>
        </section>
        <section>
            <h2>Contato</h2>
            <p>Email: contato@ongexemplo.org | Telefone: (00) 0000-0000</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 ONG Exemplo. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
"""

projetos_html = """<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ONG Exemplo - Projetos</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <h1>Projetos Sociais</h1>
        <nav>
            <ul>
                <li><a href="index.html">Início</a></li>
                <li><a href="projetos.html">Projetos</a></li>
                <li><a href="cadastro.html">Cadastro</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h2>Oportunidades de Voluntariado</h2>
            <img src="img/voluntario.jpg" alt="Voluntariado" width="300">
            <p>Participe e ajude em nossos projetos sociais.</p>
        </section>
        <section>
            <h2>Como Doar</h2>
            <img src="img/projeto1.jpg" alt="Doação" width="300">
            <p>Saiba como apoiar financeiramente nossas ações.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 ONG Exemplo. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
"""

cadastro_html = """<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cadastro - ONG Exemplo</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <h1>Cadastro de Voluntários / Doadores</h1>
        <nav>
            <ul>
                <li><a href="index.html">Início</a></li>
                <li><a href="projetos.html">Projetos</a></li>
                <li><a href="cadastro.html">Cadastro</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <form>
            <fieldset>
                <legend>Informações Pessoais</legend>
                <label for="nome">Nome Completo:</label>
                <input type="text" id="nome" name="nome" required>
                <label for="email">E-mail:</label>
                <input type="email" id="email" name="email" required>
                <label for="cpf">CPF:</label>
                <input type="text" id="cpf" name="cpf" pattern="\\d{3}\\.\\d{3}\\.\\d{3}-\\d{2}" placeholder="000.000.000-00" required>
                <label for="telefone">Telefone:</label>
                <input type="tel" id="telefone" name="telefone" placeholder="(00) 00000-0000" required>
                <label for="dataNascimento">Data de Nascimento:</label>
                <input type="date" id="dataNascimento" name="dataNascimento" required>
            </fieldset>
            <fieldset>
                <legend>Endereço</legend>
                <label for="cep">CEP:</label>
                <input type="text" id="cep" name="cep" placeholder="00000-000" required>
                <label for="cidade">Cidade:</label>
                <input type="text" id="cidade" name="cidade" required>
                <label for="estado">Estado:</label>
                <input type="text" id="estado" name="estado" required>
            </fieldset>
            <button type="submit">Cadastrar</button>
        </form>
    </main>
    <footer>
        <p>&copy; 2025 ONG Exemplo. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
"""

# CSS básico
style_css = """body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}
header, footer {
    background-color: #333;
    color: #fff;
    padding: 10px 20px;
}
header nav ul {
    list-style: none;
    display: flex;
    gap: 15px;
}
header nav ul li a {
    color: white;
    text-decoration: none;
}
main {
    padding: 20px;
}
form {
    background: #fff;
    padding: 20px;
    border-radius: 5px;
}
fieldset {
    margin-bottom: 15px;
    border: 1px solid #ccc;
    padding: 10px;
}
label {
    display: block;
    margin-bottom: 5px;
}
input, button {
    width: 100%;
    padding: 8px;
    margin-bottom: 10px;
}
button {
    background-color: #333;
    color: white;
    border: none;
    cursor: pointer;
}
"""

# JS básico
script_js = """console.log("Projeto ONG carregado");"""

# Criar pasta principal
os.makedirs(project_name, exist_ok=True)

# Criar subpastas
for folder in folders:
    os.makedirs(os.path.join(project_name, folder), exist_ok=True)

# Criar arquivos HTML
with open(os.path.join(project_name, "index.html"), "w", encoding="utf-8") as f:
    f.write(index_html)

with open(os.path.join(project_name, "projetos.html"), "w", encoding="utf-8") as f:
    f.write(projetos_html)

with open(os.path.join(project_name, "cadastro.html"), "w", encoding="utf-8") as f:
    f.write(cadastro_html)

# Criar CSS
with open(os.path.join(project_name, "css/style.css"), "w", encoding="utf-8") as f:
    f.write(style_css)

# Criar JS
with open(os.path.join(project_name, "js/script.js"), "w", encoding="utf-8") as f:
    f.write(script_js)

# Criar placeholders de imagens
placeholder_images = ["logo.png", "projeto1.jpg", "voluntario.jpg"]
for img in placeholder_images:
    open(os.path.join(project_name, "img", img), "a").close()

print("Projeto ONG gerado com sucesso na pasta 'ONG-Platform'.")
