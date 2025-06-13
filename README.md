<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elite Education - Lembaga Pendidikan Berkualitas</title>
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        /* Variabel Warna */
        :root {
            --primary: #2563eb;
            --secondary: #1e40af;
            --accent: #08c741;
            --dark: #1f2937;
            --light: #f9fafb;
        }
        
        /* Header */
        header {
            background-color: var(--primary);
            color: white;
            padding: 1rem 5%;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
        }
        
        .logo span {
            color: var(--accent);
        }
        
        .nav-links {
            display: flex;
            gap: 2rem;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--accent);
        }
        
        .cta-button {
            background-color: var(--accent);
            color: white;
            padding: 0.5rem 1.5rem;
            border-radius: 5px;
            font-weight: 600;
            transition: 0.3s;
        }
        
        .cta-button:hover {
            background-color: #e69009;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 5rem 5%;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
        }
        
        /* Program Section */
        .programs {
            padding: 5rem 5%;
            background-color: var(--light);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--dark);
        }
        
        .section-title p {
            color: #6b7280;
            max-width: 700px;
            margin: 0.5rem auto 0;
        }
        
        .program-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .program-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: 0.3s;
        }
        
        .program-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .program-img {
            height: 200px;
            background-color: #ddd;
            background-size: cover;
            background-position: center;
        }
        
        .program-content {
            padding: 1.5rem;
        }
        
        .program-content h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
            color: var(--dark);
        }
        
        .program-content p {
            color: #6b7280;
            margin-bottom: 1rem;
        }
        
        .program-price {
            font-weight: 700;
            color: var(--primary);
            font-size: 1.2rem;
            margin-bottom: 1rem;
            display: block;
        }
        
        /* Testimoni */
        .testimonials {
            padding: 5rem 5%;
            background-color: white;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .testimonial-card {
            background-color: var(--light);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .testimonial-text {
            font-style: italic;
            margin-bottom: 1rem;
            color: var(--dark);
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
            gap: 1rem;
        }
        
        .author-img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: #ddd;
        }
        
        .author-info h4 {
            color: var(--dark);
        }
        
        .author-info p {
            color: #6b7280;
            font-size: 0.9rem;
        }
        
        /* CTA Section */
        .cta-section {
            background-color: var(--primary);
            color: white;
            padding: 5rem 5%;
            text-align: center;
        }
        
        .cta-section h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .cta-section p {
            max-width: 700px;
            margin: 0 auto 2rem;
            font-size: 1.1rem;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 5% 2rem;
        }
        
        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }
        
        .footer-col h3 {
            font-size: 1.3rem;
            margin-bottom: 1rem;
            color: var(--accent);
        }
        
        .footer-col ul {
            list-style: none;
        }
        
        .footer-col ul li {
            margin-bottom: 0.5rem;
        }
        
        .footer-col ul li a {
            color: #d1d5db;
            text-decoration: none;
            transition: 0.3s;
        }
        
        .footer-col ul li a:hover {
            color: var(--accent);
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
        }
        
        .copyright {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid #374151;
            color: #9ca3af;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 1rem;
            }
            
            .nav-links {
                flex-direction: column;
                gap: 1rem;
                align-items: center;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header/Navbar -->
    <header>
        <div class="navbar">
            <div class="logo">ELITE<span>EDUCATION</span></div>
            <div class="nav-links">
                <a href="#home">Beranda</a>
                <a href="#programs">Program</a>
                <a href="#testimonials">Testimoni</a>
                <a href="#about">Tentang Kami</a>
                <a href="#contact">Kontak</a>
                <a href="#register" class="cta-button">Daftar Sekarang</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <h1>Raih Masa Depan Cerah Bersama Elite Education</h1>
        <p>Kami menyediakan program pendidikan berkualitas dengan pengajar profesional untuk membantu Anda mencapai potensi maksimal.</p>
        <a href="kuis.html.html">Simulasi Tes</a>
    </section>

    <!-- Program Section -->
    <section class="programs" id="programs">
        <div class="section-title">
            <h2>Program Pendidikan Kami</h2>
            <p>Pilih program yang sesuai dengan kebutuhan belajar Anda</p>
        </div>
        <div class="program-grid">
            <!-- Program 1 -->
            <div class="program-card">
                <div class="program-img" style="background-image: url('https://images.unsplash.com/photo-1434030216411-0b793f4b4173?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                <div class="program-content">
                    <h3>Bimbingan Belajar SD-SMP</h3>
                    <p>Program intensif untuk siswa SD dan SMP dengan kurikulum terbaik dan pengajar berpengalaman.</p>
                    <span class="program-price">Rp 480.000/bulan</span>
                    <a href="#" class="cta-button">Daftar Sekarang</a>
                </div>
            </div>
            
            <!-- Program 2 -->
            <div class="program-card">
                <div class="program-img" style="background-image: url('https://images.unsplash.com/photo-1523050854058-8df90110c9f1?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                <div class="program-content">
                    <h3>Persiapan TOEFL ITP</h3>
                    <p>Sukseskan TOEFL ITP dengan strategi belajar efektif dan try out berkala.</p>
                    <span class="program-price">mulai Rp 200.000/bulan</span>
                    <a href="#" class="cta-button">Daftar Sekarang</a>
                </div>
            </div>
            
            <!-- Program 3 -->
            <div class="program-card">
                <div class="program-img" style="background-image: url('https://images.unsplash.com/photo-1546410531-bb4caa6b424d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                <div class="program-content">
                    <h3>Kursus IELTS</h3>
                    <p>Kelas interaktif dengan pengajar berpengalaman.</p>
                    <span class="program-price">Rp 1.440.000/bulan</span>
                    <a href="#" class="cta-button">Daftar Sekarang</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimoni Section -->
    <section class="testimonials" id="testimonials">
        <div class="section-title">
            <h2>Apa Kata Mereka?</h2>
            <p>Testimoni dari siswa dan orang tua yang telah bergabung dengan kami</p>
        </div>
        <div class="testimonial-grid">
            <!-- Testimoni 1 -->
            <div class="testimonial-card">
                <p class="testimonial-text">"Anak saya mengalami peningkatan nilai yang signifikan setelah mengikuti bimbel di Elite Education. Pengajarnya sangat sabar dan metode belajarnya menyenangkan."</p>
                <div class="testimonial-author">
                    <div class="author-img"></div>
                    <div class="author-info">
                        <h4>Budi Santoso</h4>
                        <p>Orang Tua Siswa</p>
                    </div>
                </div>
            </div>
            
            <!-- Testimoni 2 -->
            <div class="testimonial-card">
                <p class="testimonial-text">"Kelas persiapan TOEFL di Elite Education sangat membantu. Materinya lengkap dan pembahasan soal-soalnya sangat detail. Berkat ini saya diterima di PTN favorit."</p>
                <div class="testimonial-author">
                    <div class="author-img"></div>
                    <div class="author-info">
                        <h4>Anita Rahma</h4>
                        <p>Siswa Kelas 12</p>
                    </div>
                </div>
            </div>
            
            <!-- Testimoni 3 -->
            <div class="testimonial-card">
                <p class="testimonial-text">"Saya bisa lebih percaya diri berbahasa Inggris setelah mengikuti kursus disini. Metode pengajarannya praktis dan tidak membosankan."</p>
                <div class="testimonial-author">
                    <div class="author-img"></div>
                    <div class="author-info">
                        <h4>Rina Wijaya</h4>
                        <p>Mahasiswa</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta-section">
        <h2>Siap Memulai Perjalanan Belajarmu?</h2>
        <p>Daftarkan diri Anda sekarang dan dapatkan diskon 20% untuk pendaftaran pertama!</p>
        <a href="#register" class="cta-button">Hubungi Kami</a>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-grid">
            <div class="footer-col">
                <h3>EduPlus</h3>
                <p>Lembaga pendidikan berkualitas dengan pengajar profesional dan kurikulum terbaik.</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-facebook"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-youtube"></i></a>
                    <a href="#"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
            <div class="footer-col">
                <h3>Program</h3>
                <ul>
                    <li><a href="#">Bimbingan Belajar</a></li>
                    <li><a href="#">Persiapan TOEFL</a></li>
                    <li><a href="#">Kursus IELTS</a></li>
                    <li><a href="#">Les Privat</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h3>Perusahaan</h3>
                <ul>
                    <li><a href="#">Tentang Kami</a></li>
                    <li><a href="#">Pengajar</a></li>
                    <li><a href="#">Karir</a></li>
                    <li><a href="#">Blog</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h3>Kontak</h3>
                <ul>
                    <li><i class="fas fa-map-marker-alt"></i> Jl. Ade Irma Nasution, Kec. Baruga, Kel. Watubangga, Kendari, SULTRA</li>
                    <li><i class="fas fa-phone"></i> 0852 8222 2739</li>
                    <li><i class="fas fa-envelope"></i> ig:elitedu7 </li>
                    <li><i class="fas fa-clock"></i> Senin-Sabtu: 08.00-17.00</li>
                </ul>
            </div>
        </div>
        <div class="copyright">
            <p>&copy; 2024 EduPlus. Semua Hak Dilindungi.</p>
        </div>
    </footer>

    <!-- Font Awesome untuk icon -->
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</body>
</html>
