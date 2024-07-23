# Somando Números

Este repositório contém um exemplo simples de uma aplicação web que soma dois números inseridos pelo usuário. A página HTML possui dois campos de entrada para os números e um botão que, quando clicado, exibe o resultado da soma.

## Descrição

A aplicação permite ao usuário inserir dois números e clicar no botão "Somar" para calcular e exibir a soma desses números.

## Estrutura do Projeto

- **index.html**: Contém a estrutura HTML, estilo CSS embutido e o código JavaScript para calcular a soma.

### index.html

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Somando Números</title>
    <style>
        body {
            font: normal 18pt Arial;
        }
    </style>
</head>
<body>
    <h1>Soma de Valores</h1>
    <input type="number" name="txtn1" id="txtn1"> +
    <input type="number" name="txtn2" id="txtn2">
    <input type="button" value="Somar" onclick="soma()">
    <div id="Res">Resultado</div>

    <script>
        function soma() {
            var tn1 = window.document.getElementById('txtn1');
            var tn2 = window.document.querySelector('input#txtn2');
            var Res = window.document.getElementById('Res');
            var n1 = Number(tn1.value);
            var n2 = Number(tn2.value);
            var s = n1 + n2;
            Res.innerHTML = `A soma entre ${n1} e ${n2} é igual a <strong>${s}</strong>`;
        }
    </script>
</body>
</html>

Como Executar
Faça o download ou clone este repositório.
Abra o arquivo index.html em um navegador web.
Insira dois números nos campos e clique no botão "Somar" para ver o resultado exibido na página.

Objetivo
Este exemplo foi criado para fins educacionais, com o objetivo de demonstrar como manipular o DOM e realizar cálculos usando JavaScript.

Contribuição
Sinta-se à vontade para fazer um fork deste repositório, melhorar o código e enviar pull requests. Feedbacks e sugestões são bem-vindos!

Contato
Para mais informações, entre em contato: [santhiago.takaesu2021@gmail.com]