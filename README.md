<html>
  <H1>으이아의 홈페이지</H1>
</html>
[응이아.html](https://github.com/user-attachments/files/33028070/default.html)
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>응이아 - Personal Space</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Font - Inter & Noto Sans KR -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&family=Noto+Sans+KR:wght@300;400;500;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Noto Sans KR', 'Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#eef2ff',
                            100: '#e0e7ff',
                            500: '#6366f1',
                            600: '#4f46e5',
                            700: '#4338ca',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .glass-card {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.4);
        }
        
        .gradient-bg {
            background: linear-gradient(-45deg, #0f172a, #1e1b4b, #311042, #0f172a);
            background-size: 400% 400%;
            animation: gradientMove 15s ease infinite;
        }

        @keyframes gradientMove {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .card-hover {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .card-hover:hover {
            transform: translateY(-6px) scale(1.01);
            box-shadow: 0 20px 30px -10px rgba(0, 0, 0, 0.3);
        }
    </style>
</head>
<body class="gradient-bg min-h-screen text-slate-100 font-sans flex flex-col justify-between antialiased selection:bg-indigo-500 selection:text-white">

    <!-- Background Animated Glowing Blobs -->
    <div class="fixed inset-0 overflow-hidden pointer-events-none z-0">
        <div class="absolute -top-40 -left-40 w-96 h-96 bg-purple-500/20 rounded-full blur-3xl animate-pulse"></div>
        <div class="absolute top-1/2 -right-40 w-96 h-96 bg-indigo-500/20 rounded-full blur-3xl animate-pulse delay-1000"></div>
        <div class="absolute -bottom-40 left-1/3 w-96 h-96 bg-blue-500/20 rounded-full blur-3xl animate-pulse delay-700"></div>
    </div>

    <div class="relative z-10 flex-grow flex flex-col items-center justify-center px-4 py-12 sm:px-6 lg:px-8">
        
        <!-- Profile Header Section -->
        <header class="text-center max-w-2xl w-full mb-12 transform transition-all duration-500">
            <!-- Profile Avatar / Badge -->
            <div class="inline-block relative mb-6">
                <div class="w-28 h-28 sm:w-32 sm:h-32 rounded-full p-1 bg-gradient-to-tr from-indigo-500 via-purple-500 to-pink-500 shadow-xl">
                    <div class="w-full h-full bg-slate-900 rounded-full flex items-center justify-center overflow-hidden border-2 border-slate-800">
                        <span class="text-4xl sm:text-5xl font-extrabold bg-gradient-to-r from-indigo-400 via-purple-300 to-pink-400 bg-clip-text text-transparent">
                            응
                        </span>
                    </div>
                </div>
                <div class="absolute bottom-1 right-1 bg-emerald-500 w-5 h-5 rounded-full border-2 border-slate-900" title="Active"></div>
            </div>

            <!-- Title & Subtitle -->
            <h1 class="text-4xl sm:text-5xl font-black tracking-tight text-white mb-3">
                응이아
            </h1>
            <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-white/10 backdrop-blur-md border border-white/15 text-indigo-200 text-sm sm:text-base font-medium shadow-inner">
                <i class="fa-solid font-normal fa-graduation-cap text-indigo-400"></i>
                <span>연성대학교 경영학과 2학년</span>
            </div>
        </header>

        <!-- Navigation Link Cards -->
        <main class="w-full max-w-xl space-y-5">
            
            <!-- Card 1: TOPIK -->
            <a href="https://www.topik.go.kr/TWSTDY/TWSTDY0210.do" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="group block card-hover glass-card rounded-2xl p-5 shadow-lg border border-white/20 transition-all duration-300">
                <div class="flex items-center justify-between">
                    <div class="flex items-center space-x-4">
                        <div class="w-12 h-12 rounded-xl bg-indigo-600/20 text-indigo-400 flex items-center justify-center group-hover:bg-indigo-600 group-hover:text-white transition-colors duration-300">
                            <i class="fa-solid fa-book-open text-xl"></i>
                        </div>
                        <div>
                            <h2 class="text-lg font-bold text-slate-800 group-hover:text-indigo-600 transition-colors">
                                토픽 공부하자
                            </h2>
                            <p class="text-xs sm:text-sm text-slate-500 font-medium">
                                TOPIK 한국어능력시험 공부 자료
                            </p>
                        </div>
                    </div>
                    <div class="text-slate-400 group-hover:text-indigo-600 group-hover:translate-x-1 transition-all">
                        <i class="fa-solid fa-arrow-up-right-from-square text-lg"></i>
                    </div>
                </div>
            </a>

            <!-- Card 2: Exercise/Hobby -->
            <a href="https://www.somoim.co.kr/%EC%9A%B4%EB%8F%99-%EC%8A%A4%ED%8F%AC%EC%B8%A0" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="group block card-hover glass-card rounded-2xl p-5 shadow-lg border border-white/20 transition-all duration-300">
                <div class="flex items-center justify-between">
                    <div class="flex items-center space-x-4">
                        <div class="w-12 h-12 rounded-xl bg-emerald-600/20 text-emerald-500 flex items-center justify-center group-hover:bg-emerald-600 group-hover:text-white transition-colors duration-300">
                            <i class="fa-solid fa-person-running text-xl"></i>
                        </div>
                        <div>
                            <h2 class="text-lg font-bold text-slate-800 group-hover:text-emerald-600 transition-colors">
                                운동 취미로 하자
                            </h2>
                            <p class="text-xs sm:text-sm text-slate-500 font-medium">
                                소모임 운동 & 스포츠 모임
                            </p>
                        </div>
                    </div>
                    <div class="text-slate-400 group-hover:text-emerald-600 group-hover:translate-x-1 transition-all">
                        <i class="fa-solid fa-arrow-up-right-from-square text-lg"></i>
                    </div>
                </div>
            </a>

            <!-- Card 3: Vietnam News -->
            <a href="https://vnexpress.net/" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="group block card-hover glass-card rounded-2xl p-5 shadow-lg border border-white/20 transition-all duration-300">
                <div class="flex items-center justify-between">
                    <div class="flex items-center space-x-4">
                        <div class="w-12 h-12 rounded-xl bg-rose-600/20 text-rose-500 flex items-center justify-center group-hover:bg-rose-600 group-hover:text-white transition-colors duration-300">
                            <i class="fa-regular fa-newspaper text-xl"></i>
                        </div>
                        <div>
                            <h2 class="text-lg font-bold text-slate-800 group-hover:text-rose-600 transition-colors">
                                베트남 신문 참여하자
                            </h2>
                            <p class="text-xs sm:text-sm text-slate-500 font-medium">
                                VnExpress 최신 베트남 뉴스
                            </p>
                        </div>
                    </div>
                    <div class="text-slate-400 group-hover:text-rose-600 group-hover:translate-x-1 transition-all">
                        <i class="fa-solid fa-arrow-up-right-from-square text-lg"></i>
                    </div>
                </div>
            </a>

        </main>
    </div>

    <!-- Footer / Personal Info Section -->
    <footer class="relative z-10 w-full py-8 border-t border-white/10 bg-slate-950/60 backdrop-blur-md">
        <div class="max-w-xl mx-auto px-4 flex flex-col items-center justify-center space-y-3 text-center">
            
            <p class="text-xs text-slate-400 font-medium uppercase tracking-wider">
                Contact & Information
            </p>

            <!-- Copy Email Action -->
            <div class="flex items-center space-x-2 bg-white/5 border border-white/10 px-4 py-2 rounded-full hover:bg-white/10 transition">
                <i class="fa-regular fa-envelope text-indigo-400"></i>
                <a href="mailto:nghiahanghia205@gmail.com" class="text-sm font-semibold text-slate-200 hover:text-white transition">
                    nghiahanghia205@gmail.com
                </a>
                <button onclick="copyEmail('nghiahanghia205@gmail.com')" 
                        title="이메일 복사" 
                        class="ml-2 text-xs text-slate-400 hover:text-indigo-300 p-1 rounded focus:outline-none">
                    <i class="fa-regular fa-copy" id="copy-icon"></i>
                </button>
            </div>

            <!-- Notification Toast -->
            <div id="toast" class="hidden text-xs text-emerald-400 font-medium transition-opacity duration-300">
                <i class="fa-solid fa-check mr-1"></i> 이메일 주소가 복사되었습니다!
            </div>

            <p class="text-xs text-slate-500 pt-2">
                &copy; <span id="year"></span> 응이아. All rights reserved.
            </p>
        </div>
    </footer>

    <script>
        // Set dynamic copyright year
        document.getElementById('year').textContent = new Date().getFullYear();

        // Clipboard Copy Utility Function
        function copyEmail(email) {
            // Fallback copy execution for iframe compatibility
            const tempInput = document.createElement('input');
            tempInput.value = email;
            document.body.appendChild(tempInput);
            tempInput.select();
            document.execCommand('copy');
            document.body.removeChild(tempInput);

            // Visual feedback
            const toast = document.getElementById('toast');
            const copyIcon = document.getElementById('copy-icon');

            copyIcon.className = "fa-solid fa-check text-emerald-400";
            toast.classList.remove('hidden');

            setTimeout(() => {
                copyIcon.className = "fa-regular fa-copy";
                toast.classList.add('hidden');
            }, 2500);
        }
    </script>
</body>
</html>
