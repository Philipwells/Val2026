<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Valentine's Day, Boluwatife 💝</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #ff6b9d 0%, #c44569 100%);
            min-height: 100vh;
            padding: 20px;
            overflow-x: hidden;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            padding: 40px;
            animation: slideIn 0.8s ease-out;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
        }

        .heart-emoji {
            font-size: 60px;
            margin-bottom: 20px;
            animation: heartbeat 1.5s ease-in-out infinite;
        }

        @keyframes heartbeat {
            0%, 100% {
                transform: scale(1);
            }
            25% {
                transform: scale(1.1);
            }
            50% {
                transform: scale(1.2);
            }
            75% {
                transform: scale(1.1);
            }
        }

        h1 {
            color: #c44569;
            font-size: 42px;
            margin-bottom: 10px;
            letter-spacing: 1px;
        }

        .subtitle {
            color: #ff6b9d;
            font-size: 24px;
            margin-bottom: 15px;
            font-weight: 300;
        }

        .rose-line {
            font-size: 30px;
            margin: 20px 0;
            letter-spacing: 10px;
        }

        .names {
            background: linear-gradient(135deg, #ff6b9d 0%, #c44569 100%);
            color: white;
            padding: 20px;
            border-radius: 15px;
            margin-bottom: 30px;
            font-size: 20px;
            letter-spacing: 2px;
        }

        .names span {
            display: block;
            margin: 8px 0;
        }

        /* Photo Gallery Styles */
        .photo-section {
            margin-bottom: 40px;
        }

        .section-title {
            color: #c44569;
            font-size: 24px;
            text-align: center;
            margin-bottom: 25px;
            font-weight: bold;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .photo-card {
            position: relative;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
            background: #f0f0f0;
            aspect-ratio: 1;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 3px solid #ffe5f0;
        }

        .photo-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 15px 40px rgba(196, 69, 105, 0.3);
        }

        .photo-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .photo-card.empty {
            background: linear-gradient(135deg, #ffe5f0 0%, #ffb3d9 100%);
            color: #c44569;
            font-weight: bold;
            font-size: 14px;
            text-align: center;
            padding: 20px;
        }

        /* Message Section */
        .message {
            color: #333;
            font-size: 18px;
            line-height: 1.8;
            margin-bottom: 30px;
            text-align: center;
        }

        .special-message {
            background: #ffe5f0;
            padding: 20px;
            border-left: 5px solid #ff6b9d;
            margin-bottom: 30px;
            border-radius: 5px;
            font-style: italic;
            color: #c44569;
            font-size: 16px;
        }

        /* Button Group */
        .button-group {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }

        button {
            background: linear-gradient(135deg, #ff6b9d 0%, #c44569 100%);
            color: white;
            border: none;
            padding: 15px 30px;
            border-radius: 25px;
            font-size: 16px;
            cursor: pointer;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            font-weight: bold;
            letter-spacing: 1px;
        }

        button:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 30px rgba(196, 69, 105, 0.4);
        }

        button:active {
            transform: scale(0.95);
        }

        .date {
            color: #999;
            font-size: 14px;
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #eee;
        }

        /* Modal for full image view */
        .modal {
            display: none;
            position: fixed;
            z-index: 2000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            animation: fadeIn 0.3s ease-out;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        .modal-content {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            max-width: 90vw;
            max-height: 90vh;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5);
        }

        .modal-content img {
            width: 100%;
            height: 100%;
            object-fit: contain;
            max-height: 85vh;
        }

        .close {
            position: absolute;
            right: 20px;
            top: 20px;
            color: white;
            font-size: 40px;
            font-weight: bold;
            cursor: pointer;
            background: rgba(0, 0, 0, 0.5);
            width: 50px;
            height: 50px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            transition: background 0.3s ease;
        }

        .close:hover {
            background: rgba(0, 0, 0, 0.8);
        }

        .floating-hearts {
            position: fixed;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
            z-index: -1;
        }

        .heart {
            position: absolute;
            color: #ff6b9d;
            font-size: 24px;
            opacity: 0.6;
            animation: float 6s ease-in infinite;
        }

        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 0.6;
            }
            90% {
                opacity: 0.6;
            }
            100% {
                transform: translateY(-100vh) rotate(360deg);
                opacity: 0;
            }
        }

        @media (max-width: 600px) {
            .container {
                padding: 20px;
            }

            h1 {
                font-size: 32px;
            }

            .gallery {
                grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            }
        }
    </style>
</head>
<body>
    <div class="floating-hearts" id="heartsContainer"></div>

    <div class="container">
        <div class="header">
            <div class="heart-emoji">💝</div>
            <h1>Happy Valentine's Day</h1>
            <p class="subtitle">To My Beautiful Boluwatife</p>
            <div class="rose-line">🌹 💕 🌹</div>

            <div class="names">
                <span>To: Boluwatife ✨</span>
                <span style="margin: 15px 0;">💌</span>
                <span>From: Olawale 💕</span>
            </div>
        </div>

        <!-- Photo Gallery Section -->
        <div class="photo-section">
            <div class="section-title">📸 Our Beautiful Moments 📸</div>
            <div class="gallery" id="gallery">
                <!-- Photos will be added here -->
            </div>
        </div>

        <!-- Message Section -->
        <div class="message">
            <p>Today is a special day, but it doesn't compare to how special you are to me every single day.</p>
        </div>

        <div class="special-message">
            "In all the world, there is no heart for me like yours. In all the world, there is no love for you like mine." 💕
        </div>

        <div class="message">
            <p>Thank you for being the reason I smile, the reason I believe in love, and the reason my life is so beautiful.</p>
            <p style="margin-top: 15px;">You mean the world to me, Boluwatife. Every moment with you is a treasure.</p>
        </div>

        <!-- Action Buttons -->
        <div class="button-group">
            <button onclick="showAlert()">💝 Surprise Message</button>
            <button onclick="createConfetti()">🎉 Celebrate!</button>
            <button onclick="document.getElementById('photoInput').click()">📸 Add Photos</button>
        </div>

        <input type="file" id="photoInput" multiple accept="image/*" style="display: none;" onchange="handlePhotoUpload(event)">

        <div class="date">
            February 14, 2026 💕 Happy Valentine's Day
        </div>
    </div>

    <!-- Modal for viewing full images -->
    <div id="imageModal" class="modal">
        <span class="close" onclick="closeModal()">&times;</span>
        <div class="modal-content">
            <img id="modalImage" src="" alt="Full size image">
        </div>
    </div>

    <script>
        // Sample photos - Replace these with your actual photo URLs
        const photos = [
            "7257314a-3ffc-4b04-bb44-2b25cec7b0d4-1.jpg"
        ];

        // Initialize gallery
        function initGallery() {
            const gallery = document.getElementById('gallery');
            gallery.innerHTML = '';

            photos.forEach((photo, index) => {
                const photoCard = document.createElement('div');
                photoCard.className = 'photo-card';
                
                if (photo) {
                    const img = document.createElement('img');
                    img.src = photo;
                    img.alt = `Memory ${index + 1}`;
                    img.onclick = () => openModal(photo);
                    photoCard.appendChild(img);
                } else {
                    photoCard.classList.add('empty');
                    photoCard.textContent = '📸 Add a photo';
                }
                
                gallery.appendChild(photoCard);
            });

            // Add empty slots if less than 6 photos
            while (gallery.children.length < 6) {
                const emptyCard = document.createElement('div');
                emptyCard.className = 'photo-card empty';
                emptyCard.textContent = '📸 Add a photo';
                emptyCard.onclick = () => document.getElementById('photoInput').click();
                gallery.appendChild(emptyCard);
            }
        }

        // Open modal to view full image
        function openModal(imageSrc) {
            const modal = document.getElementById('imageModal');
            const modalImage = document.getElementById('modalImage');
            modalImage.src = imageSrc;
            modal.style.display = 'block';
        }

        // Close modal
        function closeModal() {
            document.getElementById('imageModal').style.display = 'none';
        }

        // Handle photo upload
        function handlePhotoUpload(event) {
            const files = event.target.files;
            for (let file of files) {
                const reader = new FileReader();
                reader.onload = (e) => {
                    photos.push(e.target.result);
                    initGallery();
                };
                reader.readAsDataURL(file);
            }
        }

        // Show surprise message
        function showAlert() {
            const messages = [
                "You are my greatest love story 💕",
                "Forever starts with you 💑",
                "You make my heart skip a beat 💗",
                "I love you more every day 💕",
                "You are my favorite person 💕",
                "My heart belongs to you 💕",
                "Every day with you is a blessing 💕",
                "You are my reason to smile 💕"
            ];
            const randomMessage = messages[Math.floor(Math.random() * messages.length)];
            alert(randomMessage);
        }

        // Create confetti effect
        function createConfetti() {
            const colors = ['#ff6b9d', '#c44569', '#ff1744', '#f50057'];
            const confettiPieces = 50;

            for (let i = 0; i < confettiPieces; i++) {
                const confetti = document.createElement('div');
                confetti.style.position = 'fixed';
                confetti.style.width = '10px';
                confetti.style.height = '10px';
                confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                confetti.style.left = Math.random() * window.innerWidth + 'px';
                confetti.style.top = '-10px';
                confetti.style.borderRadius = '50%';
                confetti.style.pointerEvents = 'none';
                confetti.style.zIndex = '1000';

                document.body.appendChild(confetti);

                const duration = Math.random() * 3 + 2;
                const leftOffset = (Math.random() - 0.5) * 200;

                confetti.animate([
                    { transform: 'translateY(0) translateX(0) rotate(0deg)', opacity: 1 },
                    { transform: `translateY(${window.innerHeight + 10}px) translateX(${leftOffset}px) rotate(720deg)`, opacity: 0 }
                ], {
                    duration: duration * 1000,
                    easing: 'cubic-bezier(0.25, 0.46, 0.45, 0.94)'
                });

                setTimeout(() => confetti.remove(), duration * 1000);
            }
        }

        // Create floating hearts
        function createFloatingHearts() {
            const container = document.getElementById('heartsContainer');
            for (let i = 0; i < 15; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.textContent = '❤️';
                heart.style.left = Math.random() * 100 + '%';
                heart.style.animationDelay = Math.random() * 3 + 's';
                heart.style.animationDuration = (5 + Math.random() * 3) + 's';
                container.appendChild(heart);
            }
        }

        // Close modal when clicking outside
        window.onclick = (event) => {
            const modal = document.getElementById('imageModal');
            if (event.target === modal) {
                closeModal();
            }
        }

        // Initialize on page load
        initGallery();
        createFloatingHearts();
    </script>
</body>
</html>
