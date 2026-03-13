<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lê Thảo Nguyên | Personal Portfolio</title>
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

        /* --- Navigation --- */
        nav { display: flex; justify-content: space-around; align-items: center; padding: 20px 0; background: var(--white); box-shadow: 0 2px 15px rgba(0,0,0,0.05); position: sticky; top: 0; z-index: 1000; }
        nav a { color: var(--pink-dark); text-decoration: none; font-weight: bold; text-transform: uppercase; font-size: 14px; letter-spacing: 1px; transition: 0.3s; }
        nav a:hover { color: var(--pink-bold); }

        /* --- Hero Section --- */
        .hero { height: 90vh; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; background: white; padding: 20px; border-bottom: 5px solid var(--pink-soft); }
        .hero img { width: 180px; height: 180px; border-radius: 50%; border: 10px solid var(--pink-soft); box-shadow: 0 15px 35px rgba(0,0,0,0.1); object-fit: cover; margin-bottom: 25px; }
        .hero h1 { font-size: 3.5rem; margin: 10px 0; color: var(--pink-dark); letter-spacing: -2px; }
        .hero p { font-size: 1.3rem; color: #666; max-width: 600px; line-height: 1.6; }

        /* --- Main Container --- */
        .container { max-width: 1000px; margin: auto; padding: 80px 20px; }
        .card { background: var(--white); border-radius: 30px; padding: 50px; box-shadow: 0 10px 40px rgba(0,0,0,0.03); margin-bottom: 60px; }
        
        h2 { color: var(--pink-dark); font-size: 2.2rem; border-left: 8px solid var(--pink-bold); padding-left: 20px; margin-bottom: 40px; text-transform: uppercase; }

        /* --- Section 01: Giới thiệu --- */
        .about-flex { display: flex; flex-wrap: wrap; gap: 40px; align-items: center; }
        .about-text { flex: 1.2; min-width: 300px; line-height: 1.9; font-size: 1.1rem; }
        .about-img { flex: 0.8; min-width: 300px; border-radius: 20px; width: 100%; box-shadow: 15px 15px 0 var(--pink-bold); }

        /* --- Section 02: Kỹ năng --- */
        .skills-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); gap: 30px; }
        .skill-group { margin-bottom: 30px; }
        .skill-info { display: flex; justify-content: space-between; font-weight: bold; margin-bottom: 12px; font-size: 1.1rem; }
        .skill-bar { background: #f0f0f0; height: 18px; border-radius: 20px; overflow: hidden; }
        .skill-per { background: linear-gradient(90deg, var(--pink-bold), var(--pink-dark)); height: 100%; border-radius: 20px; }

        /* --- Section 03: Dự án/Hành trình (Có ảnh) --- */
        .project-item { display: flex; flex-wrap: wrap; gap: 30px; padding-bottom: 50px; margin-bottom: 50px; border-bottom: 1px solid #eee; }
        .project-item:last-child { border-bottom: none; }
        .project-img { flex: 1; min-width: 300px; }
        .project-img img { width: 100%; border-radius: 15px; box-shadow: 0 5px 20px rgba(0,0,0,0.1); }
        .project-info { flex: 1.5; min-width: 300px; }
        .project-info h3 { color: var(--pink-dark); font-size: 1.6rem; margin-top: 0; }
        .project-info p { line-height: 1.8; color: #555; }

        /* --- Section 04: Liên hệ --- */
        .contact-box { text-align: center; }
        .social-icons { display: flex; justify-content: center; gap: 25px; margin-top: 30px; }
        .social-icons a { font-size: 2.5rem; color: var(--pink-dark); transition: 0.3s; }
        .social-icons a:hover { transform: scale(1.2); color: var(--pink-bold); }

        footer { text-align: center; padding: 80px 20px; background: #1a1a1a; color: white; }
        footer p { margin: 5px 0; opacity: 0.8; }

        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            .about-flex, .project-item { flex-direction: column; }
        }
    </style>
</head>
<body>

    <nav>
        <a href="#about">Về mình</a>
        <a href="#skills">Kỹ năng</a>
        <a href="#projects">Hành trình</a>
        <a href="#contact">Kết nối</a>
    </nav>

    <div class="hero">
        <img src="https://via.placeholder.com/180" alt="Lê Thảo Nguyên">
        <p style="text-transform: uppercase; letter-spacing: 5px; color: var(--pink-dark); font-weight: bold; margin-bottom: 10px;">Personal Portfolio</p>
        <h1>LÊ THẢO NGUYÊN</h1>
        <p>Gen Z Creative | Digital Content Creator | Tech Enthusiast <br> Ninh Hòa, Khánh Hòa</p>
    </div>

    <div class="container">
        
        <section id="about">
            <h2>01. Câu chuyện của mình</h2>
            <div class="card about-flex">
                <div class="about-text">
                    <p>Xin chào! Mình là <b>Thảo Nguyên</b>. Hiện tại mình đang theo học tại <b>Ninh Hòa, Khánh Hòa</b>. Ngay từ nhỏ, mình đã có một sự tò mò vô hạn với thế giới kỹ thuật số và những cách thức mà công nghệ kết nối con người lại với nhau.</p>
                    <p>Mình không chỉ coi công nghệ là một công cụ, mà là một mảnh đất để mình gieo mầm những ý tưởng sáng tạo. Mục tiêu của mình là trở thành một người sáng tạo nội dung có sức ảnh hưởng, mang lại những giá trị tích cực và truyền cảm hứng cho cộng đồng trẻ.</p>
                    <p>Bản Portfolio này là nơi mình ghi dấu những nỗ lực, sự học hỏi và cả những niềm vui trong quá trình hoàn thiện bản thân mỗi ngày.</p>
                </div>
                <img src="https://via.placeholder.com/450x300" class="about-img" alt="Hình ảnh giới thiệu">
            </div>
        </section>

        <section id="skills">
            <h2>02. Năng lực cá nhân</h2>
            <div class="card">
                <div class="skills-grid">
                    <div class="skill-group">
                        <div class="skill-info"><span>Thiết kế Đồ họa (Canva/Design)</span><span>95%</span></div>
                        <div class="skill-bar"><div class="skill-per" style="width: 95%;"></div></div>
                    </div>
                    <div class="skill-group">
                        <div class="skill-info"><span>Sáng tạo nội dung số</span><span>90%</span></div>
                        <div class="skill-bar"><div class="skill-per" style="width: 90%;"></div></div>
                    </div>
                    <div class="skill-group">
                        <div class="skill-info"><span>Tin học & Công nghệ</span><span>95%</span></div>
                        <div class="skill-bar"><div class="skill-per" style="width: 95%;"></div></div>
                    </div>
                    <div class="skill-group">
                        <div class="skill-info"><span>Tiếng Anh giao tiếp</span><span>85%</span></div>
                        <div class="skill-bar"><div class="skill-per" style="width: 85%;"></div></div>
                    </div>
                </div>
                <p style="margin-top: 20px; font-style: italic; color: #888; text-align: center;">Ngoài ra, mình còn sở hữu các kỹ năng mềm như: Làm việc nhóm, Giao tiếp thuyết trình và Giải quyết vấn đề một cách sáng tạo.</p>
            </div>
        </section>

        <section id="projects">
            <h2>03. Hành trình & Dự án tiêu biểu</h2>
            <div class="card">
                <div class="project-item">
                    <div class="project-img">
                        <img src="https://via.placeholder.com/400x250" alt="Dự án Website">
                    </div>
                    <div class="project-info">
                        <h3>Thiết kế Portfolio Cá nhân</h3>
                        <p>Đây là dự án tâm huyết nhất của mình trong năm 2026. Mình đã tự tay nghiên cứu các cấu trúc HTML/CSS để tạo ra một không gian số thể hiện đúng tính cách của bản thân.</p>
                        <p><b>Thành quả:</b> Một trang web mượt mà, tối ưu hóa trên điện thoại và nhận được nhiều lời khen từ bạn bè.</p>
                    </div>
                </div>

                <div class="project-item">
                    <div class="project-img">
                        <img src="https://via.placeholder.com/400x250" alt="Dự án Sáng tạo">
                    </div>
                    <div class="project-info">
                        <h3>Sáng tạo nội dung đa phương tiện</h3>
                        <p>Mình thường xuyên thực hiện các bộ ảnh chân dung và video ngắn để lưu lại những khoảnh khắc đẹp tại Ninh Hòa. Qua đó, mình học được cách phối màu, dựng video và kể chuyện bằng hình ảnh.</p>
                        <p><b>Thành quả:</b> Xây dựng được phong cách cá nhân riêng biệt trên các nền tảng mạng xã hội.</p>
                    </div>
                </div>

                <div class="project-item">
                    <div class="project-img">
                        <img src="https://via.placeholder.com/400x250" alt="Hoạt động xã hội">
                    </div>
                    <div class="project-info">
                        <h3>Kết nối Cộng đồng trẻ</h3>
                        <p>Tham gia và tổ chức các hoạt động ngoại khóa tại trường, giúp mình rèn luyện kỹ năng lãnh đạo và kết nối mọi người lại với nhau để cùng thực hiện những mục tiêu chung.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact">
            <h2>04. Kết nối cùng mình</h2>
            <div class="card contact-box">
                <p>Mình luôn sẵn sàng cho những cơ hội mới, những cuộc trò chuyện thú vị và những sự hợp tác đầy cảm hứng. Đừng ngần ngại liên hệ với mình qua các kênh dưới đây nhé!</p>
                <div style="font-size: 1.2rem; margin: 20px 0;">
                    <p><i class="fas fa-envelope"></i> <b>thaonguyenle2026@gmail.com</b></p>
                    <p><i class="fas fa-map-marker-alt"></i> <b>Ninh Hòa, Khánh Hòa, Việt Nam</b></p>
                </div>
                <div class="social-icons">
                    <a href="#"><i class="fab fa-facebook"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-tiktok"></i></a>
                    <a href="#"><i class="fab fa-github"></i></a>
                </div>
            </div>
        </section>

    </div>

    <footer>
        <p><b>LÊ THẢO NGUYÊN</b></p>
        <p>© 2026 All Rights Reserved.</p>
        <p style="font-size: 13px; color: #888;">Trang web được thiết kế bằng tất cả sự đam mê và nhiệt huyết.</p>
    </footer>

</body>
</html>

