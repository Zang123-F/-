#-
浪漫
<!DOCTYPE html>
<html>
<head>
    <title>给最爱的你 ❤️</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            background: #ffe6f2; /* 浅粉色背景 */
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            font-family: 'Microsoft YaHei', cursive;
        }
        .container {
            text-align: center;
            padding: 20px;
            animation: fadeIn 2s;
        }
        h1 {
            color: #ff69b4; /* 粉红色标题 */
            font-size: 2.5em;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }
        .love-note {
            color: #ff1493; /* 深粉色文字 */
            font-size: 1.8em;
            margin: 30px;
            line-height: 1.6;
        }
        .heart {
            color: #ff69b4;
            font-size: 3em;
            animation: pulse 1.5s infinite;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>❤️ 情人节快乐！我的爱人 ❤️</h1>
        <div class="love-note" id="message">正在加载爱的告白...</div>
        <div class="heart">♥</div>
    </div>

    <script>
        // 随机情话库（可以自行添加修改）
        const loveMessages = [
            "遇见你，是我今生最美的意外",
            "你的笑容是我每天最期待的风景",
            "我想把全世界的温柔都藏起来，留给你",
            "星河滚烫，你是人间理想",
            "与你共度的每个朝夕，都是情人节",
            "心跳多久，爱你就有多久",
            "你是我平凡生活里的耀眼星辰",
            "细水长流是你，柴米油盐是你，白首也是你"
        ];

        // 随机显示情话
        function showRandomMessage() {
            const randomIndex = Math.floor(Math.random() * loveMessages.length);
            document.getElementById('message').textContent = loveMessages[randomIndex];
            
            // 添加浮动效果
            document.getElementById('message').style.animation = 'float 3s ease-in-out';
        }

        // 初始化
        window.onload = function() {
            showRandomMessage();
            setInterval(showRandomMessage, 5000); // 每5秒自动切换
        }
    </script>
</body>
</html>
