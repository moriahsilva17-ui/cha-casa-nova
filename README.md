# cha-casa-nova
Lista de presentes para o chá de casa nova
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Chá de Casa Nova 💛</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background: #fdf6f0;
            color: #333;
        }

        header {
            background: #d4a373;
            color: white;
            text-align: center;
            padding: 30px 20px;
        }

        header h1 {
            margin: 0;
            font-size: 2.5em;
        }

        header p {
            margin-top: 10px;
            font-size: 1.1em;
        }

        .container {
            max-width: 1000px;
            margin: 30px auto;
            padding: 0 20px;
        }

        .itens {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .item {
            background: white;
            border-radius: 12px;
            padding: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.08);
            text-align: center;
            transition: 0.2s;
        }

        .item:hover {
            transform: translateY(-4px);
        }

        .item img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 8px;
        }

        .item h3 {
            margin: 10px 0 5px;
        }

        .item button {
            margin-top: 8px;
            padding: 8px 12px;
            border: none;
            border-radius: 6px;
            background: #d4a373;
            color: white;
            cursor: pointer;
        }

        .item button.reservado {
            background: #999;
            cursor: not-allowed;
        }

        footer {
            text-align: center;
            padding: 20px;
            margin-top: 40px;
            font-size: 0.9em;
            color: #777;
        }
    </style>
</head>
<body>

<header>
    <h1>Chá de Casa Nova do João & Maria 🏡</h1>
    <p>Estamos montando nosso cantinho com muito amor. Se quiser nos presentear, escolha um item abaixo 💛</p>
</header>

<div class="container">
    <div class="itens">

        <div class="item">
            <img src="https://images.unsplash.com/photo-1586201375761-83865001e31c" alt="Jogo de Panelas">
            <h3>Jogo de Panelas</h3>
            <button onclick="reservar(this)">Reservar</button>
        </div>

        <div class="item">
            <img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c" alt="Jogo de Cama">
            <h3>Jogo de Cama</h3>
            <button onclick="reservar(this)">Reservar</button>
        </div>

        <div class="item">
            <img src="https://images.unsplash.com/photo-1598300053653-1c6bfa1e0f62" alt="Toalhas de Banho">
            <h3>Toalhas de Banho</h3>
            <button onclick="reservar(this)">Reservar</button>
        </div>

        <div class="item">
            <img src="https://images.unsplash.com/photo-1583778176476-4a8b02b1b1e2" alt="Liquidificador">
            <h3>Liquidificador</h3>
            <button onclick="reservar(this)">Reservar</button>
        </div>

        <div class="item">
            <img src="https://images.unsplash.com/photo-1588854337115-1c67d9247e4d" alt="Conjunto de Pratos">
            <h3>Conjunto de Pratos</h3>
            <button onclick="reservar(this)">Reservar</button>
        </div>

        <div class="item">
            <img src="https://images.unsplash.com/photo-1578898887932-dce23a595ad4" alt="Cafeteira">
            <h3>Cafeteira</h3>
            <button onclick="reservar(this)">Reservar</button>
        </div>

    </div>
</div>

<footer>
    Com carinho, João & Maria 💍✨
</footer>

<script>
    function reservar(botao) {
        botao.textContent = "Reservado 💛";
        botao.classList.add("reservado");
        botao.disabled = true;
    }
</script>

</body>
</html>
