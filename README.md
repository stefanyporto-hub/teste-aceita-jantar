# <!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> ENTRADA </title>
 
     <style>
       body{
            background-color: #eee76b;
        }
        .painel{
            background-color: white;
            margin: auto ;
            width: 500px;
            height: 500px;
            border-radius: 20px;
            text-align: center;
            padding-top:50px;
            border:  3px solid #993cd4 ;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }

          #sim{
           height: 60px;
           width: 90px;
           background-color: #7e23c6;
           border: 2px solid white;
           border-radius: 10px;
           color:white;
           margin-left: -50px;
           cursor: pointer;
           
           
          }


          #nao{
           position: absolute;
           height: 60px;
           width: 90px;
           width: 90px;
           background-color: #7e23c6;
           border: 2px solid white;
           border-radius: 10px;
           color:white;
           margin-left: 10px;
           cursor: pointer;
          }
     </style>

</head>
<body>
 <div class="painel"> 
    <h1> Motivos para você sairmos em um date  </h1>

    <img src="/foto/emoji-emojis.gif">

    <h2>Quer saber os motivos?</h2>

   <a href="https://youtube.com/shorts/c6TSrYeist8?si=lBlLJGqtS3G_9lbd"><button id="sim">Sim</button></a> 
    <button id="nao"> Não</button>

  </div>

<script>
  const botao = document.getElementById("nao");

    // Lista de nomes possíveis
    const nomes = ["Certeza?", "Tá curiosa em", "É só clicar no sim ", "Vamos lá !", "Aperta"];

    botao.addEventListener("click", () => {
      // Mudar o texto do botão
      const novoNome = nomes[Math.floor(Math.random() * nomes.length)];
      botao.textContent = novoNome;

      // Mudar a posição do botão
      const larguraJanela = window.innerWidth;
      const alturaJanela = window.innerHeight;

      var maxX = larguraJanela - botao.offsetHeight
      var maxY = alturaJanela - botao.offsetHeight
    });
</script>

</body>
</html>
