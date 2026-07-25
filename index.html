<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GamePay — Донат и Игровая Валюта</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #12131C;
            color: #FFFFFF;
            padding-bottom: 50px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #1f2130, #161722);
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 2px solid #2D3047;
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
            color: #00E676;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .admin-btn {
            background: #2D3047;
            color: #AAA;
            border: 1px solid #444968;
            padding: 6px 12px;
            border-radius: 6px;
            font-size: 13px;
            cursor: pointer;
            transition: 0.2s;
        }

        .admin-btn:hover {
            background: #3B3E5C;
            color: #FFF;
        }

        .container {
            max-width: 600px;
            margin: 20px auto;
            padding: 0 15px;
        }

        /* Card Styles */
        .card {
            background: #1C1E2D;
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 20px;
            border: 1px solid #2B2E45;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }

        .card h2 {
            font-size: 18px;
            margin-bottom: 15px;
            color: #00E676;
        }

        .form-group {
            margin-bottom: 15px;
        }

        label {
            display: block;
            font-size: 13px;
            color: #AAA;
            margin-bottom: 6px;
        }

        input[type="text"], input[type="number"], select {
            width: 100%;
            padding: 12px;
            background: #12131C;
            border: 1px solid #333752;
            border-radius: 8px;
            color: #FFF;
            font-size: 15px;
            outline: none;
            transition: 0.2s;
        }

        input:focus {
            border-color: #00E676;
        }

        /* Calculation Info Box */
        .calc-info {
            background: #161722;
            border-radius: 8px;
            padding: 12px;
            margin-top: 15px;
            border-left: 3px solid #00E676;
        }

        .calc-row {
            display: flex;
            justify-content: space-between;
            font-size: 14px;
            margin-bottom: 6px;
            color: #CCC;
        }

        .calc-row.total {
            font-size: 18px;
            font-weight: bold;
            color: #FFF;
            border-top: 1px solid #2B2E45;
            padding-top: 8px;
            margin-top: 8px;
        }

        .calc-row.total span:last-child {
            color: #00E676;
        }

        .pay-btn {
            width: 100%;
            padding: 14px;
            background: #00E676;
            color: #000;
            font-weight: bold;
            font-size: 16px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            margin-top: 15px;
            transition: 0.2s;
        }

        .pay-btn:hover {
            background: #00C853;
        }

        /* Modal Admin Panel */
        .modal {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.8);
            justify-content: center;
            align-items: center;
            z-index: 100;
            padding: 15px;
        }

        .modal-content {
            background: #1C1E2D;
            width: 100%;
            max-width: 450px;
            border-radius: 12px;
            padding: 20px;
            border: 1px solid #3B3E5C;
            position: relative;
        }

        .close-btn {
            position: absolute;
            top: 12px;
            right: 15px;
            font-size: 20px;
            color: #AAA;
            cursor: pointer;
        }

        .admin-section {
            background: #12131C;
            padding: 15px;
            border-radius: 8px;
            margin-top: 15px;
            border: 1px solid #2B2E45;
        }

        .save-btn {
            width: 100%;
            padding: 10px;
            background: #2979FF;
            color: white;
            border: none;
            border-radius: 6px;
            font-weight: bold;
            cursor: pointer;
            margin-top: 10px;
        }

        .save-btn:hover {
            background: #1565C0;
        }

        .badge {
            background: rgba(0, 230, 118, 0.15);
            color: #00E676;
            padding: 2px 8px;
            border-radius: 4px;
            font-size: 12px;
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">⚡ GamePay</div>
        <button class="admin-btn" onclick="openAdmin()">⚙️ Админка</button>
    </header>

    <div class="container">
        <!-- Покупка валюты -->
        <div class="card">
            <h2>🛒 Покупка игровой валюты</h2>

            <div class="form-group">
                <label>Выберите игру:</label>
                <select id="gameSelect">
                    <option value="roblox">Roblox (Robux)</option>
                    <option value="brawl">Brawl Stars (Gems)</option>
                    <option value="freefire">Free Fire (Diamonds)</option>
                </select>
            </div>

            <div class="form-group">
                <label>Ваш логин / ID в игре:</label>
                <input type="text" id="playerTag" placeholder="Например: Player#1234">
            </div>

            <div class="form-group">
                <label>Количество игровой валюты:</label>
                <input type="number" id="amountInput" value="1000" min="10" oninput="calculatePrice()">
            </div>

            <!-- Расчет стоимости -->
            <div class="calc-info">
                <div class="calc-row">
                    <span>Базовая цена:</span>
                    <span id="basePrice">0 ₽</span>
                </div>
                <div class="calc-row">
                    <span>Сервисный сбор (<span id="commissionPercentDisplay" class="badge">1%</span>):</span>
                    <span id="commissionAmount">0 ₽</span>
                </div>
                <div class="calc-row total">
                    <span>Итого к оплате:</span>
                    <span id="totalPrice">0 ₽</span>
                </div>
            </div>

            <button class="pay-btn" onclick="processPayment()">Перейти к оплате</button>
        </div>
    </div>

    <!-- Модальное окно Админ-Панели -->
    <div class="modal" id="adminModal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeAdmin()">&times;</span>
            <h2 style="color: #00E676; margin-bottom: 10px;">⚙️ Панель Управления</h2>
            <p style="font-size: 12px; color: #AAA;">Настройки комиссии и профита вашего сайта</p>

            <div class="admin-section">
                <label style="color: #FFF; font-weight: bold;">Процент комиссии сайта (1% - 100%):</label>
                <div style="display: flex; gap: 10px; align-items: center; margin-top: 10px;">
                    <input type="number" id="adminCommissionInput" min="1" max="100" value="1" style="width: 100px;">
                    <span style="font-size: 18px; font-weight: bold;">%</span>
                </div>
                <p style="font-size: 11px; color: #888; margin-top: 6px;">
                    Этот процент будет автоматически прибавляться к стоимости заказа и капать вам в доход.
                </p>
                <button class="save-btn" onclick="saveAdminCommission()">Сохранить процент</button>
            </div>
        </div>
    </div>

    <script>
        // Курс за 1 единицу валюты (в рублях)
        const RATE_PER_UNIT = 1.2; 

        // Получить текущий сохраненный процент комиссии
        function getCommissionRate() {
            let saved = localStorage.getItem('site_commission_rate');
            return saved ? parseFloat(saved) : 1; // По умолчанию 1%
        }

        // Сохранить процент комиссии через админку
        function saveAdminCommission() {
            let input = document.getElementById('adminCommissionInput').value;
            let val = parseFloat(input);

            if (isNaN(val) || val < 1 || val > 100) {
                alert('Пожалуйста, введите значение от 1 до 100!');
                return;
            }

            localStorage.setItem('site_commission_rate', val);
            alert('Успешно! Процент комиссии изменен на ' + val + '%');
            closeAdmin();
            calculatePrice();
        }

        // Перерасчет стоимости на сайте
        function calculatePrice() {
            let amount = parseFloat(document.getElementById('amountInput').value) || 0;
            let commissionPercent = getCommissionRate();

            // Базовая стоимость товара
            let base = amount * RATE_PER_UNIT;
            
            // Расчет комиссии (вашей чистой прибыли)
            let commissionSum = base * (commissionPercent / 100);

            // Итоговая стоимость для покупателя
            let total = base + commissionSum;

            // Обновляем текст на экране
            document.getElementById('basePrice').innerText = base.toFixed(2) + ' ₽';
            document.getElementById('commissionAmount').innerText = commissionSum.toFixed(2) + ' ₽';
            document.getElementById('totalPrice').innerText = total.toFixed(2) + ' ₽';
            document.getElementById('commissionPercentDisplay').innerText = commissionPercent + '%';
        }

        // Переход к оплате
        function processPayment() {
            let tag = document.getElementById('playerTag').value;
            let total = document.getElementById('totalPrice').innerText;

            if (!tag.trim()) {
                alert('Введите ваш логин или ID в игре!');
                return;
            }

            alert('Заказ сформирован! Сумма: ' + total + '\nПеренаправление на страницу оплаты...');
        }

        // Открытие и закрытие Админки
        function openAdmin() {
            document.getElementById('adminCommissionInput').value = getCommissionRate();
            document.getElementById('adminModal').style.display = 'flex';
        }

        function closeAdmin() {
            document.getElementById('adminModal').style.display = 'none';
        }

        // При загрузке страницы
        window.onload = function() {
            calculatePrice();
        };
    </script>
</body>
</html>
