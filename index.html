<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>咪咪的每日用藥紀錄表</title>
    <style>
        :root {
            --primary-color: #ff9999;
            --secondary-color: #ffe6e6;
            --success-color: #a8e6cf;
            --text-color: #4a4a4a;
        }

        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            background-color: #fffaf0;
            color: var(--text-color);
            margin: 0;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .container {
            max-width: 600px;
            width: 100%;
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        h1 {
            text-align: center;
            color: #ff6b6b;
            margin-bottom: 5px;
        }

        .date-display {
            text-align: center;
            font-size: 1.1rem;
            color: #888;
            margin-bottom: 25px;
        }

        .med-card {
            background: var(--secondary-color);
            border-left: 5px solid var(--primary-color);
            padding: 15px;
            margin-bottom: 15px;
            border-radius: 0 10px 10px 0;
        }

        .med-title {
            font-size: 1.1rem;
            font-weight: bold;
            color: #d15b5b;
            margin-bottom: 10px;
        }

        .time-slots {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .slot {
            flex: 1;
            min-width: 120px;
            background: white;
            border: 2px solid var(--primary-color);
            padding: 10px;
            border-radius: 8px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: space-between;
            gap: 8px;
            transition: all 0.3s;
        }

        .slot.taken {
            background-color: var(--success-color);
            border-color: #81c784;
            opacity: 0.7;
        }

        .slot-time {
            font-size: 0.9rem;
            font-weight: bold;
        }

        .med-btn {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 6px 12px;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            width: 100%;
            transition: background 0.2s;
        }

        .med-btn:hover {
            background-color: #ff6b6b;
        }

        .slot.taken .med-btn {
            background-color: #81c784;
            cursor: default;
        }

        .reset-container {
            text-align: center;
            margin-top: 25px;
        }

        .reset-btn {
            background-color: #4a4a4a;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 1rem;
            border-radius: 20px;
            cursor: pointer;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }

        .reset-btn:hover {
            background-color: #333;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>🐱 咪咪的每日用藥紀錄表</h1>
    <div class="date-display" id="currentDate">今日日期：</div>

    <div class="med-card">
        <div class="med-title">1. 癲癇藥 + 鉀離子 + 維他命 (早晚各1顆)</div>
        <div class="time-slots">
            <div class="slot" id="med1-morning">
                <span class="slot-time">早上 ☀️</span>
                <button class="med-btn" onclick="toggleMed('med1-morning')">吃藥了</button>
            </div>
            <div class="slot" id="med1-night">
                <span class="slot-time">晚上 🌙</span>
                <button class="med-btn" onclick="toggleMed('med1-night')">吃藥了</button>
            </div>
        </div>
    </div>

    <div class="med-card">
        <div class="med-title">2. 癲癇藥 + 腸胃蠕動 (每8小時1顆)</div>
        <div class="time-slots">
            <div class="slot" id="med2-07">
                <span class="slot-time">早上 07:00 ⏰</span>
                <button class="med-btn" onclick="toggleMed('med2-07')">吃藥了</button>
            </div>
            <div class="slot" id="med2-15">
                <span class="slot-time">下午 15:00 ⏰</span>
                <button class="med-btn" onclick="toggleMed('med2-15')">吃藥了</button>
            </div>
            <div class="slot" id="med2-23">
                <span class="slot-time">晚上 23:00 ⏰</span>
                <button class="med-btn" onclick="toggleMed('med2-23')">吃藥了</button>
            </div>
        </div>
    </div>

    <div class="med-card">
        <div class="med-title">3. 高血壓藥 (晚上1顆)</div>
        <div class="time-slots">
            <div class="slot" id="med3-night">
                <span class="slot-time">晚上 🌙</span>
                <button class="med-btn" onclick="toggleMed('med3-night')">吃藥了</button>
            </div>
        </div>
    </div>

    <div class="med-card">
        <div class="med-title">4. 中藥 (早晚各1包 / 每包2顆)</div>
        <div class="time-slots">
            <div class="slot" id="med4-morning">
                <span class="slot-time">早上 ☀️</span>
                <button class="med-btn" onclick="toggleMed('med4-morning')">吃藥了</button>
            </div>
            <div class="slot" id="med4-night">
                <span class="slot-time">晚上 🌙</span>
                <button class="med-btn" onclick="toggleMed('med4-night')">吃藥了</button>
            </div>
        </div>
    </div>

    <div class="reset-container">
        <button class="reset-btn" onclick="resetAll()">☀️ 開啟新的一天 (重設紀錄)</button>
    </div>
</div>

<script>
    // 顯示今日日期
    const today = new Date();
    document.getElementById('currentDate').innerText = `今日日期：${today.getFullYear()} 年 ${today.getMonth() + 1} 月 ${today.getDate()} 日`;

    // 網頁載入時，從瀏覽器暫存(LocalStorage)讀取紀錄
    window.onload = function() {
        const savedState = JSON.parse(localStorage.getItem('mimiMedRecords')) || {};
        for (const id in savedState) {
            if (savedState[id]) {
                setSlotAsTaken(id);
            }
        }
    };

    // 切換吃藥狀態
    function toggleMed(slotId) {
        const slot = document.getElementById(slotId);
        // 如果已經吃過了就不重複觸發
        if (slot.classList.contains('taken')) return;

        setSlotAsTaken(slotId);
        saveState();
    }

    // 將時段改為「已服用」樣式
    function setSlotAsTaken(slotId) {
        const slot = document.getElementById(slotId);
        if (slot) {
            slot.classList.add('taken');
            const btn = slot.querySelector('.med-btn');
            btn.innerText = '✓ 已吃藥';
        }
    }

    // 儲存狀態到瀏覽器暫存
    function saveState() {
        const slots = document.querySelectorAll('.slot');
        const state = {};
        slots.forEach(slot => {
            state[slot.id] = slot.classList.contains('taken');
        });
        localStorage.setItem('mimiMedRecords', JSON.stringify(state));
    }

    // 重置所有紀錄
    function resetAll() {
        if (confirm('確定要清除今天的紀錄，開啟新的一天嗎？')) {
            const slots = document.querySelectorAll('.slot');
            slots.forEach(slot => {
                slot.classList.remove('taken');
                const btn = slot.querySelector('.med-btn');
                btn.innerText = '吃藥了';
            });
            localStorage.removeItem('mimiMedRecords');
        }
    }
</script>

</body>
</html>
