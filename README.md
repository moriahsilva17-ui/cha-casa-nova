# cha-casa-nova
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Chá de Casa Nova - Anthony & Moriah 💙</title>

<style>
body {
    font-family: 'Segoe UI', sans-serif;
    margin: 0;
    background: #eef5fb;
    color: #2c3e50;
}

header {
    background: #5fa8d3;
    color: white;
    text-align: center;
    padding: 35px 15px;
}

header h1 {
    margin: 0;
    font-size: 2em;
}

.container {
    max-width: 1100px;
    margin: 30px auto;
    padding: 0 15px;
}

.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 20px;
}

.card {
    background: white;
    border-radius: 14px;
    padding: 18px;
    box-shadow: 0 6px 14px rgba(0,0,0,0.08);
    text-align: center;
}

.card img {
    width: 80px;
    margin-bottom: 10px;
    opacity: 0.8;
}

.card h3 {
    margin: 6px 0;
}

.preco {
    font-weight: bold;
    color: #5fa8d3;
    margin: 6px 0;
}

button {
    padding: 8px 12px;
    border: none;
    border-radius: 6px;
    background: #5fa8d3;
    color: white;
    cursor: pointer;
}

footer {
    text-align: center;
    padding: 25px;
    margin-top: 30px;
    color: #777;
}
</style>
</head>

<body>

<header>
    <h1>Chá de Casa Nova de Anthony & Moriah 💙🏡</h1>
    <p>Escolha um presente e envie o valor via Pix ✨</p>
</header>

<div class="container">
<div class="grid">

<script>
const pix = "SUA_CHAVE_PIX_AQUI";

const icone = "https://cdn-icons-png.flaticon.com/512/1046/1046857.png"; // ícone minimalista

const itens = [
["Microondas",350],
["Liquidificador",120],
["Copos",80],
["Panelas",300],
["Frigideira",90],
["Talheres",150],
["Potes",70],
["Tábua",40],
["Travessa",60],
["Jarra",45],
["Air fryer",400],
["Tabuleiros",100],
["Pratos",180],
["Xícara",85],
["Escorredor",55],
["Peneira",30],
["Ralador",35],
["Travesseiro",70],
["Televisão",900],
["Ferro de passar",120],
["Jogo de cama",200],
["Kit toalha de banho",150],
["Kit toalha de rosto",80],
["Kit fronhas",60]
];

itens.forEach(item => {
document.write(`
<div class="card">
<img src="${icone}" alt="Ícone">
<h3>${item[0]}</h3>
<p class="preco">R$ ${item[1]},00</p>
<button onclick="pagar(${item[1]})">Pagar com Pix</button>
</div>
`);
});

function pagar(valor){
navigator.clipboard.writeText(pix);
alert("Chave Pix copiada 💙\\nValor do presente: R$ " + valor + ",00");
}
</script>

</div>
</div>

<footer>
Com amor, Anthony & Moriah 💍✨
</footer>

</body>
</html>
