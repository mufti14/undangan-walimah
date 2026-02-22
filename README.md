<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Undangan Pernikahan - Amirga & Aisyah | Undangan Pernikahan</title>
    
    <!-- Font Awesome 6 -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <!-- Google Fonts Premium -->
    <link href="https://fonts.googleapis.com/css2?family=Parisienne&family=Cormorant+Garamond:wght@300;400;500;600;700&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">
    
    <!-- AOS Animation Library -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    
    <style>
	
		/* Perbaikan untuk dropdown/select */
.form-group select {
    width: 100%;
    padding: 15px 20px;
    background: rgba(255,255,255,0.05);
    border: 1px solid rgba(212, 175, 55, 0.2);
    border-radius: 12px;
    font-family: 'Montserrat', sans-serif;
    font-size: 14px;
    color: #fff; /* Warna teks setelah dipilih */
    transition: all 0.3s;
    appearance: none; /* Menghilangkan arrow default */
    -webkit-appearance: none;
    -moz-appearance: none;
    background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="%23d4af37" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="6 9 12 15 18 9"></polyline></svg>');
    background-repeat: no-repeat;
    background-position: right 15px center;
    background-size: 16px;
}

/* Warna untuk option yang belum dipilih (placeholder) */
.form-group select option {
    background-color: #1a1a1a;
    color: #fff;
}

/* Warna khusus untuk option yang disabled (placeholder) */
.form-group select option[disabled][selected] {
    color: #999; /* Warna abu-abu untuk teks placeholder */
}

/* Warna saat hover di option */
.form-group select option:hover {
    background-color: #d4af37;
    color: #000;
}
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            background: #1a1a1a;
            color: #d4af37;
            overflow-x: hidden;
        }
        
        /* Premium Background dengan Pattern */
        .premium-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #0a0a0a 0%, #1f1f1f 100%);
            z-index: -2;
        }
        
        .premium-bg::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" opacity="0.1"><path d="M20,30 Q30,20 40,30 T60,30" stroke="%23d4af37" fill="none" stroke-width="0.5"/><path d="M20,50 Q30,40 40,50 T60,50" stroke="%23d4af37" fill="none" stroke-width="0.5"/><path d="M20,70 Q30,60 40,70 T60,70" stroke="%23d4af37" fill="none" stroke-width="0.5"/></svg>');
            background-size: 200px 200px;
            opacity: 0.3;
        }
        
        /* Animasi Bunga Jatuh */
        .flower-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .flower {
            position: absolute;
            color: rgba(212, 175, 55, 0.2);
            font-size: 20px;
            animation: fall linear infinite;
        }
        
        @keyframes fall {
            to {
                transform: translateY(100vh) rotate(360deg);
            }
        }
        
        /* Splash Screen Mewah */
        .splash-screen {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
            position: relative;
            background: linear-gradient(135deg, rgba(10,10,10,0.95) 0%, rgba(31,31,31,0.98) 100%);
        }
        
        .splash-content {
            position: relative;
            z-index: 2;
            max-width: 500px;
            animation: glowPulse 3s infinite;
        }
        
        .splash-border {
            border: 2px solid rgba(212, 175, 55, 0.3);
            border-radius: 30px;
            padding: 40px 20px;
            position: relative;
            background: rgba(10,10,10,0.7);
            backdrop-filter: blur(10px);
            box-shadow: 0 0 50px rgba(212, 175, 55, 0.2);
        }
        
        .splash-border::before,
        .splash-border::after {
            content: '✦';
            position: absolute;
            font-size: 24px;
            color: #d4af37;
            opacity: 0.5;
        }
        
        .splash-border::before {
            top: -15px;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .splash-border::after {
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .splash-subtitle {
            font-family: 'Parisienne', cursive;
            font-size: 32px;
            color: #d4af37;
            margin-bottom: 15px;
            text-shadow: 0 0 20px rgba(212, 175, 55, 0.5);
        }
        
        .splash-title {
            font-family: 'Cormorant Garamond', serif;
            font-size: 64px;
            font-weight: 700;
            color: #fff;
            margin-bottom: 20px;
            line-height: 1.2;
            letter-spacing: 2px;
        }
        
        .splash-date {
            font-size: 18px;
            letter-spacing: 5px;
            margin-bottom: 40px;
            color: #d4af37;
            position: relative;
            display: inline-block;
        }
        
        .splash-date::before,
        .splash-date::after {
            content: '';
            position: absolute;
            top: 50%;
            width: 50px;
            height: 1px;
            background: linear-gradient(90deg, transparent, #d4af37, transparent);
        }
        
        .splash-date::before {
            right: 100%;
            margin-right: 20px;
        }
        
        .splash-date::after {
            left: 100%;
            margin-left: 20px;
        }
        
        .splash-button {
            background: linear-gradient(135deg, #d4af37 0%, #b49450 100%);
            border: none;
            color: #000;
            padding: 18px 50px;
            font-size: 16px;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.4s;
            font-weight: 600;
            letter-spacing: 3px;
            margin-top: 30px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.3);
        }
        
        .splash-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            transition: left 0.5s;
        }
        
        .splash-button:hover::before {
            left: 100%;
        }
        
        .splash-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 40px rgba(212, 175, 55, 0.4);
        }
        
        /* Main Content Mewah */
        .main-content {
            max-width: 500px;
            margin: 0 auto;
            background: rgba(10,10,10,0.8);
            backdrop-filter: blur(10px);
            display: none;
            position: relative;
            box-shadow: 0 0 100px rgba(212, 175, 55, 0.1);
        }
        
        /* Gold Accent Lines */
        .gold-line {
            height: 1px;
            background: linear-gradient(90deg, transparent, #d4af37, #d4af37, #d4af37, transparent);
            width: 80%;
            margin: 0 auto;
        }
        
        /* Header Mewah */
        .royal-header {
            text-align: center;
            padding: 80px 20px 50px;
            position: relative;
            background: linear-gradient(135deg, rgba(0,0,0,0.9) 0%, rgba(20,20,20,0.95) 100%);
        }
        
        .royal-header::before {
            content: '♕';
            position: absolute;
            top: 30px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 48px;
            color: rgba(212, 175, 55, 0.2);
            font-family: serif;
        }
        
        .header-floral {
            font-size: 48px;
            color: #d4af37;
            opacity: 0.3;
            margin-bottom: 20px;
        }
        
        .couple-names {
            font-family: 'Parisienne', cursive;
            font-size: 56px;
            color: #d4af37;
            margin-bottom: 10px;
            text-shadow: 0 0 30px rgba(212, 175, 55, 0.3);
        }
        
        .and-symbol {
            font-family: 'Parisienne', cursive;
            font-size: 48px;
            color: #d4af37;
            margin: 20px 0;
            position: relative;
        }
        
        .and-symbol::before,
        .and-symbol::after {
            content: '';
            position: absolute;
            top: 50%;
            width: 60px;
            height: 1px;
            background: linear-gradient(90deg, transparent, #d4af37, transparent);
        }
        
        .and-symbol::before {
            right: 100%;
            margin-right: 20px;
        }
        
        .and-symbol::after {
            left: 100%;
            margin-left: 20px;
        }
        
        .couple-parents {
            font-size: 14px;
            color: #fff;
            letter-spacing: 2px;
            opacity: 0.8;
            line-height: 1.8;
        }
        
        /* Section Mewah */
        .royal-section {
            padding: 60px 25px;
            text-align: center;
            position: relative;
        }
        
        .royal-section::before {
            content: '✦';
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            font-size: 24px;
            color: #d4af37;
            opacity: 0.5;
        }
        
        .section-title {
            font-family: 'Cormorant Garamond', serif;
            font-size: 42px;
            font-weight: 600;
            color: #d4af37;
            margin-bottom: 20px;
            position: relative;
            display: inline-block;
        }
        
        .section-title::before,
        .section-title::after {
            content: '✦';
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            font-size: 20px;
            color: #d4af37;
            opacity: 0.5;
        }
        
        .section-title::before {
            left: -40px;
        }
        
        .section-title::after {
            right: -40px;
        }
        
        .section-subtitle {
            font-size: 14px;
            color: #fff;
            letter-spacing: 4px;
            margin-bottom: 30px;
            text-transform: uppercase;
            opacity: 0.7;
        }
        
        /* Card Mewah dengan Glassmorphism */
        .royal-card {
            background: rgba(20,20,20,0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(212, 175, 55, 0.2);
            border-radius: 20px;
            padding: 40px 30px;
            margin: 30px 0;
            box-shadow: 0 20px 50px rgba(0,0,0,0.5);
            position: relative;
            overflow: hidden;
        }
        
        .royal-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 2px;
            background: linear-gradient(90deg, transparent, #d4af37, #d4af37, #d4af37, transparent);
        }
        
        .royal-card::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, #d4af37, transparent);
        }
        
        /* Countdown Mewah */
        .countdown {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 40px 0;
        }
        
        .countdown-item {
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.1) 0%, rgba(212, 175, 55, 0.05) 100%);
            border: 1px solid rgba(212, 175, 55, 0.2);
            border-radius: 15px;
            padding: 20px 15px;
            min-width: 80px;
            position: relative;
        }
        
        .countdown-item::before {
            content: '';
            position: absolute;
            top: -5px;
            left: -5px;
            right: -5px;
            bottom: -5px;
            border: 1px solid rgba(212, 175, 55, 0.1);
            border-radius: 20px;
            pointer-events: none;
        }
        
        .countdown-number {
            font-family: 'Cormorant Garamond', serif;
            font-size: 42px;
            font-weight: 700;
            color: #d4af37;
            line-height: 1;
        }
        
        .countdown-label {
            font-size: 12px;
            color: #fff;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-top: 5px;
        }
        
        /* Date Items */
        .date-item {
            margin-bottom: 35px;
            position: relative;
        }
        
        .date-item i {
            color: #d4af37;
            font-size: 32px;
            margin-bottom: 15px;
            opacity: 0.8;
        }
        
        .date-item h3 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 28px;
            color: #d4af37;
            margin-bottom: 10px;
        }
        
        .date-item p {
            font-size: 16px;
            color: #fff;
            opacity: 0.9;
            line-height: 1.8;
        }
        
        .event-separator {
            width: 100px;
            height: 1px;
            background: linear-gradient(90deg, transparent, #d4af37, transparent);
            margin: 30px auto;
        }
        
        /* Location */
        .venue-name {
            font-family: 'Cormorant Garamond', serif;
            font-size: 32px;
            color: #d4af37;
            margin-bottom: 15px;
        }
        
        .venue-address {
            font-size: 15px;
            color: #fff;
            margin-bottom: 25px;
            line-height: 1.8;
            opacity: 0.9;
        }
        
        .map-button {
            display: inline-block;
            background: transparent;
            border: 2px solid #d4af37;
            color: #d4af37;
            padding: 15px 40px;
            border-radius: 50px;
            text-decoration: none;
            font-size: 14px;
            transition: all 0.4s;
            font-weight: 600;
            letter-spacing: 2px;
            position: relative;
            overflow: hidden;
            z-index: 1;
        }
        
        .map-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: #d4af37;
            transition: left 0.4s;
            z-index: -1;
        }
        
        .map-button:hover {
            color: #000;
        }
        
        .map-button:hover::before {
            left: 0;
        }
        
        /* Gallery Mewah */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
            margin-top: 40px;
        }
        
        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 15px;
            border: 2px solid rgba(212, 175, 55, 0.2);
            aspect-ratio: 3/4;
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.6s;
        }
        
        .gallery-item:hover img {
            transform: scale(1.1);
        }
        
        .gallery-item::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(to bottom, transparent 50%, rgba(212, 175, 55, 0.2));
            pointer-events: none;
        }
        
        /* Form Mewah */
        .royal-form {
            background: rgba(20,20,20,0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(212, 175, 55, 0.2);
            border-radius: 20px;
            padding: 40px 30px;
            margin-top: 30px;
        }
        
        .form-group {
            margin-bottom: 25px;
            text-align: left;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: #d4af37;
            font-size: 14px;
            font-weight: 500;
            letter-spacing: 1px;
        }
        
        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 15px 20px;
            background: rgba(255,255,255,0.05);
            border: 1px solid rgba(212, 175, 55, 0.2);
            border-radius: 12px;
            font-family: 'Montserrat', sans-serif;
            font-size: 14px;
            color: #fff;
            transition: all 0.3s;
        }
        
        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #d4af37;
            box-shadow: 0 0 20px rgba(212, 175, 55, 0.2);
        }
        
        .form-group input::placeholder,
        .form-group textarea::placeholder {
            color: rgba(255,255,255,0.3);
        }
        
        .submit-btn {
            background: linear-gradient(135deg, #d4af37 0%, #b49450 100%);
            color: #000;
            padding: 18px 40px;
            border: none;
            border-radius: 50px;
            font-size: 16px;
            cursor: pointer;
            transition: all 0.4s;
            width: 100%;
            font-weight: 600;
            letter-spacing: 2px;
            position: relative;
            overflow: hidden;
        }
        
        .submit-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            transition: left 0.5s;
        }
        
        .submit-btn:hover::before {
            left: 100%;
        }
        
        /* Guestbook */
        .guestbook-item {
            background: rgba(20,20,20,0.5);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(212, 175, 55, 0.2);
            border-radius: 15px;
            padding: 25px;
            margin-bottom: 20px;
            text-align: left;
            transition: transform 0.3s;
        }
        
        .guestbook-item:hover {
            transform: translateX(5px);
            border-color: rgba(212, 175, 55, 0.5);
        }
        
        .guestbook-name {
            font-weight: 600;
            color: #d4af37;
            margin-bottom: 8px;
            font-size: 18px;
        }
        
        .guestbook-message {
            font-size: 14px;
            color: #fff;
            margin-bottom: 8px;
            line-height: 1.6;
            opacity: 0.9;
        }
        
        .guestbook-date {
            font-size: 12px;
            color: rgba(212, 175, 55, 0.5);
        }
        
        /* Footer Mewah */
        .royal-footer {
            background: linear-gradient(135deg, #000 0%, #1a1a1a 100%);
            color: #fff;
            text-align: center;
            padding: 60px 20px 40px;
            position: relative;
            border-top: 1px solid rgba(212, 175, 55, 0.2);
        }
        
        .royal-footer::before {
            content: '♕';
            position: absolute;
            top: -20px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 40px;
            color: #d4af37;
            background: #000;
            padding: 0 20px;
        }
        
        .footer-quote {
            font-family: 'Parisienne', cursive;
            font-size: 28px;
            color: #d4af37;
            margin: 20px 0;
        }
        
        .footer-links {
            margin: 30px 0;
        }
        
        .footer-links a {
            color: #d4af37;
            margin: 0 15px;
            font-size: 24px;
            text-decoration: none;
            transition: all 0.3s;
            display: inline-block;
        }
        
        .footer-links a:hover {
            transform: translateY(-5px);
            text-shadow: 0 10px 20px rgba(212, 175, 55, 0.3);
        }
        
        /* Music Player */
        .music-player {
            position: fixed;
            bottom: 30px;
            right: 30px;
            z-index: 1000;
        }
        
        .music-toggle {
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, #d4af37 0%, #b49450 100%);
            border: none;
            border-radius: 50%;
            color: #000;
            cursor: pointer;
            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.3);
            transition: all 0.4s;
            font-size: 24px;
            position: relative;
            overflow: hidden;
        }
        
        .music-toggle::before {
            content: '';
            position: absolute;
            top: -5px;
            left: -5px;
            right: -5px;
            bottom: -5px;
            border: 2px solid rgba(255,255,255,0.3);
            border-radius: 50%;
            animation: pulse 2s infinite;
        }
        
        .music-toggle:hover {
            transform: scale(1.1) rotate(360deg);
        }
        
        /* Floating Elements */
        .floating-gold {
            position: absolute;
            font-size: 24px;
            color: #d4af37;
            opacity: 0.1;
            pointer-events: none;
        }
        
        /* ===== CSS TAMBAHAN UNTUK NOTIFIKASI DAN GUESTBOOK ===== */
        @keyframes slideDown {
            from { transform: translate(-50%, -20px); opacity: 0; }
            to { transform: translate(-50%, 0); opacity: 1; }
        }
        
        @keyframes fadeOut {
            from { opacity: 1; }
            to { opacity: 0; }
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        @keyframes pulse {
            0% { transform: scale(1); opacity: 1; }
            100% { transform: scale(1.3); opacity: 0; }
        }
        
        @keyframes glowPulse {
            0%, 100% { text-shadow: 0 0 30px rgba(212, 175, 55, 0.3); }
            50% { text-shadow: 0 0 50px rgba(212, 175, 55, 0.6); }
        }
        
        .fa-spinner {
            animation: spin 1s linear infinite;
        }
        
        .guestbook-list {
            margin-top: 30px;
            max-height: 400px;
            overflow-y: auto;
            padding-right: 10px;
        }
        
        .guestbook-list::-webkit-scrollbar {
            width: 5px;
        }
        
        .guestbook-list::-webkit-scrollbar-track {
            background: rgba(212,175,55,0.1);
        }
        
        .guestbook-list::-webkit-scrollbar-thumb {
            background: #d4af37;
            border-radius: 10px;
        }
        
        /* Responsive */
        @media (max-width: 480px) {
            .splash-title {
                font-size: 48px;
            }
            
            .couple-names {
                font-size: 42px;
            }
            
            .section-title {
                font-size: 32px;
            }
            
            .section-title::before,
            .section-title::after {
                display: none;
            }
            
            .countdown {
                gap: 10px;
            }
            
            .countdown-item {
                min-width: 60px;
                padding: 15px 10px;
            }
            
            .countdown-number {
                font-size: 32px;
            }
        }
    </style>
    
    <!-- AOS Script -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
</head>
<body>
    <div class="premium-bg"></div>
    
    <!-- Animasi Bunga Jatuh -->
    <div class="flower-container" id="flowerContainer"></div>
    
    <!-- Splash Screen -->
    <div class="splash-screen" id="splashScreen">
        <div class="splash-content" data-aos="fade-up" data-aos-duration="1500">
            <div class="splash-border">
                <div class="splash-subtitle">Undangan Walimah</div>
                <div class="splash-title">Amirga & Aisyah</div>
                <div class="gold-line"></div>
                <div class="splash-date">5 April 2026</div>
                <button class="splash-button" onclick="openInvitation()">
                    <i class="far fa-envelope" style="margin-right: 10px;"></i>BUKA UNDANGAN
                </button>
            </div>
        </div>
    </div>
    
    <!-- Main Content -->
    <div class="main-content" id="mainContent">
        <!-- Royal Header -->
        <div class="royal-header">
            <div class="header-floral">✦ ✦ ✦</div>
            <div class="couple-names" data-aos="fade-down">Muhamad Amirga</div>
            <div class="and-symbol" data-aos="zoom-in">&</div>
            <div class="couple-names" data-aos="fade-up">Aisyah</div>
            <div class="couple-parents" data-aos="fade-up" data-aos-delay="200">
                Putra dari Bpk. Kanta Sugianta & Ibu Simih Ade<br>
                Putri dari Bpk. Maolana Mufti & Ibu Siti Nurkhanah
            </div>
        </div>
        
        <!-- Bismillah -->
        <div class="royal-section" data-aos="fade-up">
            <div style="font-family: 'Parisienne', cursive; font-size: 36px; color: #d4af37; margin-bottom: 20px;">بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيم</div>
            <p style="font-size: 15px; line-height: 1.8; color: #fff; max-width: 350px; margin: 0 auto;">
                "Dan di antara tanda-tanda kekuasaan-Nya ialah Dia menciptakan untukmu pasangan hidup dari jenismu sendiri, supaya kamu cenderung dan merasa tenteram kepadanya, dan dijadikan-Nya di antaramu rasa kasih dan sayang."
            </p>
            <p style="margin-top: 15px; color: #d4af37;">(QS. Ar-Rum: 21)</p>
        </div>
        
        <!-- Countdown -->
		
        <div class="royal-section" data-aos="fade-up">
            <div class="section-title">Countdown</div>
            <div class="section-subtitle">MENUJU HARI BAHAGIA</div>
            
            <div class="countdown" id="countdown">
                <div class="countdown-item">
                    <div class="countdown-number" id="days">00</div>
                    <div class="countdown-label">Hari</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-number" id="hours">00</div>
                    <div class="countdown-label">Jam</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-number" id="minutes">00</div>
                    <div class="countdown-label">Menit</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-number" id="seconds">00</div>
                    <div class="countdown-label">Detik</div>
                </div>
            </div>
        </div>
        
        <!-- Save The Date -->
        <div class="royal-section" data-aos="fade-up">
            <div class="section-title">Waktu dan Tempat</div>
            
            
            <div class="royal-card">
                <div class="date-item">
                    <i class="fas fa-ring"></i>
                    <h3>Akad Nikah</h3>
                    <p>Sabtu, 5 April 2026</p>
                    <p>Pukul 10.00 - 11.00 WIB</p>
                </div>
                
                <div class="event-separator"></div>
                
                <div class="date-item">
                    <i class="fas fa-glass-cheers"></i>
                    <h3>Resepsi</h3>
                    <p>Sabtu, 5 April 2024</p>
                    <p>Pukul 11.00 - 14.00 WIB</p>
                </div>
            </div>
        </div>
        
        <!-- Location -->
        <div class="royal-section" data-aos="fade-up">
            <div class="section-title">Lokasi Acara</div>
            
            
            <div class="royal-card">
                <i class="fas fa-map-marked-alt" style="font-size: 48px; color: #d4af37; margin-bottom: 20px;"></i>
                <div class="venue-name">Pesantren Sabilunnajah Putra</div>
                <div class="venue-address">
                    Jl. Sungai Citarik II Desa, Sukamanah,<br>
                    Kec. Rancaekek, Kabupaten Bandung<br>
                    Jawa Barat 40394
                </div>
                
                <a href="https://maps.app.goo.gl/fU64CFZc71Ub9MrB9" target="_blank" class="map-button">
                    <i class="fas fa-map-marker-alt" style="margin-right: 8px;"></i>BUKA GOOGLE MAPS
                </a>
            </div>
        </div>
        
     
        
        <!-- RSVP dengan Form yang sudah terintegrasi Google Sheets -->
        <div class="royal-section" data-aos="fade-up">
            <div class="section-title">Konfirmasi Kehadiran</div>
            
            
            <div class="royal-form">
                <form id="rsvpForm" onsubmit="handleRSVP(event)">
                    <div class="form-group">
                        <label>Nama Lengkap</label>
                        <input type="text" name="nama" placeholder="Masukkan nama lengkap" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Jumlah Tamu</label>
                        <select name="jumlah" required>
                            <option value="" disabled selected>-- Pilih jumlah --</option>
                            <option value="1">1 orang</option>
                            <option value="2">2 orang</option>
                            <option value="3">3 orang</option>
                            <option value="4">4 orang</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label>Konfirmasi Kehadiran</label>
                        <select name="konfirmasi" required>
                            <option value="" disabled selected>-- Pilih konfirmasi --</option>
                            <option value="Hadir">Hadir</option>
                            <option value="Tidak Hadir">Tidak Hadir</option>
                            <option value="Ragu">Masih Ragu</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label>Pesan & Doa</label>
                        <textarea name="pesan" rows="4" placeholder="Tulis pesan dan doa untuk pengantin..."></textarea>
                    </div>
                    
                    <button type="submit" class="submit-btn">
                        <i class="fas fa-paper-plane" style="margin-right: 8px;"></i>KIRIM KONFIRMASI
                    </button>
                </form>
            </div>
        </div>
        
        <!-- Guest Book dengan List Dinamis dari Google Sheets (Hanya dari form RSVP) -->
        <div class="royal-section" data-aos="fade-up">
            <div class="section-title">Ucapan & Doa</div>
            
            
            <!-- LIST UCAPAN AKAN MUNCUL DI SINI -->
            <div id="guestbook-list" class="guestbook-list"></div>
        </div>
        
        <!-- Gift -->
	<div class="royal-section" data-aos="fade-up">
		<div class="section-title">Wedding Gift</div>
		<div class="section-subtitle">TANDA KASIH</div>
		
		<div class="royal-card">
			<i class="fas fa-gift" style="font-size: 64px; color: #d4af37; margin-bottom: 20px;"></i>
			<p style="color: #fff; margin-bottom: 25px; line-height: 1.8;">
				Doa restu Anda adalah hadiah terbaik bagi kami. 
				Namun jika ingin memberikan tanda kasih, dapat melalui:
			</p>
			
			<!-- BANK BCA -->
			<div class="rekening-item">
				<div class="rekening-header">
					<p style="color: #d4af37; font-weight: 600; margin:0;">BANK BCA</p>
				</div>
				<div class="rekening-nomor">
					<p id="rekeningBCA">5776512181</p>
					<button class="copy-btn" onclick="copyRekening('5776512181', 'BCA')">
						<i class="fas fa-copy"></i> Salin
					</button>
				</div>
				<p style="color: #fff; opacity: 0.7; margin-top: 5px;">a.n. Muhamad Amirga</p>
			</div>
			
			<!-- BANK BSI -->
			<div class="rekening-item" style="margin-top: 20px;">
				<div class="rekening-header">
					<p style="color: #d4af37; font-weight: 600; margin:0;">BANK BSI</p>
				</div>
				<div class="rekening-nomor">
					<p id="rekeningBSI">7598590160</p>
					<button class="copy-btn" onclick="copyRekening('7598590160', 'BSI')">
						<i class="fas fa-copy"></i> Salin
					</button>
				</div>
				<p style="color: #fff; opacity: 0.7; margin-top: 5px;">a.n. Maolana Mufti</p>
			</div>
		</div>
	</div>
			
			<!-- Footer -->
			<div class="royal-footer">
				<p style="max-width: 350px; margin: 0 auto; line-height: 1.8; opacity: 0.9;">
					Merupakan suatu kehormatan dan kebahagiaan bagi kami apabila Bapak/Ibu/Saudara/i berkenan hadir untuk memberikan doa restu.
				</p>
				
				<div class="footer-quote">
					Jazaakumullaahu khairan
				</div>
				
				<p style="margin: 20px 0 10px; opacity: 0.8;">Kami yang berbahagia,</p>
				<p style="font-family: 'Parisienne', cursive; font-size: 42px; color: #d4af37; margin: 15px 0;">Amirga & Aisyah</p>
				
				
			</div>
		</div>
		
		<!-- Music Player -->
		<div class="music-player">
			<button class="music-toggle" id="musicToggle" onclick="toggleMusic()">
				<i class="fas fa-music" id="musicIcon"></i>
			</button>
		</div>
		
		<audio id="bgMusic" loop>
			<source src="https://lapor.sabilunnajah.com/nasyid.mp3" type="audio/mp3">
		</audio>
		
		<script>
		
        // ===== KONFIGURASI =====
        // GANTI URL INI DENGAN URL APPS SCRIPT ANDA!
        const scriptURL = 'https://script.google.com/macros/s/AKfycbxnGFsK_nvbtdhbyuM9IV6T89pYMRK_MqrNdlY9UW7v9xMF8C_zOvJqyqAejiJLQ8Jz/exec';
        
        // ===== INIT AOS =====
        AOS.init({duration: 1000, once: true, offset: 100});
        
        // ===== BUNGA JATUH =====
        function createFlowers() {
            const container = document.getElementById('flowerContainer');
            const flowerCount = 20;
            
            for (let i = 0; i < flowerCount; i++) {
                const flower = document.createElement('div');
                flower.className = 'flower';
                flower.innerHTML = ['🌸', '🌼', '🌺', '🌹', '💮'][Math.floor(Math.random() * 5)];
                flower.style.left = Math.random() * 100 + '%';
                flower.style.fontSize = (Math.random() * 20 + 10) + 'px';
                flower.style.animationDuration = (Math.random() * 5 + 5) + 's';
                flower.style.animationDelay = Math.random() * 5 + 's';
                flower.style.opacity = Math.random() * 0.3;
                container.appendChild(flower);
            }
        }
        createFlowers();
        
        // ===== BUKA UNDANGAN =====
        function openInvitation() {
            const splash = document.getElementById('splashScreen');
            const main = document.getElementById('mainContent');
            
            splash.style.display = 'none';
            main.style.display = 'block';
            
            // Scroll ke atas
            window.scrollTo(0, 0);
            
            // Start music
            var music = document.getElementById('bgMusic');
            music.play().catch(function(error) {
                console.log("Autoplay prevented");
            });
            
            // Load ucapan
            loadGuestbook();
            
            // Trigger AOS refresh
            setTimeout(() => {
                AOS.refresh();
            }, 100);
        }
        
        // ===== KIRIM RSVP =====
        function handleRSVP(event) {
            event.preventDefault();
            
            const form = event.target;
            const submitBtn = form.querySelector('.submit-btn');
            const originalText = submitBtn.innerHTML;
            
            // Ambil data
            const nama = form.querySelector('[name="nama"]')?.value || '';
            const jumlah = form.querySelector('[name="jumlah"]')?.value || '';
            const konfirmasi = form.querySelector('[name="konfirmasi"]')?.value || '';
            const pesan = form.querySelector('[name="pesan"]')?.value || '';
            
            // Validasi
            if (!nama) {
                showNotification('Nama harus diisi', 'warning');
                return;
            }
            
            // Loading
            submitBtn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> Mengirim...';
            submitBtn.disabled = true;
            
            // Data untuk dikirim - SEMUA MASUK KE KOLOM PESAN
            const data = {
                name: nama,
                email: '',
                jumlah: jumlah,
                konfirmasi: konfirmasi,
                pesan: pesan,  // Ini yang akan tampil di list
                ucapan: ''      // Kosongkan
            };
            
            // Kirim ke Google Sheets
            fetch(scriptURL, {
                method: 'POST',
                mode: 'no-cors',
                headers: {'Content-Type': 'application/x-www-form-urlencoded'},
                body: new URLSearchParams(data)
            })
            .then(() => {
                showNotification('Terima kasih! Konfirmasi Anda telah diterima.', 'success');
                form.reset();
                setTimeout(loadGuestbook, 1000); // Reload list
            })
            .catch(() => showNotification('Gagal mengirim. Coba lagi.', 'error'))
            .finally(() => {
                submitBtn.innerHTML = originalText;
                submitBtn.disabled = false;
            });
        }
        
		// ===== FUNGSI COPY REKENING =====
function copyRekening(nomor, bank) {
    // Copy nomor ke clipboard
    navigator.clipboard.writeText(nomor).then(function() {
        // Cari tombol yang diklik
        const buttons = document.querySelectorAll('.copy-btn');
        let clickedButton = null;
        
        // Cari tombol yang sesuai dengan bank
        buttons.forEach(btn => {
            if (btn.textContent.includes('Salin') && btn.closest('.rekening-item').textContent.includes(bank)) {
                clickedButton = btn;
            }
        });
        
        if (clickedButton) {
            const originalText = clickedButton.innerHTML;
            
            // Ubah tombol jadi "Tersalin!"
            clickedButton.innerHTML = '<i class="fas fa-check"></i> Tersalin!';
            clickedButton.style.background = '#4CAF50';
            clickedButton.style.color = 'white';
            clickedButton.style.border = '1px solid #4CAF50';
            
            // Kembalikan ke semula setelah 2 detik
            setTimeout(() => {
                clickedButton.innerHTML = '<i class="fas fa-copy"></i> Salin';
                clickedButton.style.background = 'transparent';
                clickedButton.style.color = '#d4af37';
                clickedButton.style.border = '1px solid #d4af37';
            }, 2000);
        }
        
        // Tampilkan notifikasi (opsional)
        showNotification(`Nomor rekening ${bank} berhasil disalin!`, 'success');
        
    }).catch(function(err) {
        showNotification('Gagal menyalin. Coba lagi.', 'error');
    });
}
        // ===== LOAD UCAPAN DARI GOOGLE SHEETS (DARI KOLOM PESAN) =====
        async function loadGuestbook() {
            const container = document.getElementById('guestbook-list');
            if (!container) return;
            
            container.innerHTML = '<div style="text-align:center; padding:20px;"><i class="fas fa-spinner fa-spin"></i> Memuat ucapan...</div>';
            
            try {
                const response = await fetch(scriptURL + '?action=getWishes');
                const result = await response.json();
                
                if (result.result === 'success' && result.data.length > 0) {
                    let html = '';
                    
                    // Filter yang memiliki pesan (dari kolom Pesan)
                    const pesanList = result.data.filter(item => item.pesan && item.pesan.trim() !== '');
                    
                    // Tampilkan 20 pesan terbaru
                    pesanList.slice(0, 20).forEach(item => {
                        const date = new Date(item.timestamp);
                        const timeAgo = getTimeAgo(date);
                        
                        html += `
                            <div class="guestbook-item" data-aos="fade-right">
                                <div class="guestbook-name">
                                    <i class="fas fa-user" style="color:#d4af37; margin-right:8px;"></i>
                                    ${escapeHtml(item.nama || 'Tamu Undangan')}
                                </div>
                                <div class="guestbook-message">"${escapeHtml(item.pesan)}"</div>
                                <div class="guestbook-date">${timeAgo}</div>
                            </div>
                        `;
                    });
                    
                    container.innerHTML = html;
                } else {
                    container.innerHTML = '<div style="text-align:center; padding:30px; color:#999;">Belum ada ucapan. Jadilah yang pertama! ❤️</div>';
                }
            } catch (error) {
                console.error(error);
                container.innerHTML = '<div style="text-align:center; padding:20px; color:#d4af37;">Gagal memuat ucapan</div>';
            }
        }
        
        // ===== FORMAT WAKTU =====
        function getTimeAgo(date) {
            const now = new Date();
            const diffMs = now - date;
            const diffMins = Math.floor(diffMs / 60000);
            const diffHours = Math.floor(diffMs / 3600000);
            const diffDays = Math.floor(diffMs / 86400000);
            
            if (diffMins < 1) return 'Baru saja';
            if (diffMins < 60) return diffMins + ' menit lalu';
            if (diffHours < 24) return diffHours + ' jam lalu';
            if (diffDays === 1) return 'Kemarin';
            return diffDays + ' hari lalu';
        }
        
        // ===== CEK HTML INJECTION =====
        function escapeHtml(unsafe) {
            if (!unsafe) return '';
            return unsafe
                .replace(/&/g, "&amp;")
                .replace(/</g, "&lt;")
                .replace(/>/g, "&gt;")
                .replace(/"/g, "&quot;")
                .replace(/'/g, "&#039;");
        }
        
        // ===== NOTIFIKASI =====
        function showNotification(message, type = 'success') {
            const notif = document.createElement('div');
            notif.style.cssText = `
                position: fixed;
                top: 20px;
                left: 50%;
                transform: translateX(-50%);
                background: ${type === 'success' ? '#4CAF50' : type === 'error' ? '#f44336' : '#ff9800'};
                color: white;
                padding: 12px 24px;
                border-radius: 50px;
                font-size: 14px;
                z-index: 9999;
                box-shadow: 0 4px 15px rgba(0,0,0,0.2);
                animation: slideDown 0.3s ease;
                max-width: 90%;
                text-align: center;
            `;
            notif.textContent = message;
            document.body.appendChild(notif);
            
            setTimeout(() => {
                notif.style.animation = 'fadeOut 0.3s ease';
                setTimeout(() => notif.remove(), 300);
            }, 3000);
        }
        
        // ===== MUSIK =====
        let isPlaying = false;
        const music = document.getElementById('bgMusic');
        const musicIcon = document.getElementById('musicIcon');
        
        function toggleMusic() {
            if (isPlaying) {
                music.pause();
                musicIcon.classList.remove('fa-pause');
                musicIcon.classList.add('fa-music');
            } else {
                music.play();
                musicIcon.classList.remove('fa-music');
                musicIcon.classList.add('fa-pause');
            }
            isPlaying = !isPlaying;
        }
        
        // ===== COUNTDOWN =====
        function updateCountdown() {
            const weddingDate = new Date('April 5, 2026 10:00:00').getTime();
            const now = new Date().getTime();
            const distance = weddingDate - now;
            
            if (distance < 0) {
                document.getElementById('days').innerText = '00';
                document.getElementById('hours').innerText = '00';
                document.getElementById('minutes').innerText = '00';
                document.getElementById('seconds').innerText = '00';
                return;
            }
            
            const days = Math.floor(distance / (1000 * 60 * 60 * 24));
            const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((distance % (1000 * 60)) / 1000);
            
            document.getElementById('days').innerText = days.toString().padStart(2, '0');
            document.getElementById('hours').innerText = hours.toString().padStart(2, '0');
            document.getElementById('minutes').innerText = minutes.toString().padStart(2, '0');
            document.getElementById('seconds').innerText = seconds.toString().padStart(2, '0');
        }
        
        setInterval(updateCountdown, 1000);
        
        // ===== FLOATING GOLD ELEMENTS =====
        function addFloatingElements() {
            const sections = document.querySelectorAll('.royal-section');
            sections.forEach(section => {
                for (let i = 0; i < 3; i++) {
                    const gold = document.createElement('div');
                    gold.className = 'floating-gold';
                    gold.innerHTML = '✦';
                    gold.style.top = Math.random() * 100 + '%';
                    gold.style.left = Math.random() * 100 + '%';
                    gold.style.transform = `rotate(${Math.random() * 360}deg)`;
                    section.appendChild(gold);
                }
            });
        }
        addFloatingElements();
        
        // ===== CEK GUESTBOOK SAAT HALAMAN DIBUKA =====
        if (document.getElementById('mainContent').style.display === 'block') {
            loadGuestbook();
        }
    </script>
</body>
</html>
