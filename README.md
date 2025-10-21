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

/* ===== Menu Responsivo ===== */
@media (max-width: 768px) {
    header nav ul {
        display: none;
        flex-direction: column;
        background-color: #333;
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
    <img src="https://via.placeholder.com/150x80?text=Logo+Instituto+Arara+Azul" alt="Logo Instituto Arara Azul">
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
    <section id="inicio">
        <h2>Sobre o Instituto</h2>
        <p><strong>Missão:</strong> Proteger animais silvestres, com foco especial nas araras-azuis.</p>
        <p><strong>Visão:</strong> Um mundo mais justo e equilibrado entre o ser humano e a natureza.</p>
        <p><strong>Valores:</strong> Transparência, ética e amor à vida.</p>

        <h2>Equipe</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/7/73/Anodorhynchus_hyacinthinus_-Brazil-8a.jpg" alt="Equipe Instituto Arara Azul">
        <p>Conheça nossa equipe dedicada de biólogos, veterinários e voluntários apaixonados pela fauna brasileira.</p>

        <h2>Contato</h2>
        <p>Email: contato@institutoararaazul.org | Telefone: (67) 3333-2222</p>
    </section>

    <section id="projetos">
        <h2>Oportunidades de Voluntariado</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/5/5f/Hyacinth_Macaw_in_flight_-Pantanal.jpg" alt="Voluntariado Instituto Arara Azul">
        <p>Participe de ações de resgate e monitoramento de araras-azuis no Pantanal.</p>

        <h2>Como Doar</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/b/b3/Hyacinth_Macaw_Blue_Parrot.jpg" alt="Doação Instituto Arara Azul">
        <p>Ajude com doações para manter nossos programas de proteção e reabilitação da fauna.</p>
    </section>

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
                <label for="dataNascimento">Data de Nascimento:</label>
                <input type="date" id="dataNascimento" name="dataNascimento" required>
            </fieldset>

            <fieldset>
                <legend>Endereço</legend>
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
function toggleMenu() {
    document.getElementById('nav-links').classList.toggle('show');
}
</script>

</body>
</html>
