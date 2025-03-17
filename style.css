<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sağlıklı Yaşam</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f9fc;
            color: #333;
        }
        
        header {
            background-color: #4CAF50;
            color: white;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        nav {
            background-color: #388E3C;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
        }
        
        nav ul li {
            position: relative;
        }
        
        nav ul li a {
            display: block;
            color: white;
            text-decoration: none;
            padding: 15px 20px;
            transition: background-color 0.3s;
        }
        
        nav ul li a:hover {
            background-color: #2E7D32;
        }
        
        .dropdown-content {
            display: none;
            position: absolute;
            background-color: #f9f9f9;
            min-width: 200px;
            box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
            z-index: 1;
        }
        
        .dropdown-content a {
            color: #333;
            padding: 12px 16px;
            text-decoration: none;
            display: block;
            text-align: left;
        }
        
        .dropdown-content a:hover {
            background-color: #ddd;
            color: #333;
        }
        
        .dropdown:hover .dropdown-content {
            display: block;
        }
        
        .hero {
            background-image: url('/api/placeholder/1200/400');
            background-size: cover;
            background-position: center;
            height: 400px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-align: center;
            position: relative;
            margin-bottom: 40px;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.4);
        }
        
        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 800px;
            padding: 20px;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: #4CAF50;
            color: white;
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
        }
        
        .btn:hover {
            background-color: #388E3C;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
            padding-bottom: 15px;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: #4CAF50;
        }
        
        .categories {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 50px;
        }
        
        .category-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }
        
        .category-card:hover {
            transform: translateY(-10px);
        }
        
        .category-img {
            height: 200px;
            overflow: hidden;
        }
        
        .category-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .category-card:hover .category-img img {
            transform: scale(1.1);
        }
        
        .category-content {
            padding: 20px;
        }
        
        .category-content h3 {
            margin-bottom: 15px;
            color: #388E3C;
        }
        
        .accordion {
            margin-bottom: 50px;
        }
        
        .accordion-item {
            background-color: white;
            margin-bottom: 15px;
            border-radius: 5px;
            overflow: hidden;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        
        .accordion-header {
            padding: 15px 20px;
            background-color: #f1f1f1;
            cursor: pointer;
            position: relative;
            user-select: none;
        }
        
        .accordion-header h3 {
            font-size: 1.1rem;
            font-weight: 600;
        }
        
        .accordion-header::after {
            content: '+';
            position: absolute;
            right: 20px;
            top: 50%;
            transform: translateY(-50%);
            font-size: 1.5rem;
            transition: transform 0.3s;
        }
        
        .accordion-item.active .accordion-header::after {
            content: '-';
        }
        
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
        }
        
        .accordion-item.active .accordion-content {
            max-height: 500px;
        }
        
        .accordion-body {
            padding: 20px;
            line-height: 1.6;
        }
        
        .testimonials {
            margin-bottom: 50px;
            position: relative;
        }
        
        .testimonial-container {
            display: flex;
            overflow-x: hidden;
            scroll-behavior: smooth;
            padding: 20px 0;
        }
        
        .testimonial {
            min-width: 100%;
            padding: 20px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }
        
        .testimonial-img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            overflow: hidden;
            margin-bottom: 20px;
            border: 5px solid #4CAF50;
        }
        
        .testimonial-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .testimonial p {
            font-style: italic;
            margin-bottom: 20px;
            line-height: 1.6;
        }
        
        .slider-nav {
            display: flex;
            justify-content: center;
            margin-top: 20px;
        }
        
        .slider-dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background-color: #ddd;
            margin: 0 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        .slider-dot.active {
            background-color: #4CAF50;
        }
        
        .newsletter {
            background-color: #4CAF50;
            padding: 50px 0;
            color: white;
            text-align: center;
        }
        
        .newsletter h2 {
            margin-bottom: 20px;
        }
        
        .newsletter p {
            margin-bottom: 30px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .newsletter-form {
            display: flex;
            max-width: 500px;
            margin: 0 auto;
        }
        
        .newsletter-form input {
            flex: 1;
            padding: 15px;
            border: none;
            border-radius: 30px 0 0 30px;
            outline: none;
        }
        
        .newsletter-form button {
            padding: 15px 25px;
            background-color: #333;
            color: white;
            border: none;
            border-radius: 0 30px 30px 0;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        .newsletter-form button:hover {
            background-color: #222;
        }
        
        footer {
            background-color: #333;
            color: white;
            padding: 40px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .footer-section h3 {
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-section h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 2px;
            background-color: #4CAF50;
        }
        
        .footer-section ul {
            list-style: none;
        }
        
        .footer-section ul li {
            margin-bottom: 10px;
        }
        
        .footer-section ul li a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-section ul li a:hover {
            color: #4CAF50;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: #4CAF50;
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #444;
        }
        
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
            }
            
            .dropdown-content {
                position: static;
                box-shadow: none;
                max-height: 0;
                overflow: hidden;
                transition: max-height 0.3s;
            }
            
            .dropdown:hover .dropdown-content {
                max-height: 500px;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .newsletter-form {
                flex-direction: column;
            }
            
            .newsletter-form input {
                border-radius: 30px;
                margin-bottom: 10px;
            }
            
            .newsletter-form button {
                border-radius: 30px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Sağlıklı Yaşam</h1>
            <p>Daha sağlıklı ve mutlu bir yaşam için bilgi kaynağınız</p>
        </div>
    </header>
    
    <nav>
        <ul>
            <li><a href="#anasayfa">Ana Sayfa</a></li>
            <li class="dropdown">
                <a href="#beslenme">Beslenme</a>
                <div class="dropdown-content">
                    <a href="#">Sağlıklı Tarifler</a>
                    <a href="#">Diyet Planları</a>
                    <a href="#">Vitamin ve Mineraller</a>
                    <a href="#">Gıda Takviyeleri</a>
                </div>
            </li>
            <li class="dropdown">
                <a href="#egzersiz">Egzersiz</a>
                <div class="dropdown-content">
                    <a href="#">Kardiyo Egzersizleri</a>
                    <a href="#">Güç Antrenmanı</a>
                    <a href="#">Esneklik ve Yoga</a>
                    <a href="#">Ev Egzersizleri</a>
                </div>
            </li>
            <li class="dropdown">
                <a href="#zihinsel-saglik">Zihinsel Sağlık</a>
                <div class="dropdown-content">
                    <a href="#">Stres Yönetimi</a>
                    <a href="#">Meditasyon</a>
                    <a href="#">Uyku Düzeni</a>
                    <a href="#">Pozitif Düşünce</a>
                </div>
            </li>
            <li><a href="#blog">Blog</a></li>
            <li><a href="#iletisim">İletişim</a></li>
        </ul>
    </nav>
    
    <section class="hero" id="anasayfa">
        <div class="hero-content">
            <h1>Sağlıklı Yaşamın Anahtarları</h1>
            <p>Sağlıklı beslenme, düzenli egzersiz ve zihinsel sağlık önerileriyle daha enerjik ve mutlu bir yaşama adım atın.</p>
            <a href="#" class="btn">Daha Fazla Bilgi</a>
        </div>
    </section>
    
    <section class="container">
        <h2 class="section-title">Sağlıkl
