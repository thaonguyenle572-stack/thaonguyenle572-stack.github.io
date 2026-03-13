<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lê Thảo Nguyên | Digital Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --pink-bg: #fff5f8;
            --pink-accent: #ff80bf;
            --pink-deep: #d63384;
            --white: #ffffff;
            --text: #333;
        }

        * { box-sizing: border-box; }
        body { 
            font-family: 'Segoe UI', Tahoma, sans-serif; 
            margin: 0; 
            background-color: var(--pink-bg); 
            color: var(--text); 
            scroll-behavior: smooth; 
        }

        /* --- Thanh Menu --- */
        nav { 
            display: flex; 
            justify-content: space-around; 
            align-items: center; 
            padding: 15px 0; 
            background: var(--white); 
            box-shadow: 0 2px 10px rgba(0,0,0,0.05); 
            position: sticky; 
            top: 0; 
            z-index: 1000; 
        }
        nav a { 
            color: var(--pink-deep); 
            text-decoration: none; 
            font-weight: bold; 
            text-transform: uppercase; 
            font-size: 13px; 
            letter-spacing: 1px; 
        }

        /* --- Phần Đầu Trang (Hero) --- */
        .hero { 
            height: 80vh; 
            display: flex; 
            flex-direction: column; 
            justify-content: center; 
            align-items: center; 
            text-align: center; 
            background: white; 
            padding: 20px; 
        }
        .hero img { 
            width: 170px; 
            height: 170px; 
            border-radius: 50%; 
            border: 8px solid var(--pink-bg); 
            box-shadow: 0 10px 25px rgba(0,0,0,0.1); 
            object-fit: cover; 
            margin-bottom: 20px; 
        }
        .hero h1 { font-size: 3rem; margin: 10px 0; color: var(--pink-deep); }
        .hero p { font-size: 1.2rem; color: #666; max-width: 500px; line-height: 1.6; }

        /* --- Khung Chứa Nội Dung --- */
        .container { max-width: 900px; margin: auto; padding: 60px 20px; }
        .card { 
            background: var(--white); 
            border-radius: 25px; 
            padding: 40px; 
            box-shadow: 0 10px 30px rgba(0,0,0,0.03); 
            margin-bottom: 50px; 
        }
        h2 { 
            color: var(--pink-deep); 
            font-size: 1.8rem; 
            border-left: 6px solid var(--pink-accent); 
            padding-left: 15px; 
            margin-bottom: 35px; 
            text-transform: uppercase; 
        }

        /* --- Phần Kỹ Năng (Thanh Phần Trăm) --- */
        .skill-group { margin-bottom: 25px; }
        .skill-info { display: flex; justify-content: space-between; font-weight: bold; margin-bottom: 10px; }
        .skill-bar { background: #f0f0f0; height: 14px; border-radius: 10px; overflow: hidden; }
        .skill-per { 
            background: linear-gradient(90deg, var(--pink-accent), var(--pink-deep)); 
            height: 100%; 
            border-radius: 10px; 
            transition: 1.5s; 
        }

        /* --- Phần Dự Án/Hành Trình (Có Ảnh) --- */
        .item-row { display: flex; flex-wrap: wrap; gap: 30px; margin-bottom: 40px; align-items: center; }
        .item-img { flex: 1; min-width: 300px; }
        .item-img img { width: 100%; border-radius: 20px; box-shadow: 0 8px 20px rgba(0,0,0,0.1); }
        .item-text { flex: 1.2; min-width: 300px; line-height: 1.8; }
        .item-text h3 { color: var(--pink-deep); margin-top: 0; }

        /* --- Liên Hệ --- */
        .contact-box { text-align: center; }
        .social-links { display: flex; justify-content: center; gap: 20px; margin-top: 25px; }
        .social-links a { 
            font-size: 2rem; 
            color: var(--pink-deep); 
            transition: 0.3s; 
        }
        .social-links a:hover { transform: translateY(-5px); color: var(--pink-accent); }

        footer { text-align: center; padding: 50px; background: #1a1a1a; color: white; margin-top: 50px; }
        
        @media (max-width: 600px) {
            .hero h1 { font-size: 2.2rem; }
            .item-row { flex-direction: column; }
        }
    </style>
</head>
<body>

    <nav>
        <a href="#about">Câu chuyện</a>
        <a href="#skills">Năng lực</a>
        <a href="#journey">Hành trình</a>
        <a href="#contact">Liên kết</a>
    </nav>

    <div class="hero">
        <img src="https://images.unsplash.com/photo-1529626455594-4ff0802cfb7e?auto=format&fit=crop&w=300&q=80" alt="Lê Thảo Nguyên">
        <p style="text-transform: uppercase; letter-spacing: 3px; font-weight: bold; color: var(--pink-deep);">Lớp 11 | Sáng Tạo & Đam Mê</p>
        <h1>LÊ THẢO NGUYÊN</h1>
        <p>Hành trình khám phá thế giới số của một cô gái Gen Z đến từ Ninh Hòa, Khánh Hòa.</p>
    </div>

    <div class="container">
        
        <section id="about">
            <h2>01. Về mình</h2>
            <div class="card">
                <div class="item-row">
                    <div class="item-text">
                        <p>Chào bạn! Mình là Thảo Nguyên. Một người trẻ luôn khát khao học hỏi và sáng tạo. Mình tin rằng công nghệ là cánh cửa mở ra những cơ hội tuyệt vời để chúng ta kết nối và lan tỏa giá trị tốt đẹp.</p>
                        <p>Dự án website này là bước đi đầu tiên để mình rèn luyện tư duy kỹ thuật và gu thẩm mỹ của bản thân.</p>
                    </div>
                    <div class="item-img">
                        <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?auto=format&fit=crop&w=500&q=80" alt="About Me">
                    </div>
                </div>
            </div>
        </section>

        <section id="skills">
            <h2>02. Kỹ năng nổi bật</h2>
            <div class="card">
                <div class="skill-group">
                    <div class="skill-info"><span>Thiết kế Canva & Sáng tạo nội dung</span><span>95%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 95%;"></div></div>
                </div>
                <div class="skill-group">
                    <div class="skill-info"><span>Tin học & Công nghệ</span><span>90%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 90%;"></div></div>
                </div>
                <div class="skill-group">
                    <div class="skill-info"><span>Giao tiếp & Thuyết trình</span><span>85%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 85%;"></div></div>
                </div>
            </div>
        </section>

        <section id="journey">
            <h2>03. Hành trình trải nghiệm</h2>
            <div class="card">
                <div class="item-row">
                    <div class="item-img">
                        <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=500&q=80" alt="Dự án Web">
                    </div>
                    <div class="item-text">
                        <h3>Xây dựng Portfolio</h3>
                        <p>Tự mình nghiên cứu cấu trúc web và cách triển khai trên GitHub. Đây là thử thách giúp mình hiểu hơn về thế giới lập trình.</p>
                    </div>
                </div>
                <div class="item-row" style="flex-direction: row-reverse;">
                    <div class="item-img">
                        <img src="https://images.unsplash.com/photo-1517486808906-6ca8b3f04846?auto=format&fit=crop&w=500&q=80" alt="Hoạt động">
                    </div>
                    <div class="item-text">
                        <h3>Hoạt động Cộng đồng</h3>
                        <p>Tích cực tham gia các buổi sinh hoạt tại Ninh Hòa, giúp mình kết nối với nhiều người bạn mới và học hỏi các kỹ năng sống quý báu.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact">
            <h2>04. Liên hệ & Kết nối</h2>
            <div class="card contact-box">
                <p>Bạn muốn trò chuyện hoặc hợp tác cùng mình? Đừng ngần ngại nhé!</p>
                <h3 style="color: var(--pink-deep);">thaonguyenle2026@gmail.com</h3>
                <div class="social-links">
                    <a href="#" title="Facebook"><i class="fab fa-facebook"></i></a>
                    <a href="#" title="Instagram"><i class="fab fa-instagram"></i></a>
                    <a href="#" title="TikTok"><i class="fab fa-tiktok"></i></a>
                </div>
            </div>
        </section>

    </div>

    <footer>
        <p>© 2026 LÊ THẢO NGUYÊN</p>
        <p style="font-size: 12px; opacity: 0.6;">Designed with passion in Ninh Hòa, Khánh Hòa.</p>
    </footer>

</body>
</html>


     

