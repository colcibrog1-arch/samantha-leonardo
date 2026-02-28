<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nosso Tempo</title>

<style>
body{
    margin:0;
    min-height:100vh;
    display:flex;
    justify-content:flex-start;
    align-items:center;
    padding:40px 0;
    overflow-y:auto;
    flex-direction:column;
    background:#1e90ff;
    background-image:url('https://minilua.net/wp-content/uploads/2020/04/shutterstock_760133494.jpg');
    background-size:cover;
    background-position:center;
    font-family:Arial, Helvetica, sans-serif;
    text-align:center;
    color:white;
}

#temporizador{
    font-size:28px;
    margin-bottom:20px;
    font-weight:bold;
}

.nomes{
    font-size:26px;
    margin-bottom:30px;
}

video{
    width:300px;
    border-radius:15px;
    margin-bottom:20px;
}

.texto{
    width:80%;
    max-width:600px;
    font-size:18px;
}
</style>
</head>

<body>

<div id="temporizador"></div>

<div class="nomes">
    Samanta ❤️ Leonardo
</div>

<video controls>
    <source src="zsamy.mp4" type="video/mp4">
    Seu navegador não suporta vídeo.
</video>

<div class="texto">
   ❤️ Eu te amo, meu maior bem! ❤️

Fazem 4 meses que estamos construindo essa linda história juntos… e parece que já passou tanto tempo, né? É como se nossas almas já se conhecessem há muito mais.

Eu quero que você saiba o quanto eu te amo. Não é um amor pequeno, é algo que cresce dentro de mim todos os dias. Você mudou a minha vida de um jeito que eu nunca imaginei que alguém pudesse mudar.

Eu fiz isso apenas para demonstrar o meu amor por você. Podemos passar por altos e baixos, mas eu nunca deixarei de te amar.

Me desculpa pelo meu jeito temperamental, pelo meu jeito de agir, pelo meu jeito de amar, pelo meu jeito de ser, pelo meu jeito de insistir. 

Eu sei que não sou perfeito. Às vezes erro, às vezes falho, às vezes deixo minhas inseguranças falarem mais alto… mas nunca, em momento algum, o meu amor por você diminui.

Você é a mulher com quem eu sonho construir tudo. Casar, ter filhos, ter uma moto kkk e um carro… construir um lindo futuro ao seu lado e viver uma vida inteira juntos.

Eu te amo mais do que palavras conseguem explicar. 
</div>

<script>
function atualizarTempo(){
    const dataInicial = new Date("2025-10-21T00:00:00");
    const agora = new Date();
    const diferenca = agora - dataInicial;

    const dias = Math.floor(diferenca / (1000 * 60 * 60 * 24));
    const horas = Math.floor((diferenca / (1000 * 60 * 60)) % 24);
    const minutos = Math.floor((diferenca / (1000 * 60)) % 60);
    const segundos = Math.floor((diferenca / 1000) % 60);

    document.getElementById("temporizador").innerHTML =
        `${dias} dias, ${horas} horas, ${minutos} minutos e ${segundos} segundos juntos`;
}

setInterval(atualizarTempo, 1000);
atualizarTempo();
</script>

</body>
</html>
