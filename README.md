<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thảo Nguyên 11B4 | Personal Space</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Lexend:wght@300;400;600&family=Playfair+Display:ital,wght@1,700&display=swap');
        
        body {
            font-family: 'Lexend', sans-serif;
            background: #fafafa;
            scroll-behavior: smooth;
        }
        .serif { font-family: 'Playfair Display', serif; }
        .glass {
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        .gradient-text {
            background: linear-gradient(90deg, #6366f1, #ec4899);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
    </style>
</head>
<body class="text-gray-800">

    <nav class="fixed top-0 w-full z-50 glass py-4 px-6 flex justify-between items-center shadow-sm">
        <span class="font-semibold tracking-tighter text-xl">TN<span class="text-indigo-500">.</span></span>
        <div class="space-x-6 text-sm font-medium uppercase tracking-widest">
            <a href="#about" class="hover:text-indigo-500">Giới thiệu</a>
            <a href="#dreams" class="hover:text-indigo-500">Ước mơ</a>
            <a href="#contact" class="hover:text-indigo-500">Liên hệ</a>
        </div>
    </nav>

    <main class="pt-24 pb-12 px-4 max-w-4xl mx-auto space-y-20">

        <section id="about" class="text-center space-y-6 py-10">
            <div class="inline-block px-4 py-1 rounded-full bg-indigo-50 text-indigo-600 text-xs font-bold mb-4 uppercase tracking-widest">
                Welcome to my world
            </div>
            <h1 class="text-5xl md:text-7xl font-bold tracking-tighter leading-none">
                Mình là <span class="gradient-text">Lê Thảo Nguyên</span>
            </h1>
            <p class="serif text-2xl text-gray-500">Lớp 11B4 — Một người luôn kiếm tìm sự bình yên.</p>
            <div class="flex justify-center gap-4 mt-8">
                <a href="#contact" class="px-8 py-3 bg-gray-900 text-white rounded-full hover:bg-gray-800 transition shadow-lg">Liên hệ ngay</a>
                <a href="#dreams" class="px-8 py-3 border border-gray-300 rounded-full hover:bg-gray-50 transition">Khám phá ước mơ</a>
            </div>
        </section>

        <section id="dreams" class="grid md:grid-cols-2 gap-8">
            <div class="glass p-8 rounded-[2rem] shadow-xl space-y-4">
                <div class="w-12 h-12 bg-pink-100 rounded-2xl flex items-center justify-center text-pink-600">
                    <i class="fas fa-cloud-sun text-xl"></i>
                </div>
                <h2 class="text-2xl font-bold">Ước mơ tuổi 17</h2>
                <p class="text-gray-600 leading-relaxed">
                    Ước mơ của mình không cần quá lớn lao, chỉ cần đủ để mình cảm thấy hạnh phúc. Mình muốn trở thành một người có thể truyền cảm hứng thông qua ngôn ngữ và những dự án sáng tạo.
                </p>
            </div>

            <div class="glass p-8 rounded-[2rem] shadow-xl space-y-4">
                <div class="w-12 h-12 bg-indigo-100 rounded-2xl flex items-center justify-center text-indigo-600">
                    <i class="fas fa-code-branch text-xl"></i>
                </div>
                <h2 class="text-2xl font-bold">Dự án hiện tại</h2>
                <ul class="text-sm text-gray-600 space-y-2">
                    <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Xây dựng website cá nhân</li>
                    <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Học kỹ năng thiết kế cơ bản</li>
                    <li class="flex items-center"><i class="fas fa-check-circle text-green-500 mr-2"></i> Ghi lại nhật ký thanh xuân 11B4</li>
                </ul>
            </div>
        </section>

        <section id="contact" class="bg-indigo-600 rounded-[3rem] p-10 md:p-20 text-center text-white space-y-8">
            <h2 class="text-3xl md:text-5xl font-bold">Hãy cùng tạo nên điều gì đó tuyệt vời!</h2>
            <p class="text-indigo-100 text-lg">Bạn có thể tìm thấy Thảo Nguyên tại các nền tảng dưới đây.</p>
            <div class="flex justify-center gap-6 text-3xl">
                <a href="#" class="hover:scale-110 transition"><i class="fab fa-facebook"></i></a>
                <a href="#" class="hover:scale-110 transition"><i class="fab fa-instagram"></i></a>
                <a href="#" class="hover:scale-110 transition"><i class="fab fa-github"></i></a>
                <a href="#" class="hover:scale-110 transition"><i class="fas fa-envelope"></i></a>
            </div>
        </section>

    </main>

    <footer class="text-center py-10 text-gray-400 text-xs tracking-widest uppercase italic">
        Made with 🤍 by Thao Nguyen — 11B4
    </footer>

</body>
</html>
