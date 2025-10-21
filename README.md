<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Instituto Arara Azul</title>
<style>
/* ===== CSS ===== */
body {
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
img {
    max-width: 100%;
    height: auto;
}
section img {
    margin-bottom: 10px;
}
</style>
</head>
<body>
<header>
    <img src="https://via.placeholder.com/150x80?text=Logo+Instituto+Arara+Azul" alt="Logo Instituto Arara Azul">
    <nav>
        <ul>
            <li><a href="#inicio">Início</a></li>
            <li><a href="#projetos">Projetos</a></li>
            <li><a href="#cadastro">Cadastro</a></li>
        </ul>
    </nav>
</header>

<main>
    <!-- Início -->
    <section id="inicio">
        <h2>Sobre o Instituto</h2>
        <p>Missão: Ajudar comunidades carentes.<br>Visão: Um mundo mais justo.<br>Valores: Transparência, ética e solidariedade.</p>
        <h2>Equipe</h2>
        <img src="https://via.placeholder.com/300x200?text=Equipe" alt="Equipe Instituto Arara Azul">
        <p>Conheça nossa equipe dedicada de voluntários e colaboradores.</p>
        <h2>Contato</h2>
        <p>Email: contato@institutoararaazul.org | Telefone: (00) 0000-0000</p>
    </section>

    <!-- Projetos -->
    <section id="projetos">
        <h2>Oportunidades de Voluntariado</h2>
        <img src="https://via.placeholder.com/300x200?text=Voluntariado" alt="Voluntariado Instituto Arara Azul">
        <p>Participe e ajude em nossos projetos sociais.</p>

        <h2>Como Doar</h2>
        <img src="https://via.placeholder.com/300x200?text=Doacao" alt="Doação Instituto Arara Azul">
        <p>Saiba como apoiar financeiramente nossas ações.</p>
    </section>

    <!-- Cadastro -->
    <section id="cadastro">
        <h2>Cadastro de Voluntários / Doadores</h2>
        <form>
            <fieldset>
                <legend>Informações Pessoais</legend>
                <label for="nome">Nome Completo:</label>
                <input type="text" id="nome" name="nome" required>
                <label for="email">E-mail:</label>
                <input type="email" id="email" name="email" required>
                <label for="cpf">CPF:</label>
                <input type="text" id="cpf" name="cpf" pattern="\d{3}\.\d{3}\.\d{3}-\d{2}" placeholder="000.000.000-00" required>
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
    </section>
</main>

<footer>
    <p>&copy; 2025 Instituto Arara Azul. Todos os direitos reservados.</p>
</footer>

<script>
/* ===== JS ===== */
console.log("Projeto Instituto Arara Azul carregado");
</script>

</body>
</html>
