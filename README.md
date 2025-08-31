# ADZONTA
MAKE A WEBSITE
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valger King - Romantic Shayari by Ram Ji Kashyap</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            color: #fff;
            overflow-x: hidden;
        }

        .heart {
            position: absolute;
            font-size: 20px;
            color: #ff6b6b;
            opacity: 0.7;
            animation: float 6s ease-in-out infinite;
            z-index: 1;
        }

        @keyframes float {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 0.7;
            }
            50% {
                transform: translateY(-20px) rotate(180deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-40px) rotate(360deg);
                opacity: 0;
            }
        }

        .shayari-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 20px;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .shayari-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            background: rgba(255, 255, 255, 0.15);
        }

        .typewriter {
            overflow: hidden;
            border-right: .15em solid #ff6b6b;
            white-space: nowrap;
            margin: 0 auto;
            letter-spacing: .15em;
            animation: typing 3.5s steps(40, end), blink-caret .75s step-end infinite;
        }

        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }

        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #ff6b6b; }
        }

        .romantic-bg {
            background: linear-gradient(45deg, #ff6b6b, #ee5a52, #ff4757, #ff6b81);
            background-size: 400% 400%;
            animation: gradientShift 8s ease infinite;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .floating {
            animation: floating 3s ease-in-out infinite;
        }

        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        .category-btn {
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }

        .category-btn:hover {
            transform: scale(1.05);
            border-color: #ff6b6b;
            box-shadow: 0 5px 15px rgba(255, 107, 107, 0.3);
        }

        .heart-beat {
            animation: heartBeat 2s ease-in-out infinite;
        }

        @keyframes heartBeat {
            0% { transform: scale(1); }
            15% { transform: scale(1.3); }
            30% { transform: scale(1); }
            45% { transform: scale(1.3); }
            60% { transform: scale(1); }
        }
    </style>
</head>
<body class="min-h-screen">
    <!-- Floating Hearts Background -->
    <div id="hearts-container"></div>

    <!-- Navigation -->
    <nav class="romantic-bg py-4 px-6 shadow-lg">
        <div class="container mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="heart-beat text-3xl">❤️</div>
                <h1 class="text-2xl font-bold">Valger King</h1>
            </div>
            <div class="hidden md:flex space-x-6">
                <a href="#home" class="hover:text-pink-200 transition">Home</a>
                <a href="#shayari" class="hover:text-pink-200 transition">Shayari</a>
                <a href="#categories" class="hover:text-pink-200 transition">Categories</a>
                <a href="#about" class="hover:text-pink-200 transition">About</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="relative py-20 px-6">
        <div class="container mx-auto text-center">
            <div class="max-w-4xl mx-auto">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/0fc77210-d02c-43b3-ab8b-2d4d17dfc2b1.png" alt="Portrait of Ram Ji Kashyap - Valger King, romantic shayari poet with warm smile and traditional attire" class="mx-auto rounded-full w-48 h-48 object-cover border-4 border-white shadow-2xl floating mb-8" />
                <h1 class="text-5xl md:text-6xl font-bold mb-6 typewriter">Valger King</h1>
                <p class="text-xl md:text-2xl mb-8 opacity-90">Romantic Shayari by Ram Ji Kashyap</p>
                <p class="text-lg mb-12 max-w-2xl mx-auto leading-relaxed">
                    Where words dance with emotions and love finds its purest expression through the art of shayari.
                </p>
                <div class="space-x-4">
                    <button class="bg-pink-600 hover:bg-pink-700 text-white px-8 py-3 rounded-full font-semibold transition transform hover:scale-105">
                        Read Shayari
                    </button>
                    <button class="border-2 border-white hover:bg-white hover:text-pink-600 text-white px-8 py-3 rounded-full font-semibold transition">
                        Share Love
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Shayari -->
    <section id="shayari" class="py-16 px-6">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold text-center mb-12">Featured Romantic Shayari</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Shayari Card 1 -->
                <div class="shayari-card p-6 text-center">
                    <div class="text-pink-400 text-3xl mb-4">❤️</div>
                    <p class="text-lg leading-relaxed mb-4">
                        "Teri ek nazar ne kar diya hai ishq,<br>
                        Dil ki duniya badal di hai mohabbat ne,<br>
                        Pyaar ki rahon mein kho jana hai ab,<br>
                        Bas tumhari yaadon ka sahara hai."
                    </p>
                    <div class="text-sm opacity-75">~ Ram Ji Kashyap</div>
                </div>

                <!-- Shayari Card 2 -->
                <div class="shayari-card p-6 text-center">
                    <div class="text-pink-400 text-3xl mb-4">💖</div>
                    <p class="text-lg leading-relaxed mb-4">
                        "Dil ki dhadkan tumse hi kehti hai baatein,<br>
                        Aankhon mein basayi tumne hi raatein,<br>
                        Pyaar hai yeh ankahi daastaan,<br>
                        Jise likh raha hun main har pal subah-shaam."
                    </p>
                    <div class="text-sm opacity-75">~ Ram Ji Kashyap</div>
                </div>

                <!-- Shayari Card 3 -->
                <div class="shayari-card p-6 text-center">
                    <div class="text-pink-400 text-3xl mb-4">✨</div>
                    <p class="text-lg leading-relaxed mb-4">
                        "Mohabbat ki raahon mein mila hai jo pyaar,<br>
                        Woh rishta hai anmol tumhara humse,<br>
                        Har lamha tumhare sang bitana chahta hun,<br>
                        Yeh dil kehte hai tum ho khuda ka tohfa."
                    </p>
                    <div class="text-sm opacity-75">~ Ram Ji Kashyap</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Categories -->
    <section id="categories" class="py-16 px-6 bg-black bg-opacity-20">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold text-center mb-12">Shayari Categories</h2>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <button class="category-btn bg-pink-600 text-white py-4 px-6 rounded-lg">Romantic</button>
                <button class="category-btn bg-purple-600 text-white py-4 px-6 rounded-lg">Heartfelt</button>
                <button class="category-btn bg-red-500 text-white py-4 px-6 rounded-lg">Passionate</button>
                <button class="category-btn bg-blue-600 text-white py-4 px-6 rounded-lg">Emotional</button>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-6">
        <div class="container mx-auto">
            <div class="max-w-4xl mx-auto text-center">
                <h2 class="text-4xl font-bold mb-8">About Valger King</h2>
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/786f311d-fe87-4779-be60-536ac6b690a2.png" alt="Ram Ji Kashyap writing shayari in a peaceful garden setting with flowers and traditional decor" class="mx-auto rounded-2xl mb-8 w-full max-w-md" />
                <p class="text-lg leading-relaxed mb-6">
                    Ram Ji Kashyap, known as "Valger King," is a renowned romantic shayar whose words have touched millions of hearts. 
                    With a unique style that blends traditional Urdu poetry with contemporary emotions, his shayari resonates with 
                    lovers across generations.
                </p>
                <p class="text-lg leading-relaxed">
                    Each verse is crafted with deep emotion, capturing the essence of love, longing, and the beauty of human connections. 
                    Valger King continues to inspire and spread love through his beautiful words.
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="romantic-bg py-12 px-6">
        <div class="container mx-auto text-center">
            <div class="flex justify-center space-x-6 mb-6">
                <a href="#" class="text-2xl hover:text-pink-200 transition"><i class="fab fa-facebook"></i></a>
                <a href="#" class="text-2xl hover:text-pink-200 transition"><i class="fab fa-instagram"></i></a>
                <a href="#" class="text-2xl hover:text-pink-200 transition"><i class="fab fa-twitter"></i></a>
                <a href="#" class="text-2xl hover:text-pink-200 transition"><i class="fab fa-youtube"></i></a>
            </div>
            <p class="text-lg mb-4">© 2024 Valger King - Romantic Shayari by Ram Ji Kashyap</p>
            <p class="text-sm opacity-75">Spread love through beautiful words and heartfelt emotions</p>
        </div>
    </footer>

    <script>
        // Create floating hearts
        function createHearts() {
            const container = document.getElementById('hearts-container');
            for (let i = 0; i < 20; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.innerHTML = '❤️';
                heart.style.left = Math.random() * 100 + 'vw';
                heart.style.top = Math.random() * 100 + 'vh';
                heart.style.animationDelay = Math.random() * 6 + 's';
                container.appendChild(heart);
            }
        }

        // Typewriter effect
        function initTypewriter() {
            const elements = document.querySelectorAll('.typewriter');
            elements.forEach(el => {
                const text = el.textContent;
                el.style.width = '0';
                setTimeout(() => {
                    el.style.width = '100%';
                }, 100);
            });
        }

        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Initialize everything
        document.addEventListener('DOMContentLoaded', function() {
            createHearts();
            initTypewriter();
            
            // Add click animation to shayari cards
            const cards = document.querySelectorAll('.shayari-card');
            cards.forEach(card => {
                card.addEventListener('click', function() {
                    this.style.transform = 'scale(0.95)';
                    setTimeout(() => {
                        this.style.transform = '';
                    }, 300);
                });
            });
        });
    </script>
</body>
</html>

