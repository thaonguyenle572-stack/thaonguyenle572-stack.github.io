<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lê Thảo Nguyên | Personal Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --pink-light: #fff0f6;
            --pink-medium: #ff80bf;
            --pink-dark: #d63384;
            --white: #ffffff;
            --dark: #2d3436;
        }

        * { box-sizing: border-box; }
        body { font-family: 'Poppins', sans-serif; margin: 0; background-color: var(--pink-light); color: var(--dark); scroll-behavior: smooth; overflow-x: hidden; }

        /* --- NAVIGATION --- */
        nav { display: flex; justify-content: space-between; align-items: center; padding: 20px 8%; background: rgba(255, 255, 255, 0.95); position: sticky; top: 0; z-index: 1000; box-shadow: 0 2px 15px rgba(0,0,0,0.05); }
        .logo { font-family: 'Montserrat', sans-serif; font-weight: 700; font-size: 22px; color: var(--pink-dark); text-transform: uppercase; }
        .nav-links { display: flex; gap: 25px; }
        .nav-links a { text-decoration: none; color: var(--dark); font-weight: 600; font-size: 14px; transition: 0.3s; position: relative; }
        .nav-links a::after { content: ''; width: 0; height: 2px; background: var(--pink-dark); position: absolute; bottom: -5px; left: 0; transition: 0.3s; }
        .nav-links a:hover::after { width: 100%; }

        /* --- HERO SECTION --- */
        .hero { height: 100vh; display: flex; align-items: center; justify-content: center; padding: 0 10%; background: linear-gradient(rgba(255,255,255,0.7), rgba(255,255,255,0.7)), url('https://images.unsplash.com/photo-1494438639946-1ebd1d20bf85?auto=format&fit=crop&w=1350&q=80'); background-size: cover; background-attachment: fixed; text-align: center; }
        .hero-content { animation: fadeIn 1.5s ease-out; }
        .hero-img { width: 200px; height: 200px; border-radius: 50%; border: 10px solid var(--white); box-shadow: 0 10px 30px rgba(0,0,0,0.1); object-fit: cover; margin-bottom: 25px; }
        .hero h1 { font-family: 'Montserrat', sans-serif; font-size: 3.5rem; margin: 0; color: var(--dark); line-height: 1.1; }
        .hero span { color: var(--pink-dark); }
        .hero p { font-size: 1.2rem; margin: 20px 0 35px; color: #555; letter-spacing: 2px; text-transform: uppercase; }
        .btn { padding: 15px 35px; background: var(--pink-dark); color: white; text-decoration: none; border-radius: 50px; font-weight: bold; transition: 0.3s; box-shadow: 0 5px 15px rgba(214, 51, 132, 0.3); }
        .btn:hover { background: var(--dark); transform: scale(1.05); }

        /* --- SECTION STRUCTURE --- */
        section { padding: 100px 10%; }
        .section-title { text-align: center; margin-bottom: 60px; }
        .section-title h2 { font-size: 2.5rem; display: inline-block; position: relative; }
        .section-title h2::after { content: ''; width: 50%; height: 4px; background: var(--pink-medium); position: absolute; bottom: -10px; left: 25%; border-radius: 2px; }

        /* --- ABOUT (GIỚI THIỆU) --- */
        .about-flex { display: flex; align-items: center; gap: 50px; }
        .about-img { flex: 1; position: relative; }
        .about-img img { width: 100%; border-radius: 20px; box-shadow: 20px 20px 0 var(--pink-medium); }
        .about-text { flex: 1.5; }
        .about-text p { font-size: 1.1rem; line-height: 1.8; color: #444; }

        /* --- SKILLS (NĂNG LỰC) --- */
        .skills-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 40px; }
        .skill-card { background: var(--white); padding: 30px; border-radius: 15px; box-shadow: 0 5px 20px rgba(0,0,0,0.02); }
        .skill-item { margin-bottom: 20px; }
        .skill-name { display: flex; justify-content: space-between; font-weight: 600; margin-bottom: 8px; }
        .bar-bg { background: #eee; height: 10px; border-radius: 10px; }
        .bar-fill { background: linear-gradient(90deg, var(--pink-medium), var(--pink-dark)); height: 100%; border-radius: 10px; }

        /* --- TIMELINE (HÀNH TRÌNH) --- */
        .timeline { position: relative; max-width: 800px; margin: auto; }
        .timeline::before { content: ''; position: absolute; width: 2px; background: var(--pink-medium); top: 0; bottom: 0; left: 50%; }
        .t-item { padding: 20px 40px; position: relative; width: 50%; }
        .t-item.left { left: 0; text-align: right; }
        .t-item.right { left: 50%; text-align: left; }
        .t-content { background: var(--white); padding: 20px; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.05); }
        .t-item::after { content: ''; position: absolute; width: 16px; height: 16px; background: var(--pink-dark); border: 4px solid var(--white); border-radius: 50%; top: 25px; right: -10px; z-index: 1; }
        .t-item.right::after { left: -10px; }

        /* --- GALLERY (BỘ SƯU TẬP) --- */
        .gallery-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; }
        .gallery-item { height: 250px; overflow: hidden; border-radius: 15px; cursor: pointer; }
        .gallery-item img { width: 100%; height: 100%; object-fit: cover; transition: 0.5s; }
        .gallery-item:hover img { transform: scale(1.1) rotate(2deg); }

        /* --- CONTACT (LIÊN HỆ) --- */
        .contact-box { background: var(--white); padding: 50px; border-radius: 30px; display: flex; flex-wrap: wrap; gap: 30px; }
        .contact-info { flex: 1; min-width: 250px; }
        .contact-info div { margin-bottom: 20px; font-size: 1.1rem; }
        .contact-info i { color: var(--pink-dark); margin-right: 15px; font-size: 1.5rem; }

        footer { background: #1a1a1a; color: white; padding: 60px 10%; text-align: center; }
        .socials { margin-bottom: 20px; }
        .socials a { color: white; font-size: 25px; margin: 0 15px; transition: 0.3s; }
        .socials a:hover { color: var(--pink-medium); }

        /* ANIMATION */
        @keyframes fadeIn { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }

        @media (max-width: 768px) {
            .about-flex { flex-direction: column; }
            .timeline::before { left: 20px; }
            .t-item { width: 100%; text-align: left; padding-left: 50px; }
            .t-item.right { left: 0; }
            .t-item::after { left: 12px; }
            .hero h1 { font-size: 2.2rem; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">Nguyen.Portfolio</div>
        <div class="nav-links">
            <a href="#about">Về tui</a>
            <a href="#skills">Năng lực</a>
            <a href="#journey">Hành trình</a>
            <a href="#gallery">Hình ảnh</a>
            <a href="#contact">Liên hệ</a>
        </div>
    </nav>

    <header class="hero">
        <div class="hero-content">
            <img src="https://via.placeholder.com/200" class="hero-img" alt="Lê Thảo Nguyên">
            <h1>Xin chào, mình là<br><span>LÊ THẢO NGUYÊN</span></h1>
            <p>Sáng tạo • Đam mê • Kết nối</p>
            <a href="#contact" class="btn">LIÊN HỆ VỚI MÌNH</a>
        </div>
    </header>

    <section id="about">
        <div class="section-title"><h2>01. Về bản thân mình</h2></div>
        <div class="about-flex">
            <div class="about-img">
                <img src="https://via.placeholder.com/500x600" alt="Lê Thảo Nguyên Profile">
            </div>
            <div class="about-text">
                <p>Mình là một người trẻ đầy nhiệt huyết, hiện đang sinh sống và học tập tại <b>Ninh Hòa, Khánh Hòa</b>. Với mình, mỗi ngày trôi qua đều là một cơ hội để học hỏi những điều mới mẻ và hoàn thiện bản thân.</p>
                <p>Mình yêu thích việc sáng tạo nội dung, thiết kế những thứ xinh xắn và đặc biệt là mong muốn mang lại những giá trị tích cực cho cộng đồng thông qua các dự án cá nhân.</p>
                <p>Bản Portfolio này không chỉ là một trang web, mà là nơi lưu giữ những cột mốc và nỗ lực của mình trong hành trình trưởng thành.</p>
            </div>
        </div>
    </section>

    <section id="skills" style="background-color: #fff;">
        <div class="section-title"><h2>02. Năng lực cá nhân</h2></div>
        <div class="skills-grid">
            <div class="skill-card">
                <h3>Kỹ năng cứng</h3>
                <div class="skill-item">
                    <div class="skill-name"><span>Tin học văn phòng</span><span>90%</span></div>
                    <div class="bar-bg"><div class="bar-fill" style="width: 90%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-name"><span>Thiết kế cơ bản (Canva)</span><span>95%</span></div>
                    <div class="bar-bg"><div class="bar-fill" style="width: 95%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-name"><span>Tiếng Anh giao tiếp</span><span>75%</span></div>
                    <div class="bar-bg"><div class="bar-fill" style="width: 75%;"></div></div>
                </div>
            </div>
            <div class="skill-card">
                <h3>Kỹ năng mềm</h3>
                <div class="skill-item">
                    <div class="skill-name"><span>Làm việc nhóm</span><span>95%</span></div>
                    <div class="bar-bg"><div class="bar-fill" style="width: 95%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-name"><span>Giao tiếp thuyết trình</span><span>85%</span></div>
                    <div class="bar-bg"><div class="bar-fill" style="width: 85%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-name"><span>Giải quyết vấn đề</span><span>80%</span></div>
                    <div class="bar-bg"><div class="bar-fill" style="width: 80%;"></div></div>
                </div>
            </div>
        </div>
    </section>

    <section id="journey">
        <div class="section-title"><h2>03. Hành trình phát triển</h2></div>
        <div class="timeline">
            <div class="t-item left">
                <div class="t-content">
                    <h4>Năm 2024</h4>
                    <p>Bắt đầu xây dựng những dự án cá nhân đầu tiên và học cách thiết kế website.</p>
                </div>
            </div>
            <div class="t-item right">
                <div class="t-content">
                    <h4>Năm 2025</h4>
                    <p>Tham gia các hoạt động ngoại khóa tại Ninh Hòa để rèn luyện kỹ năng xã hội.</p>
                </div>
            </div>
            <div class="t-item left">
                <div class="t-content">
                    <h4>Tương lai 2026</h4>
                    <p>Hoàn thành những mục tiêu lớn về học tập và định hướng sự nghiệp rõ ràng.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="gallery" style="background-color: #fff;">
        <div class="section-title"><h2>04. Khoảnh khắc & Kỷ niệm</h2></div>
        <div class="gallery-grid">
            <div class="gallery-item"><img src="https://via.placeholder.com/400x400" alt="Hinh 1"></div>
            <div class="gallery-item"><img src="https://via.placeholder.com/400x400" alt="Hinh 2"></div>
            <div class="gallery-item"><img src="https://via.placeholder.com/400x400" alt="Hinh 3"></div>
            <div class="gallery-item"><img src="https://via.placeholder.com/400x400" alt="Hinh 4"></div>
            <div class="gallery-item"><img src="https://via.placeholder.com/400x400" alt="Hinh 5"></div>
            <div class="gallery-item"><img src="https://via.placeholder.com/400x400" alt="Hinh 6"></div>
        </div>
    </section>

    <section id="contact">
        <div class="section-title"><h2>05. Kết nối với mình</h2></div>
        <div class="contact-box">
            <div class="contact-info">
                <h3>Thông tin liên hệ</h3>
                <div><i class="fas fa-envelope"></i> thaonguyenle2026@gmail.com</div>
                <div><i class="fas fa-map-marker-alt"></i> Ninh Hòa, Khánh Hòa, Việt Nam</div>
                <div><i class="fas fa-phone"></i> +84 XXX XXX XXX</div>
            </div>
            <div style="flex: 1; text-align: center;">
                <p>Mình luôn sẵn sàng để làm quen và hợp tác với các bạn!</p>
                <div class="socials" style="margin-top: 30px;">
                    <a href="#"><i class="fab fa-facebook"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-github"></i></a>
                    <a href="#"><i class="fab fa-tiktok"></i></a>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <p>© 2026 LÊ THẢO NGUYÊN</p>
        <p style="font-size: 13px; color: #888;">Trang web được thiết kế bằng tất cả sự chân thành.</p>
    </footer>

</body>
</html>
