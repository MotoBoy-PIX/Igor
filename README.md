<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Salve, Família! - Apoie um Trabalhador</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-image: url('https://images.unsplash.com/photo-1514565131-fce0801e5785?ixlib=rb-1.2.1&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: #f5f5f5;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        .container {
            background-color: rgba(0, 0, 0, 0.7);
            backdrop-filter: blur(5px);
            border-radius: 15px;
            padding: 30px;
            max-width: 600px;
            margin: 20px;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        h1 {
            color: #f8c537;
            text-align: center;
            margin-bottom: 25px;
            font-size: 2.2em;
        }

        p {
            font-size: 1.1em;
            line-height: 1.6;
            margin-bottom: 20px;
            text-align: justify;
        }

        .pix-section {
            background-color: rgba(248, 197, 55, 0.1);
            border-left: 4px solid #f8c537;
            padding: 15px;
            margin: 25px 0;
            border-radius: 0 8px 8px 0;
        }

        .pix-key {
            font-family: monospace;
            font-size: 1.3em;
            font-weight: bold;
            color: #f8c537;
            word-break: break-all;
        }

        .copy-btn {
            background-color: #f8c537;
            color: #1a1a1a;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            font-weight: bold;
            cursor: pointer;
            margin-top: 10px;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .copy-btn:hover {
            background-color: #e6b732;
            transform: translateY(-2px);
        }

        .copy-btn:active {
            transform: translateY(0);
        }

        .blessing {
            text-align: center;
            font-style: italic;
            margin-top: 30px;
            font-size: 1.2em;
            color: #f8c537;
        }

        .emoji {
            font-size: 1.3em;
        }

        @media (max-width: 600px) {
            .container {
                padding: 20px;
            }
            
            h1 {
                font-size: 1.8em;
            }
            
            p {
                font-size: 1em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Seu pedido foi entregue! <span class="emoji">🙏</span></h1>
        
        <p>Entreguei sua comida sem comer um pedacinho.</p>
        
        <p>isso já merece um trocado, vai!.</p>
        
        <div class="pix-section">
            <p>Chave Pix:</p>
            <div class="pix-key" id="pixKey">425.353.518-62</div>
            <button class="copy-btn" onclick="copyPixKey()">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                    <path d="M4 1.5H3a2 2 0 0 0-2 2V14a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V3.5a2 2 0 0 0-2-2h-1v1h1a1 1 0 0 1 1 1V14a1 1 0 0 1-1 1H3a1 1 0 0 1-1-1V3.5a1 1 0 0 1 1-1h1v-1z"/>
                    <path d="M9.5 1a.5.5 0 0 1 .5.5v1a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1-.5-.5v-1a.5.5 0 0 1 .5-.5h3zm-3-1A1.5 1.5 0 0 0 5 1.5v1A1.5 1.5 0 0 0 6.5 4h3A1.5 1.5 0 0 0 11 2.5v-1A1.5 1.5 0 0 0 9.5 0h-3z"/>
                </svg>
                Copiar Chave
            </button>
        </div>
        
        <p>Sua ajuda fortalece mais do que você imagina.</p>
        
        <p class="blessing">Muito obrigado por ter lido essa mensagem. Que Deus te abençoe! <span class="emoji">🙌</span></p>
    </div>

    <script>
        function copyPixKey() {
            const pixKey = document.getElementById('pixKey').innerText;
            navigator.clipboard.writeText(pixKey).then(() => {
                const btn = document.querySelector('.copy-btn');
                btn.innerHTML = `
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                        <path d="M12.736 3.97a.733.733 0 0 1 1.047 0c.286.289.29.756.01 1.05L7.88 12.01a.733.733 0 0 1-1.065.02L3.217 8.384a.757.757 0 0 1 0-1.06.733.733 0 0 1 1.047 0l3.052 3.093 5.4-6.425a.247.247 0 0 1 .02-.022Z"/>
                    </svg>
                    Chave Copiada!
                `;
                setTimeout(() => {
                    btn.innerHTML = `
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                            <path d="M4 1.5H3a2 2 0 0 0-2 2V14a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V3.5a2 2 0 0 0-2-2h-1v1h1a1 1 0 0 1 1 1V14a1 1 0 0 1-1 1H3a1 1 0 0 1-1-1V3.5a1 1 0 0 1 1-1h1v-1z"/>
                            <path d="M9.5 1a.5.5 0 0 1 .5.5v1a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1-.5-.5v-1a.5.5 0 0 1 .5-.5h3zm-3-1A1.5 1.5 0 0 0 5 1.5v1A1.5 1.5 0 0 0 6.5 4h3A1.5 1.5 0 0 0 11 2.5v-1A1.5 1.5 0 0 0 9.5 0h-3z"/>
                        </svg>
                        Copiar Chave
                    `;
                }, 2000);
            });
        }
    </script>
</body>
</html>
