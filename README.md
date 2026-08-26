<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>𝑰𝒃𝒓𝒂𝒉𝒊𝒎 | الصفحة الشخصية</title>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;900&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --bg-dark: #0b0f19;
            --card-bg: #151c2e;
            --card-hover: #1e2942;
            --accent-primary: #38bdf8;
            --accent-gold: #f59e0b;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --border-color: rgba(255, 255, 255, 0.08);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Cairo', sans-serif;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            line-height: 1.6;
            padding: 20px 12px;
            min-height: 100vh;
        }

        .container {
            max-width: 750px;
            margin: 0 auto;
        }

        /* Profile Header */
        header {
            text-align: center;
            padding: 30px 15px;
            background: linear-gradient(135deg, rgba(56, 189, 248, 0.1), rgba(245, 158, 11, 0.05));
            border-radius: 20px;
            border: 1px solid var(--border-color);
            margin-bottom: 25px;
            backdrop-filter: blur(10px);
        }

        .title-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            margin-bottom: 8px;
        }

        header h1 {
            font-size: 2.5rem;
            font-weight: 900;
            background: linear-gradient(45deg, #38bdf8, #f59e0b);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .spain-flag {
            width: 38px;
            height: auto;
            border-radius: 4px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.4);
        }

        header p {
            color: var(--text-muted);
            font-size: 1.1rem;
        }

        /* Sections */
        .section {
            background: var(--card-bg);
            border-radius: 16px;
            padding: 24px;
            margin-bottom: 24px;
            border: 1px solid var(--border-color);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.3);
        }

        .section-title {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 1.3rem;
            font-weight: 700;
            color: var(--accent-primary);
            border-bottom: 2px solid rgba(56, 189, 248, 0.2);
            padding-bottom: 10px;
            margin-bottom: 20px;
        }

        /* Social Links */
        .social-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(130px, 1fr));
            gap: 12px;
        }

        .social-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            padding: 12px 14px;
            border-radius: 12px;
            text-decoration: none;
            color: #fff;
            font-weight: 600;
            transition: all 0.3s ease;
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid var(--border-color);
        }

        .social-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.4);
        }

        .social-btn.telegram { background: #0088cc; }
        .social-btn.instagram { background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888); }
        .social-btn.tiktok { background: #000000; border: 1px solid #333; }
        .social-btn.whatsapp { background: #25D366; }
        .social-btn.youtube { background: #FF0000; }

        /* Cards Grid */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .person-card {
            background: var(--card-hover);
            border-radius: 14px;
            overflow: hidden;
            border: 1px solid var(--border-color);
            text-align: center;
            transition: transform 0.3s ease;
        }

        .person-card:hover {
            transform: translateY(-5px);
        }

        .person-img {
            width: 100%;
            height: 280px;
            object-fit: cover;
            object-position: top;
            background-color: #1e2942;
        }

        .person-info {
            padding: 15px;
        }

        .person-title {
            font-size: 1.15rem;
            font-weight: 700;
            color: var(--accent-gold);
        }

        .person-subtitle {
            font-size: 0.85rem;
            color: var(--text-muted);
            margin-top: 4px;
        }

        /* Games Grid */
        .games-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
            gap: 15px;
        }

        .game-card {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 12px;
            padding: 18px;
            text-align: center;
            border: 1px solid var(--border-color);
            font-weight: 700;
            font-size: 1.1rem;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        /* Hobbies & Love Section */
        .hobby-card {
            background: linear-gradient(135deg, rgba(245, 158, 11, 0.1), rgba(56, 189, 248, 0.05));
            border-radius: 12px;
            padding: 18px;
            margin-bottom: 12px;
            border: 1px solid var(--border-color);
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .hobby-card i {
            font-size: 1.8rem;
            color: var(--accent-gold);
        }

        .hobby-text h3 {
            font-size: 1.1rem;
            color: var(--text-main);
        }

        .hobby-text p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        footer {
            text-align: center;
            padding: 20px;
            color: var(--text-muted);
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- Header Section -->
        <header>
            <div class="title-container">
                <h1>𝑰𝒃𝒓𝒂𝒉𝒊𝒎</h1>
                <img src="https://flagcdn.com/w80/es.png" alt="علم إسبانيا" class="spain-flag" referrerpolicy="no-referrer">
            </div>
            <p>أهلاً بك في موقعي الشخصي ✨</p>
        </header>

        <!-- Social Media Accounts -->
        <div class="section">
            <div class="section-title">
                <i class="fa-solid fa-share-nodes"></i>
                <span>حساباتي الشخصية</span>
            </div>
            <div class="social-grid">
                <a href="https://t.me/V1_n_x" target="_blank" class="social-btn telegram">
                    <i class="fa-brands fa-telegram"></i> تليجرام
                </a>
                <a href="https://www.instagram.com/v1_n_x?igsi=YTV1M3RjNDYyNnly" target="_blank" class="social-btn instagram">
                    <i class="fa-brands fa-instagram"></i> إنستغرام
                </a>
                <a href="https://www.tiktok.com/@v1_n_x?_r=1&_t=ZS-99C8uNpo115" target="_blank" class="social-btn tiktok">
                    <i class="fa-brands fa-tiktok"></i> تيك توك
                </a>
                <a href="https://wa.me/qr/U5KWRTSQZPZLE1" target="_blank" class="social-btn whatsapp">
                    <i class="fa-brands fa-whatsapp"></i> واتساب
                </a>
                <a href="https://youtube.com/@ibrahim-n4b1u?si=b-Ev2FQeE8Ev77P8" target="_blank" class="social-btn youtube">
                    <i class="fa-brands fa-youtube"></i> يوتيوب
                </a>
            </div>
        </div>

        <!-- Favorite Players -->
        <div class="section">
            <div class="section-title">
                <i class="fa-solid fa-futbol"></i>
                <span>أعمامي (اللاعبون المفضلون)</span>
            </div>
            <div class="cards-grid">
                <!-- Cristiano Ronaldo -->
                <div class="person-card">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/2/23/Cristiano_Ronaldo_WC2022_-_01.jpg" alt="كريستيانو رونالدو" class="person-img" referrerpolicy="no-referrer">
                    <div class="person-info">
                        <div class="person-title">العم كريستيانو رونالدو 👑</div>
                        <div class="person-subtitle">CR7 - The King</div>
                    </div>
                </div>
                <!-- Del Piero -->
                <div class="person-card">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/2/29/Alessandro_Del_Piero_Juventus.jpg" alt="ديل بيرو" class="person-img" referrerpolicy="no-referrer">
                    <div class="person-info">
                        <div class="person-title">العم دل بيرو 🇮🇹</div>
                        <div class="person-subtitle">Alessandro Del Piero</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Favorite Actors Section -->
        <div class="section">
            <div class="section-title">
                <i class="fa-solid fa-clapperboard"></i>
                <span>الممثلون المفضلون</span>
            </div>
            <div class="cards-grid">
                <!-- Patrick Jane -->
                <div class="person-card">
                    <img src="https://static.wikia.nocookie.net/thementalist/images/3/35/Patrick_Jane12.jpg/revision/latest?cb=20251226073731" alt="باتريك جين" class="person-img" referrerpolicy="no-referrer">
                    <div class="person-info">
                        <div class="person-title">باتريك جين ☕</div>
                        <div class="person-subtitle">Patrick Jane (The Mentalist)</div>
                    </div>
                </div>
                <!-- The Professor -->
                <div class="person-card">
                    <img src="https://upload.wikimedia.org/wikipedia/en/d/d5/Professor_%28Money_Heist%29.jpg" alt="البروفيسور" class="person-img" referrerpolicy="no-referrer">
                    <div class="person-info">
                        <div class="person-title">البروفيسور 👓</div>
                        <div class="person-subtitle">El Profesor (La Casa de Papel)</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Favorite Games -->
        <div class="section">
            <div class="section-title">
                <i class="fa-solid fa-gamepad"></i>
                <span>ألعابي المفضلة</span>
            </div>
            <div class="games-grid">
                <div class="game-card">
                    <i class="fa-solid fa-crosshairs" style="color: #38bdf8;"></i>
                    <span>ببجي موبايل</span>
                </div>
                <div class="game-card">
                    <i class="fa-solid fa-futbol" style="color: #f59e0b;"></i>
                    <span>بيس موبايل</span>
                </div>
            </div>
        </div>

        <!-- Hobbies & Interests -->
        <div class="section">
            <div class="section-title">
                <i class="fa-solid fa-heart"></i>
                <span>هواياتي وما أحبه</span>
            </div>
            <div class="hobby-card">
                <i class="fa-solid fa-bed"></i>
                <div class="hobby-text">
                    <h3>الهواية المفضلة</h3>
                    <p>النوم 😴</p>
                </div>
            </div>
            <div class="hobby-card">
                <i class="fa-solid fa-moon"></i>
                <div class="hobby-text">
                    <h3>أكثر شيء أحبه</h3>
                    <p><strong>My bed</strong> 🛏️</p>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <footer>
            <p>صُمم لـ 𝑰𝒃𝒓𝒂𝒉𝒊𝒎 🇪🇸</p>
        </footer>
    </div>

</body>
</html>
