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
    background-color: #0b3d2e;
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
    background-color: #0b3d2e;
    color: white;
    border: none;
    cursor: pointer;
}
img {
    max-width: 100%;
    height: auto;
    border-radius: 6px;
}
section img {
    margin-bottom: 10px;
}

/* ===== Menu Responsivo ===== */
@media (max-width: 768px) {
    header nav ul {
        display: none;
        flex-direction: column;
        background-color: #0b3d2e;
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
    <img src="https://upload.wikimedia.org/wikipedia/commons/7/73/Anodorhynchus_hyacinthinus_-Brazil-8a.jpg" alt="Logo Instituto Arara Azul" width="120">
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
        <p><strong>Missão:</strong> Proteger e preservar as araras-azuis e outras aves silvestres ameaçadas de extinção, promovendo educação ambiental e conservação dos habitats naturais.</p>
        <p><strong>Visão:</strong> Um futuro em que a biodiversidade brasileira seja respeitada e preservada para as próximas gerações.</p>
        <p><strong>Valores:</strong> Amor à natureza, ética, transparência e sustentabilidade.</p>
        <h2>Equipe</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/b/b3/Hyacinth_Macaw_Blue_Parrot.jpg" alt="Equipe Instituto Arara Azul">
        <p>Somos biólogos, veterinários e voluntários apaixonados pela fauna brasileira, unidos pela proteção das araras-azuis.</p>
        <h2>Contato</h2>
        <p>Email: contato@institutoararaazul.org | Telefone: (67) 3333-2222</p>
    </section>

    <!-- Projetos -->
    <section id="projetos">
        <h2>Projetos em Destaque</h2>
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/16/Anodorhynchus_hyacinthinus-2.jpg" alt="Projeto Arara Azul">
        <p><strong>Projeto Arara Livre:</strong> Reabilitação e soltura de araras-azuis resgatadas do tráfico de animais.</p>

        <img src="https://upload.wikimedia.org/wikipedia/commons/f/f1/Hyacinth_Macaw_Brazil.jpg" alt="Educação Ambiental">
        <p><strong>Educação Ambiental nas Escolas:</strong> Conscientização sobre a importância da fauna e do combate ao tráfico de animais silvestres.</p>

        <img src="https://upload.wikimedia.org/wikipedia/commons/5/5f/Hyacinth_Macaw_in_flight_-Pantanal.jpg" alt="Preservação de Habitat">
        <p><strong>Preservação do Habitat:</strong> Ações de reflorestamento e monitoramento das áreas de nidificação no Pantanal.</p>
    </section>

    <!-- Cadastro -->
    <section id="cadastro">
        <h2>Cadastre-se como Voluntário ou Doador</h2>
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
            <button type="submit">Enviar Cadastro</button>
        </form>
    </section>
</main>

<footer>
    <p>&copy; 2025 Instituto Arara Azul. Todos os direitos reservados.</p>
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
