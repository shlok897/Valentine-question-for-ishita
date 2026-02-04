[index.html](https://github.com/user-attachments/files/25066220/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine, Ishita? 💖</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #ff0000;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Arial Rounded MT Bold', 'Arial', sans-serif;
            overflow: hidden;
            position: relative;
        }

        .photo {
            position: absolute;
            width: 180px;
            height: 180px;
            border-radius: 40%;
            border: 4px solid white;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.6);
            background-size: cover;
            background-position: center;
            opacity: 0.85;
            transition: transform 0.3s, opacity 0.3s;
            z-index: 2;
        }

        .photo:hover {
            transform: scale(1.2);
            opacity: 1;
            border-color: #ffcccc;
            box-shadow: 0 0 25px rgba(255, 255, 255, 0.8);
        }


        .photo1 { background-image: url('photos/photo 1.jpeg'); }
        .photo2 { background-image: url('photos/photo 2.jpeg'); }
        .photo3 { background-image: url('photos/photo 3.jpeg'); }
        .photo4 { background-image: url('photos/photo 4.jpeg'); }
        .photo5 { background-image: url('photos/photo 5.jpg'); }
        .photo6 { background-image: url('photos/photo 6.jpg'); }
        .photo7 { background-image: url('photos/photo 7.jpg'); }
        .photo8 { background-image: url('photos/photo 8.jpg'); }
        
       

        .container {
            background: rgba(255, 255, 255, 0.97);
            padding: 40px 60px;
            border-radius: 25px;
            box-shadow: 0 0 40px rgba(0, 0, 0, 0.3);
            text-align: center;
            z-index: 10;
            position: relative;
            max-width: 500px;
            border: 8px solid #ff4d4d;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { border-color: #ff4d4d; }
            50% { border-color: #ff9999; }
            100% { border-color: #ff4d4d; }
        }

        h1 {
            color: #ff0000;
            font-size: 2.8rem;
            margin-bottom: 30px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
            line-height: 1.2;
        }

        .buttons {
            display: flex;
            gap: 30px;
            justify-content: center;
            margin-top: 20px;
        }

        .btn {
            padding: 20px 40px;
            font-size: 1.8rem;
            border: none;
            border-radius: 15px;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: bold;
            min-width: 150px;
            box-shadow: 0 6px 0 rgba(0, 0, 0, 0.2);
            z-index: 20;
            position: relative;
        }

        .btn:active {
            transform: translateY(4px);
            box-shadow: 0 2px 0 rgba(0, 0, 0, 0.2);
        }

        .yes-btn {
            background-color: #4CAF50;
            color: white;
        }

        .yes-btn:hover {
            background-color: #45a049;
            transform: scale(1.05);
        }

        .no-btn {
            background-color: #666;
            color: white;
            position: relative;
        }

        .hearts {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
            z-index: 1;
        }

        .heart {
            position: absolute;
            font-size: 2rem;
            color: pink;
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% {
                transform: translateY(0) rotate(0deg);
                opacity: 0.7;
            }
            50% {
                transform: translateY(-20px) rotate(180deg);
                opacity: 1;
            }
        }

        .message {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 50px;
            border-radius: 20px;
            box-shadow: 0 0 50px rgba(0, 0, 0, 0.5);
            z-index: 100;
            text-align: center;
            border: 10px solid #ff4d4d;
            max-width: 600px;
            width: 90%;
        }

        .message-content {
            animation: messageAppear 0.5s ease-out;
        }

        @keyframes messageAppear {
            0% {
                transform: scale(0.5);
                opacity: 0;
            }
            100% {
                transform: scale(1);
                opacity: 1;
            }
        }

        .message h2 {
            color: #ff0000;
            font-size: 3.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }

        .message h3 {
            color: #ff4d4d;
            font-size: 2.8rem;
            margin: 20px 0;
            padding: 10px;
            background: linear-gradient(45deg, #ffcccc, #ffffff);
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(255, 77, 77, 0.3);
        }

        .message p {
            font-size: 1.8rem;
            color: #333;
            margin: 20px 0;
            line-height: 1.6;
        }

        .hearts-container {
            font-size: 2.5rem;
            margin: 20px 0;
            animation: heartbeat 1.5s infinite;
        }

        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.1); }
        }

        .close-btn {
            background-color: #ff0000;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.5rem;
            border-radius: 10px;
            cursor: pointer;
            margin-top: 20px;
            transition: all 0.3s;
        }

        .close-btn:hover {
            background-color: #cc0000;
            transform: scale(1.05);
        }
    </style>
</head>
<body>
    <div class="hearts" id="hearts"></div>
    
    <!-- Floating Photos - 8 total -->
    <div class="photo photo1"></div>
    <div class="photo photo2"></div>
    <div class="photo photo3"></div>
    <div class="photo photo4"></div>
    <div class="photo photo5"></div>
    <div class="photo photo6"></div>
    <div class="photo photo7"></div>
    <div class="photo photo8"></div>

    <div class="container">
        <h1>💖 Will You Be My Valentine, Ishita? 💖</h1>
        <div class="buttons">
            <button class="btn yes-btn" id="yesBtn">YES! 💕</button>
            <button class="btn no-btn" id="noBtn">No 😢</button>
        </div>
    </div>

    <div class="message" id="message">
        <div class="message-content">
            <h2>YAY! 🎉💖</h2>
            <div class="hearts-container">💕💖💗💓💞💝</div>
            <h3>To My Dearest Ishita,</h3>
            <p>You've just made me the happiest person in the world! 💕</p>
            <p>I can't wait to spend this special day with you, my beautiful Valentine! 🥰</p>
            <p>Every moment with you is magical, and I'm so excited for our Valentine's Day together! ✨</p>
            <div class="hearts-container">💝💞💓💗💖💕</div>
            <p>With all my love, forever and always 💘</p>
            <button class="close-btn" onclick="closeMessage()">Close This Beautiful Message 💖</button>
        </div>
    </div>

    <script>
        // Create floating hearts
        const heartsContainer = document.getElementById('hearts');
        for (let i = 0; i < 25; i++) {
            const heart = document.createElement('div');
            heart.className = 'heart';
            heart.innerHTML = '💖';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.top = Math.random() * 100 + 'vh';
            heart.style.animationDelay = Math.random() * 5 + 's';
            heart.style.fontSize = (Math.random() * 2 + 1.5) + 'rem';
            heartsContainer.appendChild(heart);
        }

        // Initial positions for 8 photos (spread around screen)
        const photoPositions = [
            { x: 5, y: 10 },   // Top-left
            { x: 90, y: 15 },  // Top-right
            { x: 10, y: 85 },  // Bottom-left
            { x: 85, y: 80 },  // Bottom-right
            { x: 5, y: 45 },   // Middle-left
            { x: 90, y: 50 },  // Middle-right
            { x: 25, y: 15 },  // Top-center-left
            { x: 70, y: 85 }   // Bottom-center-right
        ];

        // Position all 8 photos
        const photos = document.querySelectorAll('.photo');
        photos.forEach((photo, index) => {
            if (photoPositions[index]) {
                photo.style.left = photoPositions[index].x + 'vw';
                photo.style.top = photoPositions[index].y + 'vh';
            }
        });

        // Animate photos to float around
        photos.forEach((photo, index) => {
            let currentPos = { ...photoPositions[index] };
            
            setInterval(() => {
                // Calculate new position (not too far from current)
                const newX = Math.max(5, Math.min(90, currentPos.x + (Math.random() * 30 - 15)));
                const newY = Math.max(10, Math.min(85, currentPos.y + (Math.random() * 30 - 15)));
                
                // Update position
                currentPos.x = newX;
                currentPos.y = newY;
                
                photo.style.transition = 'all 10s ease-in-out';
                photo.style.left = newX + 'vw';
                photo.style.top = newY + 'vh';
            }, 10000 + (index * 1000)); // Stagger animations
        });

        // Moving "No" button
        const noBtn = document.getElementById('noBtn');
        let moveCount = 0;
        
        noBtn.addEventListener('mouseover', function() {
            moveCount++;
            
            // Get button dimensions
            const btnWidth = noBtn.offsetWidth;
            const btnHeight = noBtn.offsetHeight;
            
            // Get viewport dimensions
            const vw = Math.max(document.documentElement.clientWidth || 0, window.innerWidth || 0);
            const vh = Math.max(document.documentElement.clientHeight || 0, window.innerHeight || 0);
            
            // Calculate max positions (avoid edges where photos might be)
            const maxX = vw - btnWidth - 50;
            const maxY = vh - btnHeight - 50;
            
            // Generate random position that avoids photos
            let randomX, randomY;
            let validPosition = false;
            
            // Try to find a position not too close to photos
            for (let attempts = 0; attempts < 10; attempts++) {
                randomX = Math.random() * (maxX - 50) + 25;
                randomY = Math.random() * (maxY - 50) + 25;
                
                validPosition = true;
                
                // Check distance from each photo
                photos.forEach(photo => {
                    const photoRect = photo.getBoundingClientRect();
                    const distance = Math.sqrt(
                        Math.pow(randomX - photoRect.left, 2) + 
                        Math.pow(randomY - photoRect.top, 2)
                    );
                    
                    if (distance < 150) { // Minimum distance from photos
                        validPosition = false;
                    }
                });
                
                if (validPosition) break;
            }
            
            // If no valid position found, just pick random
            if (!validPosition) {
                randomX = Math.random() * (maxX - 50) + 25;
                randomY = Math.random() * (maxY - 50) + 25;
            }
            
            // Apply new position
            noBtn.style.position = 'fixed';
            noBtn.style.left = randomX + 'px';
            noBtn.style.top = randomY + 'px';
            noBtn.style.transition = 'all 0.3s ease-out';
            
            // Make button smaller each time
            const scale = Math.max(0.5, 1 - (moveCount * 0.1));
            noBtn.style.transform = `scale(${scale})`;
            
            // Change text after a few moves
            if (moveCount >= 3) {
                const texts = [
                    "Are you sure? 😢", 
                    "Please? 💕", 
                    "Think again! 💖", 
                    "Give me a chance! 🥺", 
                    "Ishita please say yes! 💘",
                    "My heart is breaking! 💔",
                    "Don't break my heart! 🥺",
                    "I'll be so sad! 😭"
                ];
                noBtn.textContent = texts[Math.floor(Math.random() * texts.length)];
            }
        });

        // "Yes" button action
        const yesBtn = document.getElementById('yesBtn');
        const message = document.getElementById('message');
        
        yesBtn.addEventListener('click', function() {
            message.style.display = 'block';
            
            // Create explosion of hearts
            for (let i = 0; i < 60; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.innerHTML = '💖';
                heart.style.position = 'fixed';
                heart.style.left = '50%';
                heart.style.top = '50%';
                heart.style.fontSize = (Math.random() * 3 + 2) + 'rem';
                heart.style.zIndex = '1000';
                document.body.appendChild(heart);
                
                // Animate heart
                const angle = Math.random() * Math.PI * 2;
                const velocity = 3 + Math.random() * 2;
                const x = Math.cos(angle) * velocity;
                const y = Math.sin(angle) * velocity;
                
                let posX = 50;
                let posY = 50;
                
                const animate = () => {
                    posX += x;
                    posY += y;
                    heart.style.left = posX + 'vw';
                    heart.style.top = posY + 'vh';
                    heart.style.opacity = 1 - (Math.abs(posX - 50) + Math.abs(posY - 50)) / 100;
                    
                    if (Math.abs(posX - 50) < 100 && Math.abs(posY - 50) < 100) {
                        requestAnimationFrame(animate);
                    } else {
                        heart.remove();
                    }
                };
                animate();
            }
            
            // Add floating name hearts
            for (let i = 0; i < 20; i++) {
                setTimeout(() => {
                    const nameHeart = document.createElement('div');
                    nameHeart.className = 'heart';
                    nameHeart.innerHTML = 'Ishita 💖';
                    nameHeart.style.position = 'fixed';
                    nameHeart.style.left = Math.random() * 100 + 'vw';
                    nameHeart.style.top = '100vh';
                    nameHeart.style.fontSize = '1.5rem';
                    nameHeart.style.color = '#ff4d4d';
                    nameHeart.style.fontWeight = 'bold';
                    nameHeart.style.zIndex = '1000';
                    document.body.appendChild(nameHeart);
                    
                    // Animate name heart floating up
                    let pos = 100;
                    const floatUp = () => {
                        pos -= 0.5;
                        nameHeart.style.top = pos + 'vh';
                        nameHeart.style.opacity = (100 - pos) / 100;
                        
                        if (pos > -10) {
                            requestAnimationFrame(floatUp);
                        } else {
                            nameHeart.remove();
                        }
                    };
                    floatUp();
                }, i * 150);
            }
            
            // Make all photos come to center and pulse
            photos.forEach(photo => {
                photo.style.transition = 'all 1.5s ease-out';
                photo.style.left = '50%';
                photo.style.top = '50%';
                photo.style.transform = 'translate(-50%, -50%) scale(1.5)';
                photo.style.opacity = '0.9';
                photo.style.zIndex = '1000';
                
                // Reset after celebration
                setTimeout(() => {
                    const randomPos = photoPositions[Math.floor(Math.random() * photoPositions.length)];
                    photo.style.transition = 'all 2s ease-in-out';
                    photo.style.left = randomPos.x + 'vw';
                    photo.style.top = randomPos.y + 'vh';
                    photo.style.transform = 'translate(0, 0) scale(1)';
                }, 3000);
            });
            
            // Play celebration sound (optional)
            try {
                const audio = new Audio('https://assets.mixkit.co/sfx/preview/mixkit-winning-chimes-2015.mp3');
                audio.volume = 0.3;
                audio.play();
            } catch(e) {
                console.log("Audio not available");
            }
        });

        function closeMessage() {
            message.style.display = 'none';
            // Add more hearts when closing
            for (let i = 0; i < 15; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.innerHTML = 'Ishita 💘';
                heart.style.left = Math.random() * 100 + 'vw';
                heart.style.top = Math.random() * 100 + 'vh';
                heart.style.fontSize = '1.2rem';
                heart.style.color = '#ff0000';
                document.body.appendChild(heart);
            }
        }

        // Make sure initial photos are positioned
        window.addEventListener('load', () => {
            photos.forEach((photo, index) => {
                if (photoPositions[index]) {
                    photo.style.left = photoPositions[index].x + 'vw';
                    photo.style.top = photoPositions[index].y + 'vh';
                }
            });
        });
    </script>
</body>
</html>
