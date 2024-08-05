<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Palavra ao Mover o Mouse</title>
    <style>
        #message {
            position: absolute;
            display: none;
            font-size: 20px;
            color: black;
        }
    </style>
</head>
<body>
    <div id="message">Olá!</div>

    <script>
        const message = document.getElementById('message');
        let timeout;

        document.addEventListener('mousemove', (event) => {
            // Define a posição da mensagem no local do mouse
            message.style
