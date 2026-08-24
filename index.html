<!DOCTYPE html>  
<html lang="cs">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">  
    <title>BUFET KALKULAČKA</title>  
    <style>  
        * {  
            box-sizing: border-box;  
            margin: 0;  
            padding: 0;  
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;  
            text-transform: uppercase;  
            -webkit-tap-highlight-color: transparent;  
        }  
  
        body {  
            background-color: #000000;  
            color: #FFFFFF;  
            display: flex;  
            flex-direction: column;  
            min-height: 100vh;  
            padding: 15px;  
            user-select: none;  
        }  
  
        .header {  
            text-align: center;  
            font-size: 20px;  
            font-weight: bold;  
            color: #8E8E93;  
            margin-bottom: 10px;  
        }  
  
        /* Zobrazení cen */  
        .display-box {  
            background-color: #1C1C1E;  
            border-radius: 12px;  
            padding: 15px;  
            margin-bottom: 15px;  
            border: 1px solid #3A3A3C;  
        }  
  
        .label {  
            font-size: 16px;  
            color: #8E8E93;  
            font-weight: bold;  
        }  
  
        .amount {  
            font-size: 48px;  
            font-weight: 900;  
            text-align: right;  
            color: #FFFFFF;  
            line-height: 1.1;  
        }  
  
        .sub-info {  
            display: flex;  
            justify-content: space-between;  
            align-items: center;  
            margin-top: 8px;  
            padding-top: 8px;  
            border-top: 1px solid #2C2C2E;  
            font-size: 18px;  
            font-weight: bold;  
        }  
  
        .sub-info .val {  
            color: #FFD60A;  
        }  
  
        .return-box {  
            background-color: #1C1C1E;  
            border-radius: 12px;  
            padding: 15px;  
            margin-bottom: 15px;  
            border: 2px solid #8E8E93;  
            display: none;  
        }  
  
        .return-box.active {  
            display: block;  
        }  
  
        .return-amount {  
            font-size: 42px;  
            font-weight: 900;  
            text-align: right;  
            color: #30D158;  
        }  
  
        .alert-text {  
            color: #FF453A !important;  
            font-size: 22px;  
            text-align: center;  
            margin-top: 5px;  
        }  
  
        /* Navigace režimů */  
        .mode-container {  
            display: flex;  
            gap: 10px;  
            margin-bottom: 15px;  
        }  
  
        .btn-mode {  
            flex: 1;  
            background-color: #0A84FF;  
            color: #FFFFFF;  
            border: none;  
            padding: 18px 5px;  
            font-size: 18px;  
            font-weight: bold;  
            border-radius: 12px;  
            cursor: pointer;  
            opacity: 0.4;  
        }  
  
        .btn-mode.active {  
            opacity: 1;  
            border: 3px solid #FFFFFF;  
        }  
  
        /* Hlavní tlačítko poslouchání */  
        .btn-listen {  
            width: 100%;  
            padding: 25px 10px;  
            font-size: 26px;  
            font-weight: 900;  
            border: none;  
            border-radius: 16px;  
            margin-bottom: 15px;  
            cursor: pointer;  
            color: #FFFFFF;  
            background-color: #FF3B30; /* Červená default */  
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);  
        }  
  
        .btn-listen.listening {  
            background-color: #30D158; /* Zelená při poslouchání */  
            animation: pulse 1.5s infinite;  
        }  
  
        @keyframes pulse {  
            0% { opacity: 1; }  
            50% { opacity: 0.7; }  
            100% { opacity: 1; }  
        }  
  
        /* Ovládací tlačítka dole */  
        .action-container {  
            display: flex;  
            gap: 10px;  
            margin-top: auto;  
            margin-bottom: 10px;  
        }  
  
        .btn-action {  
            flex: 1;  
            background-color: #3A3A3C;  
            color: #FFFFFF;  
            border: none;  
            padding: 18px 5px;  
            font-size: 16px;  
            font-weight: bold;  
            border-radius: 12px;  
            cursor: pointer;  
        }  
  
        .btn-new {  
            background-color: #FF9F0A;  
            color: #000000;  
        }  
  
        /* Sekce historie */  
        .history-panel {  
            background-color: #1C1C1E;  
            border-radius: 12px;  
            padding: 15px;  
            margin-top: 10px;  
            display: none;  
            max-height: 250px;  
            overflow-y: auto;  
        }  
  
        .history-panel.active {  
            display: block;  
        }  
  
        .history-item {  
            display: flex;  
            justify-content: space-between;  
            padding: 8px 0;  
            border-bottom: 1px solid #2C2C2E;  
            font-size: 14px;  
        }  
  
        .history-header {  
            display: flex;  
            justify-content: space-between;  
            align-items: center;  
            margin-bottom: 10px;  
        }  
  
        .btn-clear {  
            background-color: #FF453A;  
            color: #FFFFFF;  
            border: none;  
            padding: 5px 10px;  
            border-radius: 6px;  
            font-size: 12px;  
            font-weight: bold;  
        }  
    </style>  
</head>  
<body>  
  
    <div class="header">BUFET KALKULAČKA</div>  
  
    <!-- Zobrazení celkové ceny a posledního slova -->  
    <div class="display-box">  
        <div class="label" id="mainLabel">CELKOVÁ CENA</div>  
        <div class="amount" id="totalDisplay">0 KČ</div>  
        <div class="sub-info">  
            <span>POSLEDNÍ:</span>  
            <span class="val" id="lastWordDisplay">---</span>  
        </div>  
    </div>  
  
    <!-- Zobrazení pro vrácení v režimu PŘIJATO -->  
    <div class="return-box" id="returnBox">  
        <div class="sub-info" style="border:none; padding:0; margin-bottom: 5px;">  
            <span class="label">PŘIJATO:</span>  
            <span class="val" id="receivedDisplay" style="color:#FFF;">0 KČ</span>  
        </div>  
        <div class="label">VRÁTIT</div>  
        <div class="return-amount" id="returnDisplay">0 KČ</div>  
        <div class="alert-text" id="alertText" style="display:none;">NESTAČÍ!</div>  
    </div>  
  
    <!-- Výběr režimu -->  
    <div class="mode-container">  
        <button class="btn-mode active" id="btnModeCalc" onclick="setMode('CALC')">KALKULAČKA</button>  
        <button class="btn-mode" id="btnModeRec" onclick="setMode('REC')">PŘIJATO</button>  
    </div>  
  
    <!-- Hlavní tlačítko mikrofonu -->  
    <button class="btn-listen" id="btnListen" onclick="toggleListening()">  
        POSLOUCHÁNÍ VYPNUTO  
    </button>  
  
    <!-- Spodní akce -->  
    <div class="action-container">  
        <button class="btn-action btn-new" onclick="startNewCustomer()">NOVÝ ZÁKAZNÍK</button>  
        <button class="btn-action" onclick="toggleHistory()">HISTORIE</button>  
    </div>  
  
    <!-- Panel historie -->  
    <div class="history-panel" id="historyPanel">  
        <div class="history-header">  
            <span class="label">HISTORIE PRODEJŮ</span>  
            <button class="btn-clear" onclick="clearHistory()">SMAZAT</button>  
        </div>  
        <div id="historyList"></div>  
    </div>  
  
    <script>  
        // Stav aplikace  
        let currentMode = 'CALC'; // 'CALC' nebo 'REC'  
        let isListening = false;  
        let totalAmount = 0;  
        let receivedAmount = 0;  
        let historyData = JSON.parse(localStorage.getItem('bufet_history') || '[]');  
  
        // Rozpoznávání řeči (Web Speech API)  
        const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;  
        let recognition = null;  
  
        if (SpeechRecognition) {  
            recognition = new SpeechRecognition();  
            recognition.lang = 'cs-CZ';  
            recognition.continuous = true;  
            recognition.interimResults = false;  
  
            recognition.onresult = function(event) {  
                if (!isListening) return;  
  
                const lastResultIndex = event.results.length - 1;  
                const transcript = event.results[lastResultIndex][0].transcript.trim().toLowerCase();  
                  
                processVoiceInput(transcript);  
            };  
  
            recognition.onerror = function(event) {  
                console.log('Chyba rozpoznávání:', event.error);  
                if (isListening && event.error !== 'no-speech') {  
                    // Automatické obnovení při neaktivitě  
                    try { recognition.start(); } catch(e){}  
                }  
            };  
  
            recognition.onend = function() {  
                // Pokud má poslouchání běžet, restarujeme ho (iOS ukončuje rozpoznávání při tichu)  
                if (isListening) {  
                    try { recognition.start(); } catch(e){}  
                }  
            };  
        } else {  
            alert('VÁŠ PROHLÍŽEČ NEPODPORUJE HLASOVÉ ROZPOZNÁVÁNÍ. POUŽIJTE SAFARI NA IPHONE.');  
        }  
  
        // Převodník českých číslovek na čísla  
        function parseCzechNumber(text) {  
            // Vyčistíme text od teček a čárek  
            text = text.replace(/[.,]/g, '').trim();  
  
            // 1. Pokud je vstup rovnou číslo napsané číslicemi  
            const directNum = parseInt(text, 10);  
            if (!isNaN(directNum) && text === directNum.toString()) {  
                return directNum;  
            }  
  
            // Sladač slova na číslice  
            const words = text.split(/\s+/);  
            let total = 0;  
            let current = 0;  
  
            const units = {  
                'nula':0, 'jeden':1, 'jedna':1, 'jedno':1, 'dva':2, 'dvě':2, 'tři':3, 'čtyři':4, 'pět':5,  
                'šest':6, 'sedm':7, 'osm':8, 'devět':9, 'deset':10, 'jedenáct':11, 'dvanáct':12,  
                'trináct':13, 'třináct':13, 'čtrnáct':14, 'patnáct':15, 'šestnáct':16, 'sedmnáct':17,  
                'osmnáct':18, 'devatenáct':19  
            };  
  
            const tens = {  
                'dvacat':20, 'dvacet':20, 'třicet':30, 'čtyřicet':40, 'padesát':50,  
                'šedesát':60, 'sedmdesát':70, 'osmdesát':80, 'devadesát':90  
            };  
  
            const hundreds = {  
                'sto':100, 'stě':200, 'šta':200, 'stovka':100, 'stovky':200, 'sta':300,  
                'stoky':100, 'stěmi':200, 'stům':100  
            };  
  
            for (let word of words) {  
                let num = null;  
  
                if (units[word] !== undefined) num = units[word];  
                else if (tens[word] !== undefined) num = tens[word];  
                else if (word.includes('st')) {  
                    if (word === 'sto') num = 100;  
                    else if (word === 'dvěstě' || word === 'dvěstě') num = 200;  
                    else if (word === 'třisto') num = 300;  
                    else if (word === 'čtyřisto') num = 400;  
                    else if (word === 'pětset') num = 500;  
                    else if (word === 'šestset') num = 600;  
                    else if (word === 'sedmset') num = 700;  
                    else if (word === 'osmset') num = 800;  
                    else if (word === 'devětset') num = 900;  
                } else if (word === 'tisíc' || word === 'tisice' || word === 'tisíce') {  
                    total += (current === 0 ? 1 : current) * 1000;  
                    current = 0;  
                    continue;  
                }  
  
                // Pokud slovo obsahuje např. "200" nebo samostatné číslo přímo uvnitř textu  
                if (num === null) {  
                    const parsed = parseInt(word, 10);  
                    if (!isNaN(parsed)) num = parsed;  
                }  
  
                if (num !== null) {  
                    if (num === 100 && current > 0 && current < 10) {  
                        current = current * 100;  
                    } else {  
                        current += num;  
                    }  
                }  
            }  
  
            total += current;  
            return total > 0 ? total : null;  
        }  
  
        // Zpracování rozpoznaného hlasu  
        function processVoiceInput(transcript) {  
            document.getElementById('lastWordDisplay').innerText = transcript;  
  
            const value = parseCzechNumber(transcript);  
  
            if (value !== null && value > 0) {  
                if (currentMode === 'CALC') {  
                    totalAmount += value;  
                    updateUI();  
                } else if (currentMode === 'REC') {  
                    receivedAmount = value;  
                    updateUI();  
                }  
            }  
        }  
  
        // Přepínání poslouchání ZAP/VYP  
        function toggleListening() {  
            if (!recognition) return;  
  
            isListening = !isListening;  
            const btn = document.getElementById('btnListen');  
  
            if (isListening) {  
                btn.innerText = "POSLOUCHÁM...";  
                btn.classList.add('listening');  
                try {  
                    recognition.start();  
                } catch (e) {  
                    console.log("Start error:", e);  
                }  
            } else {  
                btn.innerText = "POSLOUCHÁNÍ VYPNUTO";  
                btn.classList.remove('listening');  
                try {  
                    recognition.stop();  
                } catch (e) {  
                    console.log("Stop error:", e);  
                }  
            }  
        }  
  
        // Přepínání režimů (KALKULAČKA / PŘIJATO)  
        function setMode(mode) {  
            currentMode = mode;  
            document.getElementById('btnModeCalc').classList.toggle('active', mode === 'CALC');  
            document.getElementById('btnModeRec').classList.toggle('active', mode === 'REC');  
            document.getElementById('returnBox').classList.toggle('active', mode === 'REC');  
  
            if (mode === 'REC') {  
                document.getElementById('mainLabel').innerText = "CELKOVÁ CENA (K ÚHRADĚ)";  
            } else {  
                document.getElementById('mainLabel').innerText = "CELKOVÁ CENA";  
            }  
  
            updateUI();  
        }  
  
        // Aktualizace uživatelského rozhraní  
        function updateUI() {  
            document.getElementById('totalDisplay').innerText = totalAmount + " KČ";  
            document.getElementById('receivedDisplay').innerText = receivedAmount + " KČ";  
  
            if (currentMode === 'REC') {  
                const returnVal = receivedAmount - totalAmount;  
                const returnDisplay = document.getElementById('returnDisplay');  
                const alertText = document.getElementById('alertText');  
  
                if (receivedAmount === 0) {  
                    returnDisplay.innerText = "0 KČ";  
                    returnDisplay.style.color = "#30D158";  
                    alertText.style.display = "none";  
                } else if (returnVal < 0) {  
                    returnDisplay.innerText = "0 KČ";  
                    alertText.style.display = "block";  
                } else {  
                    returnDisplay.innerText = returnVal + " KČ";  
                    returnDisplay.style.color = "#30D158";  
                    alertText.style.display = "none";  
                }  
            }  
        }  
  
        // Nový zákazník (vynulování + uložení do historie)  
        function startNewCustomer() {  
            if (totalAmount > 0) {  
                saveToHistory();  
            }  
  
            totalAmount = 0;  
            receivedAmount = 0;  
            document.getElementById('lastWordDisplay').innerText = "---";  
            setMode('CALC');  
            updateUI();  
        }  
  
        // Uložení do LocalStorage  
        function saveToHistory() {  
            const returnVal = receivedAmount >= totalAmount ? (receivedAmount - totalAmount) : 0;  
            const item = {  
                time: new Date().toLocaleTimeString([], {hour: '2-digit', minute:'2-digit'}),  
                total: totalAmount,  
                received: receivedAmount,  
                returned: returnVal  
            };  
  
            historyData.unshift(item);  
            if (historyData.length > 50) historyData.pop(); // Max 50 záznamů  
            localStorage.setItem('bufet_history', JSON.stringify(historyData));  
            renderHistory();  
        }  
  
        // Vykreslení historie  
        function renderHistory() {  
            const list = document.getElementById('historyList');  
            list.innerHTML = '';  
  
            if (historyData.length === 0) {  
                list.innerHTML = '<div style="color:#8E8E93; text-align:center; padding:10px;">ŽÁDNÁ HISTORIE</div>';  
                return;  
            }  
  
            historyData.forEach(item => {  
                const div = document.createElement('div');  
                div.className = 'history-item';  
                div.innerHTML = `  
                    <span>${item.time} - CENA: <b>${item.total} KČ</b></span>  
                    <span>PŘIJATO: ${item.received} | VRÁTÍT: <b>${item.returned} KČ</b></span>  
                `;  
                list.appendChild(div);  
            });  
        }  
  
        function toggleHistory() {  
            const panel = document.getElementById('historyPanel');  
            panel.classList.toggle('active');  
            if (panel.classList.contains('active')) {  
                renderHistory();  
            }  
        }  
  
        function clearHistory() {  
            historyData = [];  
            localStorage.removeItem('bufet_history');  
            renderHistory();  
        }  
  
        // Inicializace  
        updateUI();  
    </script>  
</body>  
</html>  
