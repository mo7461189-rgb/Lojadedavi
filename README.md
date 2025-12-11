<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Loja do Davi</title>
    <style>
        body {
            font-family: Arial;
            background: #f5f5f5;
            margin: 0;
            padding: 20px;
        }
        header {
            text-align: center;
            margin-bottom: 30px;
        }
        .lang-btn {
            padding: 10px 16px;
            margin: 5px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            background: #333;
            color: white;
            font-size: 16px;
        }
        .produto {
            background: white;
            padding: 20px;
            border-radius: 12px;
            margin-bottom: 20px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h2 {
            margin-top: 0;
        }
    </style>

    <script>
        function setLanguage(lang) {
            document.querySelectorAll('.text-block').forEach(el => {
                el.style.display = 'none';
            });
            document.getElementById(lang).style.display = 'block';
        }
    </script>
</head>

<body>

<header>
    <h1>Loja do Davi</h1>
    <button class="lang-btn" onclick="setLanguage('pt')">Português</button>
    <button class="lang-btn" onclick="setLanguage('en')">Inglês</button>
    <button class="lang-btn" onclick="setLanguage('es')">Espanhol</button>
</header>

<div class="produto">

    <!-- PORTUGUÊS -->
    <div id="pt" class="text-block">
        <h2>Edit Profissional</h2>
        <p>Bem vindo à Lojadedavi! Aqui tem edits profissionais, 100% confiável. Obrigado!</p>
    </div>

    <!-- INGLÊS -->
    <div id="en" class="text-block" style="display:none;">
        <h2>Professional Edit</h2>
        <p>Welcome to Lojadedavi! Here you get professional edits, 100% reliable. Thank you!</p>
    </div>

    <!-- ESPANHOL -->
    <div id="es" class="text-block" style="display:none;">
        <h2>Edit Profesional</h2>
        <p>Bienvenido a Lojadedavi! Aquí tienes edits profesionales, 100% confiable. ¡Gracias!</p>
    </div>

</div>

</body>
</html>
