<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para meu amor</title>

    <style>
        body {
            background-color: blue;
            position: relative;
        }
        .painel {
            margin: auto;
            background-color: aliceblue;
            width: 500px;
            height: 500px;
            border-radius: 20px;
            text-align: center;
            padding-top: 50px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }

        #sim {
            background-color: blue;
            height: 40px;
            width: 60px;
            border: 2px solid white;
            border-radius: 10px;
            color: white;
            margin-left: -50px;
        }

        #nao {        
            background-color: blue;
            position: absolute;
            height: 40px;
            width: 60px;
            border: 2px solid white;
            border-radius: 10px;
            color: white;
            margin-left: 10px;
        }
    </style>

</head>
<body>

    <div class="painel">
        <h1> Pro meu gatinho </h1>
        <h3>Aceita casar comigo? Ser meu até nossa morte?</h3>

        <a href="https://youtu.be/2teuNzIpsfI"><button id="sim"> Sim!!!! </button></a>
        <button onmouseover="fuja()" id="nao"> Não. </button>
        <img src="https://media1.tenor.com/m/WtukVW9vvE8AAAAC/love-you-totoro.gif" alt="">
    </div>

    <script>
        function fuja() {
            var botaoNao = document.getElementById("nao");

            var larguraJanela = window.innerWidth;
            var alturaJanela = window.innerHeight;

            var maxX = larguraJanela - botaoNao.offsetWidth;
            var maxY = alturaJanela - botaoNao.offsetHeight;
            
            var aleatorioX = Math.floor(Math.random() * maxX);
            var aleatorioY = Math.floor(Math.random() * maxY);

            botaoNao.style.left = aleatorioX + "px";
            botaoNao.style.top = aleatorioY + "px";
        }
    </script>
    
</body>
</html>
