<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lê Thảo Nguyên | Digital Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --pink-soft: #fff5f8;
            --pink-bold: #ff80bf;
            --pink-dark: #d63384;
            --white: #ffffff;
            --text: #333;
        }

        * { box-sizing: border-box; }
        body { font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; background-color: var(--pink-soft); color: var(--text); scroll-behavior: smooth; }

        /* --- Menu ngang --- */
        nav { display: flex; justify-content: space-around; align-items: center; padding: 15px 0; background: var(--white); box-shadow: 0 2px 10px rgba(0,0,0,0.05); position: sticky; top: 0; z-index: 1000; }
        nav a { color: var(--pink-dark); text-decoration: none; font-weight: bold; text-transform: uppercase; font-size: 14px; }

        /* --- Phần Banner (Hero) --- */
        .hero { height: 100vh; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; background: linear-gradient(135deg, #fff 0%, var(--pink-soft) 100%); padding: 20px; }
        .hero img { width: 180px; height: 180px; border-radius: 50%; border: 8px solid white; box-shadow: 0 10px 25px rgba(0,0,0,0.1); object-fit: cover; margin-bottom: 20px; }
        .hero h1 { font-size: 3rem; margin: 10px 0; color: var(--pink-dark); }
        .hero p { font-size: 1.2rem; color: #777; margin-bottom: 30px; }

        /* --- Nội dung chính --- */
        .container { max-width: 900px; margin: auto; padding: 60px 20px; }
        .card { background: var(--white); border-radius: 20px; padding: 40px; box-shadow: 0 5px 20px rgba(0,0,0,0.02); margin-bottom: 50px; }
        
        h2 { color: var(--pink-dark); font-size: 2rem; border-left: 6px solid var(--pink-bold); padding-left: 15px; margin-bottom: 30px; text-transform: uppercase; }

        /* --- 1. Giới thiệu --- */
        .about-content { display: flex; flex-wrap: wrap; gap: 30px; align-items: center; }
        .about-text { flex: 1; min-width: 300px; line-height: 1.8; font-size: 1.1rem; }
        .about-img { flex: 1; min-width: 300px; border-radius: 15px; width: 100%; box-shadow: 10px 10px 0 var(--pink-bold); }

        /* --- 2. Năng lực (Có thanh phần trăm) --- */
        .skill-group { margin-bottom: 25px; }
        .skill-info { display: flex; justify-content: space-between; font-weight: bold; margin-bottom: 10px; font-size: 1.1rem; }
        .skill-bar { background: #eee; height: 15px; border-radius: 10px; overflow: hidden; }
        .skill-per { background: linear-gradient(90deg, var(--pink-bold), var(--pink-dark)); height: 100%; border-radius: 10px; }

        /* --- 3. Dự án (Dài & Nhiều ý) --- */
        .project-box { border-bottom: 1px solid #eee; padding-bottom: 30px; margin-bottom: 30px; }
        .project-box:last-child { border-bottom: none; }
        .project-title { font-size: 1.4rem; font-weight: bold; color: var(--pink-dark); margin-bottom: 15px; display: flex; align-items: center; gap: 10px; }
        .project-desc { display: flex; flex-wrap: wrap; gap: 20px; }
        .project-desc img { width: 100%; max-width: 300px; border-radius: 10px; }
        .project-text { flex: 1; min-width: 250px; line-height: 1.6; }

        /* --- 4. Liên hệ --- */
        .contact-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; text-align: center; }
        .contact-item { padding: 20px; background: var(--pink-soft); border-radius: 15px; transition: 0.3s; }
        .contact-item:hover { transform: translateY(-5px); }
        .contact-item i { font-size: 2rem; color: var(--pink-dark); margin-bottom: 10px; }

        footer { text-align: center; padding: 50px; background: #222; color: white; margin-top: 50px; }

        @media (max-width: 600px) { .hero h1 { font-size: 2.2rem; } }
    </style>
</head>
<body>

    <nav>
        <a href="#about">Giới thiệu</a>
        <a href="#skills">Năng lực</a>
        <a href="#projects">Dự án</a>
        <a href="#contact">Liên hệ</a>
    </nav>

    <div class="hero">
        <img src="https://via.placeholder.com/180" alt="Lê Thảo Nguyên">
        <p>XIN CHÀO, MÌNH LÀ</p>
        <h1>LÊ THẢO NGUYÊN</h1>
        <p>Học sinh lớp 11 | Nhà sáng tạo nội dung tương lai</p>
    </div>

    <div class="container">
        
        <section id="about">
            <h2>01. Giới thiệu bản thân</h2>
            <div class="card about-content">
                <div class="about-text">
                    <p>Mình là Thảo Nguyên, hiện đang theo học tại <b>Ninh Hòa, Khánh Hòa</b>. Mình là một người yêu thích sự sáng tạo và luôn muốn khám phá những điều mới mẻ trong cuộc sống.</p>
                    <p>Phương châm sống của mình là: "Mọi nỗ lực hôm nay đều là nền móng cho thành công ngày mai". Mình không ngừng học hỏi để hoàn thiện bản thân mỗi ngày.</p>
                </div>
                <img src="https://via.placeholder.com/400x250" class="about-img" alt="Hình ảnh giới thiệu">
            </div>
        </section>

        <section id="skills">
            <h2>02. Năng lực & Kỹ năng</h2>
            <div class="card">
                <div class="skill-group">
                    <div class="skill-info"><span>Kỹ năng Tin học (Word, Canva)</span><span>95%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 95%;"></div></div>
                </div>
                <div class="skill-group">
                    <div class="skill-info"><span>Kỹ năng Giao tiếp</span><span>85%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 85%;"></div></div>
                </div>
                <div class="skill-group">
                    <div class="skill-info"><span>Làm việc nhóm</span><span>90%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 90%;"></div></div>
                </div>
                <div class="skill-group">
                    <div class="skill-info"><span>Tiếng Anh cơ bản</span><span>80%</span></div>
                    <div class="skill-bar"><div class="skill-per" style="width: 80%;"></div></div>
                </div>
            </div>
        </section>

        <section id="projects">
            <h2>03. Dự án & Trải nghiệm</h2>
            <div class="card">
                <div class="project-box">
                    <div class="project-title"><i class="fas fa-code"></i> Dự án Website Cá nhân</div>
                    <div class="project-desc">
                        <img src="https://via.placeholder.com/300x180" alt="Website dự án">
                        <div class="project-text">
                            <p>Tự tay thiết kế và xây dựng giao diện Portfolio trực tuyến bằng ngôn ngữ HTML/CSS để giới thiệu bản thân.</p>
                            <p><b>Kết quả:</b> Hoàn thành trang web mượt mà, thể hiện được phong cách cá nhân.</p>
                        </div>
                    </div>
                </div>
                <div class="project-box">
                    <div class="project-title"><i class="fas fa-users"></i> Hoạt động Ngoại khóa</div>
                    <div class="project-desc">
                        <img src="https://via.placeholder.com/300x180" alt="Hoạt động">
                        <div class="project-text">
                            <p>Tham gia các chương trình tình nguyện và sinh hoạt hè tại địa phương, giúp đỡ cộng đồng và rèn luyện kỹ năng mềm.</p>
                            <p><b>Kết quả:</b> Nhận được nhiều giấy chứng nhận và sự tin yêu từ mọi người.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact">
            <h2>04. Liên hệ liên kết</h2>
            <div class="card contact-grid">
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <p>Email</p>
                    <span style="font-size: 13px;">thaonguyenle2026@gmail.com</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <p>Địa chỉ</p>
                    <span>Ninh Hòa, Khánh Hòa</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-phone"></i>
                    <p>Điện thoại</p>
                    <span>+84 XXX XXX XXX</span>
                </div>
            </div>
        </section>

    </div>

    <footer>
        <p>© 2026 LÊ THẢO NGUYÊN - DESIGNED WITH 💖</p>
    </footer>

</body>
</html>
