<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Corte Seguro - Guia do Barbeiro</title>
    <style>
        :root {
            --gold: #d4af37;
            --dark-gold: #aa8a2e;
            --bg-dark: #121212;
            --card-bg: #1e1e1e;
            --text-light: #f0f0f0;
            --accent: #e67e22;
        }

        body { 
            margin: 0; 
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; 
            background: var(--bg-dark); 
            color: var(--text-light); 
            scroll-behavior: smooth; 
        }

        /* CAPA COMPACTA E ACOLHEDORA */
        .cover {
            background: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.8)), url('https://images.unsplash.com/photo-1585747860715-2ba37e788b70?auto=format&fit=crop&w=1350&q=80');
            background-size: cover; background-position: center;
            height: 60vh;
            display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center;
            padding: 20px;
        }
        .cover h1 { font-size: 2.8em; color: var(--gold); margin: 0; text-transform: uppercase; letter-spacing: 2px; }
        .cover p { font-size: 1.1em; color: #bbb; max-width: 450px; margin: 10px 0 25px 0; }
        .cover button { 
            padding: 12px 35px; border: 2px solid var(--gold); background: transparent; 
            color: var(--gold); font-size: 16px; border-radius: 30px; cursor: pointer; 
            transition: 0.3s; font-weight: bold; text-transform: uppercase;
        }
        .cover button:hover { background: var(--gold); color: #000; }

        /* CONTAINER COMPACTO */
        .container { max-width: 700px; margin: auto; padding: 20px; }
        
        .section { 
            background: var(--card-bg); padding: 20px; margin-bottom: 20px; 
            border-radius: 12px; border-bottom: 3px solid var(--gold);
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
        }
        
        h2 { color: var(--gold); font-size: 1.4em; display: flex; align-items: center; gap: 10px; margin-top: 0; }

        /* CARDS ODS */
        .ods-flex { display: flex; gap: 10px; margin-top: 15px; }
        .ods-mini-card { 
            background: #252525; padding: 12px; border-radius: 8px; flex: 1; 
            border: 1px solid #333; text-align: center;
        }
        .ods-mini-card strong { color: var(--accent); display: block; margin-bottom: 5px; }
        .ods-mini-card p { font-size: 0.85em; margin: 0; color: #aaa; }

        /* LISTA ESTILIZADA */
        ul, ol { padding-left: 20px; margin: 15px 0; }
        li { margin-bottom: 8px; color: #ddd; }

        .alert-box { 
            background: rgba(212, 175, 55, 0.1); border: 1px solid var(--gold); 
            padding: 15px; border-radius: 8px; color: #e0ca86; margin: 15px 0;
            display: flex; align-items: center; gap: 10px;
        }

        .img-container { text-align: center; margin: 15px 0; background: white; border-radius: 8px; padding: 10px; }
        .img-container img { max-width: 150px; height: auto; }

        /* QR CODE AREA */
        .qr-area { 
            text-align: center; background: #252525; padding: 15px; 
            border-radius: 10px; margin-top: 10px; 
        }
        canvas { background: white; padding: 8px; border-radius: 4px; }

        /* FOOTER ACADÊMICO */
        .footer-edu { 
            font-size: 0.8em; color: #666; text-align: center; 
            padding: 30px 20px; border-top: 1px solid #222; 
        }
        .footer-edu strong { color: #999; }

        .btn-action { 
            background: var(--gold); color: #000; padding: 12px; border: none; 
            border-radius: 8px; width: 100%; font-weight: bold; cursor: pointer;
            margin-top: 10px; transition: 0.3s;
        }
        .btn-action:hover { background: var(--dark-gold); }

    </style>
</head>
<body>

<div class="cover">
    <h1>💈 CORTE SEGURO</h1>
    <p>O guia de biossegurança feito exclusivamente para o barbeiro profissional.</p>
    <button onclick="document.getElementById('guia').scrollIntoView({behavior:'smooth'})">Começar Guia</button>
</div>

<div class="container" id="guia">
    
    <div class="section">
        <h2>🌍 Compromisso Global</h2>
        <p style="font-size: 0.9em; color: #aaa;">Sua barbearia alinhada com as metas da ONU para um mundo melhor:</p>
        <div class="ods-flex">
            <div class="ods-mini-card">
                <strong>ODS 3</strong>
                <p>Saúde da equipe e clientes.</p>
            </div>
            <div class="ods-mini-card">
                <strong>ODS 12</strong>
                <p>Descarte consciente.</p>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>🛡️ Proteja seu Negócio</h2>
        <p>O descarte correto evita contaminações por <strong>HIV e Hepatites</strong> e mantém você livre de multas da Vigilância Sanitária.</p>
        <div class="alert-box">
            <span>💡</span>
            <span>Resíduos de lâminas nunca devem ir para o lixo comum ou garrafas PET.</span>
        </div>
    </div>

    <div class="section">
        <h2>🟡 Passo a Passo do Descarte</h2>
        <div class="img-container">
            <img src="https://acdn-us.mitiendanube.com/stores/004/929/349/products/coletor-perfurocortante-descarpack_1-a6828377b3743b3a5017379272606102-1024-1024.webp" alt="Coletor">
        </div>
        <ol>
            <li>Use apenas o <strong>Coletor Rígido Amarelo</strong>.</li>
            <li>Não encha mais que <strong>80%</strong> da caixa.</li>
            <li>Lacre a caixa e não tente abrir novamente.</li>
            <li>Entregue na <strong>UBS</strong> mais próxima de você.</li>
        </ol>
    </div>

    <div class="section">
        <h2>📲 Vídeo Explicativo</h2>
        <p style="text-align: center; font-size: 0.9em; margin-bottom: 10px;">Aponte a câmera para o código abaixo:</p>
        <div class="qr-area">
            <canvas id="qrcode"></canvas>
        </div>
        <button class="btn-action" onclick="window.print()">Salvar Guia em PDF</button>
    </div>

</div>

<div class="footer-edu">
    <p><strong>Referencial Acadêmico:</strong> RDC 222/2018 ANVISA | Lei 12.305/10 PNRS</p>
    <p>Projeto de Extensão Universitária - Unyleya</p>
</div>

<script src="https://cdn.jsdelivr.net/npm/qrcode/build/qrcode.min.js"></script>
<script>
    window.onload = function() {
        const canvas = document.getElementById('qrcode');
        QRCode.toCanvas(canvas, "https://www.youtube.com/watch?v=tIP6VcEseqo", { 
            width: 140,
            margin: 2,
            color: { dark: "#000000", light: "#ffffff" }
        });
    }
</script>

</body>
</html>
