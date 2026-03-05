<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I Love You</title>
    <style>
        body {
            margin: 0;
            overflow: hidden;
            background: #0a0a0a;
            font-family: Arial, sans-serif;
        }

        #container {
            position: relative;
            width: 100vw;
            height: 100vh;
        }

        .heart {
            position: absolute;
            left: 0;
            top: 0;
            color: #ff2d55;
            font-size: 14px;
            user-select: none;
            pointer-events: none;
            /* Dùng transition cho transform sẽ cực kỳ mượt */
            transition: transform 2.5s cubic-bezier(0.175, 0.885, 0.32, 1.275), opacity 1.5s;
            will-change: transform; /* Báo trước cho trình duyệt tối ưu GPU */
        }

        #startBtn {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            padding: 15px 40px;
            font-size: 18px;
            background: #ff2d55;
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            z-index: 100;
            box-shadow: 0 0 20px rgba(255, 45, 85, 0.6);
        }

        /* Hiệu ứng hào quang cho chữ */
        .glow {
            text-shadow: 0 0 10px #ff2d55, 0 0 20px #ff2d55;
            font-size: 18px !important;
        }
    </style>
</head>
<body>

    <button id="startBtn">Bấm vào đây đi!</button>
    <div id="container"></div>

    <script>
        const container = document.getElementById('container');
        const startBtn = document.getElementById('startBtn');
        const count = 700; // Tăng số lượng hạt lên để chữ dày hơn
        const hearts = [];

        // Bảng mã chữ I LOVE YOU (Dày hơn)
        // Dùng hệ tọa độ (x, y) để vẽ
        const points = [];
        const pattern = [
            "  I      L      OOO    V   V  EEEEE     Y   Y   OOO   U   U",
            "  I      L     O   O   V   V  E          Y Y   O   O  U   U",
            "  I      L     O   O   V   V  EEEE        Y    O   O  U   U",
            "  I      L     O   O    V V   E           Y    O   O  U   U",
            "  I      LLLLL  OOO      V    EEEEE       Y     OOO    UUU "
        ];

        // Tạo hạt tim ban đầu (bay hỗn loạn như gió)
        function init() {
            for (let i = 0; i < count; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.innerHTML = '❤';
                
                // Vị trí ngẫu nhiên ngoài màn hình
                const startX = Math.random() * window.innerWidth;
                const startY = Math.random() * window.innerHeight;
                
                heart.style.transform = `translate(${startX}px, ${startY}px) scale(0)`;
                heart.style.opacity = '0';
                
                container.appendChild(heart);
                hearts.push({
                    el: heart,
                    x: startX,
                    y: startY
                });
            }
        }

        function createLetterPoints() {
            const spacing = 15; // Khoảng cách giữa các hạt (nhỏ hơn = dày hơn)
            const offsetX = window.innerWidth / 2 - (pattern[0].length * spacing) / 2;
            const offsetY = window.innerHeight / 2 - (pattern.length * spacing) / 2;

            for (let y = 0; y < pattern.length; y++) {
                for (let x = 0; x < pattern[y].length; x++) {
                    if (pattern[y][x] !== " ") {
                        // Với mỗi điểm trong pattern, tạo 2 hạt đè lên nhau để chữ dày hơn
                        points.push({ x: x * spacing + offsetX, y: y * spacing + offsetY });
                        points.push({ x: x * spacing + offsetX + 3, y: y * spacing + offsetY + 3 });
                    }
                }
            }
        }

        startBtn.addEventListener('click', () => {
            startBtn.style.display = 'none';
            createLetterPoints();
            
            // Giai đoạn 1: Cơn gió thổi tung
            hearts.forEach((h, i) => {
                setTimeout(() => {
                    const windX = Math.random() * window.innerWidth;
                    const windY = Math.random() * window.innerHeight;
                    h.el.style.opacity = '0.8';
                    h.el.style.transform = `translate(${windX}px, ${windY}px) scale(${Math.random() * 1 + 0.5}) rotate(${Math.random() * 360}deg)`;
                }, i * 2);
            });

            // Giai đoạn 2: Gom thành chữ (Sau 1.5 giây)
            setTimeout(() => {
                hearts.forEach((h, i) => {
                    if (i < points.length) {
                        const target = points[i];
                        h.el.style.transform = `translate(${target.x}px, ${target.y}px) scale(1.2) rotate(0deg)`;
                        h.el.classList.add('glow');
                        h.el.style.opacity = '1';
                    } else {
                        // Những hạt thừa thì bay tản ra xung quanh tạo hiệu ứng lấp lánh
                        const outX = Math.random() * window.innerWidth;
                        const outY = Math.random() * window.innerHeight;
                        h.el.style.opacity = '0.2';
                        h.el.style.transform = `translate(${outX}px, ${outY}px) scale(0.5)`;
                    }
                });
            }, 2000);
        });

        init();
    </script>
</body>
</html>
