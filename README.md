<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Página Web Responsiva</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#">Início</a></li>
                <li><a href="#">Sobre</a></li>
                <li><a href="#">Serviços</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h1>Bem-vindo à nossa página!</h1>
        <p>Explore nosso site para saber mais sobre nossos serviços.</p>
        <a href="#" class="cta-btn">Saiba mais</a>
    </section>

    <section class="content">
        <div class="card">
            <h2>Serviço 1</h2>
            <p>Descrição do serviço 1.</p>
        </div>
        <div class="card">
            <h2>Serviço 2</h2>
            <p>Descrição do serviço 2.</p>
        </div>
        <div class="card">
            <h2>Serviço 3</h2>
            <p>Descrição do serviço 3.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Todos os direitos reservados.</p>
    </footer>
</body>
</html>
/* Resetando margens e padding padrão */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Definindo fontes e cores base */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background: #333;
    color: #fff;
    padding: 1rem 0;
}

header nav ul {
    display: flex;
    justify-content: center;
    list-style-type: none;
}

header nav ul li {
    margin: 0 15px;
}

header nav ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
}

.hero {
    background: #3498db;
    color: #fff;
    text-align: center;
    padding: 2rem 0;
}

.hero h1 {
    margin-bottom: 1rem;
}

.hero .cta-btn {
    background: #e74c3c;
    padding: 10px 20px;
    color: white;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
}

.hero .cta-btn:hover {
    background: #c0392b;
}

.content {
    display: flex;
    justify-content: space-around;
    padding: 2rem 0;
    background-color: #fff;
}

.card {
    background-color: #f9f9f9;
    padding: 1rem;
    text-align: center;
    border-radius: 5px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    width: 30%;
}

.card h2 {
    margin-bottom: 1rem;
}

footer {
    text-align: center;
    padding: 1rem 0;
    background-color: #333;
    color: #fff;
}

/* Responsividade */
@media (max-width: 768px) {
    header nav ul {
        flex-direction: column;
    }

    .content {
        flex-direction: column;
        align-items: center;
    }

    .card {
        width: 80%;
        margin-bottom: 1rem;
    }
}

@media (max-width: 480px) {
    .hero h1 {
        font-size: 1.5rem;
    }

    .hero p {
        font-size: 1rem;
    }

    .hero .cta-btn {
        font-size: 1rem;
        padding: 8px 16px;
    }
}
