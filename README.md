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
    background-color: #2e6da4;
    color: #fff;
    padding: 10px 20px;
}
header nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
header nav ul {
    list-style: none;
    display: flex;
    gap: 15px;
    margin: 0;
    padding: 0;
}
header nav ul li a {
    color: white;
    text-decoration: none;
}
.hamburger {
    display: none;
    flex-direction: column;
    cursor: pointer;
}
.hamburger span {
    height: 3px;
    width: 25px;
    background: white;
    margin-bottom: 5px;
    border-radius: 2px;
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
    background-color: #2e6da4;
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

/* ===== Menu Responsivo ===== */
@media (max-width: 768px) {
    header nav ul {
        display: none;
        flex-direction: column;
        background-color: #2e6da4;
        position: absolute;
        top: 60px;
        right: 0;
        width: 200px;
    }
    header nav ul.show {
        display: flex;
    }
    .hamburger {
        display: flex;
    }
}
</style>
</head>
<body>
<header>
    <img src="https://via.placeholder.com/150x80?text=Instituto+Arara+Azul" alt="Logo Instituto Arara Azul">
    <nav>
        <div class="hamburger" onclick="toggleMenu()">
            <span></span>
            <span></span>
            <span></span>
        </div>
        <ul id="nav-links">
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
        <p>O Instituto Arara Azul é uma ONG dedicada à **proteção das araras-azuis** e de outros animais silvestres em risco.  
        Atuamos em resgates, reabilitação e reintegração ao habitat natural.</p>
        <img src="https://via.placeholder.com/300x200?text=Araras+Azuis" alt="Araras Azuis no Pantanal">
        <h2>Contato</h2>
        <p>Email: contato@institutoararaazul.org | Telefone: (00) 0000-0000</p>
    </section>

    <!-- Projetos -->
    <section id="projetos">
        <h2>Projetos em Andamento</h2>
        <img src="https://via.placeholder.com/300x200?text=Reabilitacao+de+Animais" alt="Reabilitação de Animais">
        <p>Atuamos em projetos de resgate, educação ambiental e reintrodução de espécies ameaçadas.</p>

        <h2>Como Ajudar</h2>
        <img src="https://via.placeholder.com/300x200?text=Doacoes+e+Voluntariado" alt="Doações e Voluntariado">
        <p>Seja um voluntário ou faça uma doação para manter nossos projetos vivos.</p>
    </section>

    <!-- Cadastro -->
    <section id="cadastro">
        <h2>Cadastro de Voluntários / Doadores</h2>
        <form action="https://formspree.io/f/SEU_ID_AQUI" method="POST">
            <fieldset>
                <legend>Informações Pessoais</legend>
                <label for="nome">Nome Completo:</label>
                <input type="text" id="nome" name="nome" required>
                <label for="email">E-mail:</label>
                <input type="email" id="email" name="email" required>
                <label for="telefone">Telefone:</label>
                <input type="tel" id="telefone" name="telefone" placeholder="(00) 00000-0000" required>
            </fieldset>
            <button type="submit">Cadastrar</button>
        </form>
    </section>
</main>

<footer>
    <p>© 2025 Instituto Arara Azul. Todos os direitos reservados.</p>
</footer>

<script>
/* ===== JS ===== */
console.log("Projeto Instituto Arara Azul carregado");

// Menu hambúrguer
function toggleMenu() {
    document.getElementById('nav-links').classList.toggle('show');
}
</script>
</body>
</html>
