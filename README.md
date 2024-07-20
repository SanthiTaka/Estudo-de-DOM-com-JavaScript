Estudo de DOM com JavaScript
Este repositório contém um exemplo simples de manipulação do DOM (Document Object Model) usando JavaScript. O código demonstra como interagir com elementos HTML através de eventos como clique, entrada do mouse e saída do mouse.

Descrição do Projeto
O projeto consiste em uma página HTML com um único elemento div que reage a diferentes eventos do usuário:

Clique (onclick): Quando o usuário clica na div, o texto é alterado para "Clicou" e a cor de fundo muda para vermelho.
Entrada do mouse (onmouseenter): Quando o usuário passa o mouse sobre a div, o texto é alterado para "Entrou".
Saída do mouse (onmouseout): Quando o usuário move o mouse para fora da div, o texto é alterado para "Saiu".
Estrutura do Projeto
index.html: Contém a estrutura HTML e o estilo CSS embutido.
script.js: Contém o código JavaScript para manipulação do DOM (neste exemplo, o script está embutido no HTML).
index.html
html
Copiar código
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DOM</title>
    <style>
        div#area {
            font: arial;
            background-color: rgb(0, 255, 17);
            color: white;
            width: 200px;
            height: 200px;
            line-height: 200px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div id="area" onclick="clicar()" onmouseenter="entrar()" onmouseout="sair()">
        interaja
    </div>

    <script>
        var a = window.document.getElementById('area')
        function clicar() {
            a.innerText = 'Clicou'
            a.style.background = 'red'
        }
        function entrar() {
            a.innerText = 'Entrou'
        }
        function sair() {
            a.innerText = 'Saiu'
        }
    </script>
</body>
</html>
Como Executar
Faça o download ou clone este repositório.
Abra o arquivo index.html em um navegador web.
Interaja com a div para ver as mudanças de texto e cor em resposta aos eventos do mouse.
Objetivo
Este exemplo foi criado para fins educacionais, com o objetivo de demonstrar como manipular o DOM usando JavaScript e como reagir a eventos do usuário para criar interações dinâmicas em uma página web.

Contribuição
Sinta-se à vontade para fazer um fork deste repositório, melhorar o código e enviar pull requests. Feedbacks e sugestões são bem-vindos!


