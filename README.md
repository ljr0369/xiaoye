<！doctype html>
<超文本标记语言朗="zh-CN">
<头>
    <元字符集="UTF-8">
    <元姓名="视口" 内容="宽度=设备宽度，初始比例=1.0">
    <标题>小叶同学的新年惊喜</标题>
    <风格>
身体{
            边缘:0;
            溢出:隐藏的;
            背景:线性梯度(#ff3366，#ff6b6b);
            字体系列:'微软亚黑',无衬线;
        }

    /* 霓虹灯文字 */
    .neon-text{
    文本对齐：居中；
    颜色：#fff；
    字体大小：2.5em；
    动画：发光2s轻松进出无限；
    margin-top:20px；
    }

    @keyframes glow{
    0%，100%{text-shadow:0010px#fff，0020px#ff00de；}
    50%{text-shadow:0020px#ffd700，0030px#ff0000；}
    }

    /* 红包动画 */
    .red-envelope{
    位置：绝对；
    左侧：50%；
    top:40%；
    变换：translateX(-50%)；
    宽度：200px；
    光标：指针；
    过渡：变换0.5s；
    }

    .money{
    位置：绝对；
    左侧：50%；
    top:40%；
    宽度：150px；
    不透明度：0；
    转换：全部为1；
    }

    .red-Envelope：活动+.money{
    不透明度：1；
    变换：平移(-50%，-100px)旋转(15度)；
    }

    /* 雪花和花瓣 */
    .雪，.花瓣{
    位置：绝对；
    宽度：10px；
    高度：10px；
    背景：白色；
    边界半径：50%；
    动画：下降线性无限；
    }

    .petal{background：#ff99cc；}

    @keyframes fall{
    to{transform:translateY(100vh)旋转(360度)；}
    }
    </style>
</头>
<身体>
    <H1班级="neon-text">🐍 小叶同学，2025新年快乐！</H1>
    
    <img src="https://cdn-icons-png.flaticon.com/512/1046/1046784.png"
    class="红包"
    alt="红包"
    onClick="PlayMusic()">

    <img src="https://cdn-icons-png.flaticon.com/512/5890/5890089.png" 
         class="money" 
         alt="200元">

    <audio id="bgm" src="https://cdn.jsdelivr.net/gh/yourusername/haoyunlai.mp3"></audio>

    <script>
        // 生成雪花和花瓣
        function createParticles() {
            for (let i = 0; i < 50; i++) {
                const particle = document.createElement('div');
                particle.className = Math.random() > 0.5 ? 'snow' : 'petal';
                particle.style.left = Math.random() * 100 + 'vw';
                particle.style.animationDuration = Math.random() * 3 + 2 + 's';
                document.body.appendChild(particle);
            }
        }

        // 点击播放音乐
        function playMusic() {
            const audio = document.getElementById('bgm');
            audio.play();
            audio.loop = true;
        }

        window.onload = createParticles;
    </script>
</body>
</超文本标记语言>
