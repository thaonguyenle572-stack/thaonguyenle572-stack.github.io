<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lê Thảo Nguyên | Digital Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root { --pink-soft: #fff5f8; --pink-bold: #ff80bf; --pink-dark: #d63384; --white: #ffffff; --text: #333; }
        * { box-sizing: border-box; }
        body { font-family: 'Segoe UI', sans-serif; margin: 0; background-color: var(--pink-soft); color: var(--text); scroll-behavior: smooth; }
        nav { display: flex; justify-content: space-around; align-items: center; padding: 15px 0; background: var(--white); box-shadow: 0 2px 10px rgba(0,0,0,0.05); position: sticky; top: 0; z-index: 1000; }
        nav a { color: var(--pink-dark); text-decoration: none; font-weight: bold; text-transform: uppercase; font-size: 14px; }
        .hero { height: 80vh; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; background: white; padding: 20px; }
        .hero img { width: 180px; height: 180px; border-radius: 50%; border: 8px solid var(--pink-soft); box-shadow: 0 10px 25px rgba(0,0,0,0.1); object-fit: cover; margin-bottom: 20px; }
        .hero h1 { font-size: 2.5rem; margin: 10px 0; color: var(--pink-dark); }
        .container { max-width: 800px; margin: auto; padding: 40px 20px; }
        .card { background: var(--white); border-radius: 20px; padding: 30px; box-shadow: 0 5px 20px rgba(0,0,0,0.02); margin-bottom: 40px; }
        h2 { color: var(--pink-dark); border-left: 5px solid var(--pink-bold); padding-left: 15px; margin-bottom: 25px; }
        .skill-group { margin-bottom: 20px; }
        .skill-info { display: flex; justify-content: space-between; font-weight: bold; margin-bottom: 8px; }
        .skill-bar { background: #eee; height: 12px; border-radius: 10px; overflow: hidden; }
        .skill-per { background: linear-gradient(90deg, var(--pink-bold), var(--pink-dark)); height: 100%; }
        footer { text-align: center; padding: 40px; background: #222; color: white; }
    </style>
</head> 
<body>
    <nav>
        <a href="#about">Giới thiệu</a>
        <a href="#skills">Năng lực</a>
        <a href="#contact">Liên hệ</a>
    </nav>
    <div class="hero">
        <img src="https://via.placeholder.com/180" alt="Lê Thảo Nguyên">
        <p>XIN CHÀO, MÌNH LÀ</p>
        <h1>LÊ THẢO NGUYÊN</h1>
        <p>Học sinh lớp 11 | Ninh Hòa, Khánh Hòa</p>
    </div>
    <div class="container">
        <section id="about">
            <h2>01. Giới thiệu</h2>
            <div class="card">
                <p>Mình là một người trẻ Gen Z năng động, yêu thích sáng tạo nội dung và công nghệ. Mình luôn nỗ lực để trở thành phiên bản tốt nhất của chính mình tại quê hương Ninh Hòa xinh đẹp.</p>
            </div>
        </section>
        <section id="skills">
            <h2>02. Năng lực</h2>
            <div class="card">
                <div class="skill-group">
                    <div class="skill-info"><span>Tin học & Canva</span><span>95%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 95%;"></div></div>
                </div>
                <div class="skill-group">
                    <div class="skill-info"><span>Giao tiếp</span><span>85%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 85%;"></div></div>
                </div>
            </div>
        </section>
        <section id="contact">
            <h2>03. Liên hệ</h2>
            <div class="card" style="text-align: center;">
                <p><i class="fas fa-envelope"></i> thaonguyenle2026@gmail.com</p>
                <p><i class="fas fa-map-marker-alt"></i> Ninh Hòa, Khánh Hòa</p>
            </div>
        </section>
    </div>
    <footer><p>© 2026 LÊ THẢO NGUYÊN</p></footer>
</body>
</html>
