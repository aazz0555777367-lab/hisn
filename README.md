<!DOCTYPE html>
<html lang="ar" dir="rtl" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>حصن المسلم - النسخة الملكية الفاخرة</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        emeraldTheme: {
                            50: '#ecfdf5',
                            100: '#d1fae5',
                            600: '#059669',
                            800: '#065f46',
                            900: '#064e3b',
                            950: '#022c22'
                        },
                        goldRoyal: {
                            300: '#fde047',
                            400: '#facc15',
                            500: '#eab308',
                            600: '#ca8a04',
                            700: '#a16207'
                        }
                    },
                    fontFamily: {
                        amiri: ['Amiri', 'serif'],
                        tajawal: ['Tajawal', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Amiri:ital,wght@0,400;0,700;1,400&family=Tajawal:wght@300;400;500;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Tajawal', sans-serif;
            background: #011611;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(5, 150, 105, 0.15) 0%, transparent 40%),
                radial-gradient(circle at 90% 80%, rgba(234, 179, 8, 0.08) 0%, transparent 40%),
                radial-gradient(circle at top, #064e3b 0%, #022c22 65%, #011611 100%);
            color: #f8fafc;
            min-height: 100vh;
        }
        .amiri-font {
            font-family: 'Amiri', serif;
        }
        .glass-card {
            background: linear-gradient(135deg, rgba(6, 78, 59, 0.75) 0%, rgba(2, 44, 34, 0.85) 100%);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(234, 179, 8, 0.4);
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.7), inset 0 1px 0 rgba(253, 224, 71, 0.2);
            transition: all 0.3s ease;
        }
        .glass-card:hover {
            border-color: rgba(234, 179, 8, 0.7);
            box-shadow: 0 25px 60px rgba(0, 0, 0, 0.8), 0 0 20px rgba(234, 179, 8, 0.15);
        }
        .glass-nav {
            background: rgba(2, 44, 34, 0.92);
            backdrop-filter: blur(16px);
            border-bottom: 1px solid rgba(234, 179, 8, 0.35);
        }
        .gold-gradient-text {
            background: linear-gradient(135deg, #fef08a 0%, #facc15 50%, #ca8a04 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .gold-btn {
            background: linear-gradient(135deg, #fef08a 0%, #facc15 50%, #ca8a04 100%);
            color: #022c22;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 0 4px 20px rgba(234, 179, 8, 0.35);
        }
        .gold-btn:hover {
            background: linear-gradient(135deg, #fffbeb 0%, #fde047 50%, #eab308 100%);
            transform: translateY(-2px);
            box-shadow: 0 12px 30px -5px rgba(234, 179, 8, 0.6);
        }
        .custom-scrollbar::-webkit-scrollbar {
            width: 6px;
            height: 6px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: rgba(2, 44, 34, 0.6);
            border-radius: 8px;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #eab308;
            border-radius: 8px;
        }
        .quran-page {
            background-color: #fcf8ee;
            background-image: radial-gradient(#e2d5be 1px, transparent 1px);
            background-size: 20px 20px;
            color: #1a1612;
            border: 12px solid #ca8a04;
            outline: 3px double #022c22;
            box-shadow: inset 0 0 30px rgba(0,0,0,0.15), 0 20px 40px rgba(0,0,0,0.8);
            border-radius: 12px;
            position: relative;
        }
        .quran-border-frame {
            border: 2px solid #064e3b;
            padding: 20px;
            margin: 6px;
            border-radius: 6px;
            position: relative;
        }
        .surah-header-frame {
            background: linear-gradient(90deg, #ca8a04 0%, #fde047 50%, #ca8a04 100%);
            color: #022c22;
            text-align: center;
            font-weight: bold;
            padding: 8px;
            border-radius: 8px;
            margin-bottom: 20px;
            border: 2px solid #022c22;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }
        @keyframes pulse-gold {
            0%, 100% { opacity: 0.4; }
            50% { opacity: 0.8; }
        }
        .royal-glow {
            animation: pulse-gold 3s infinite ease-in-out;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen selection:bg-goldRoyal-500 selection:text-emerald-950">

    <audio id="global-audio-player" class="hidden" preload="auto"></audio>

    <header class="sticky top-0 z-50 glass-nav px-4 py-3.5 shadow-2xl">
        <div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center justify-between gap-4">
            <div class="flex items-center gap-3 w-full md:w-auto justify-between md:justify-start">
                <div class="flex items-center gap-3">
                    <div class="w-12 h-12 rounded-2xl bg-gradient-to-tr from-goldRoyal-600 via-goldRoyal-400 to-goldRoyal-300 flex items-center justify-center shadow-xl text-emerald-950 text-xl font-black border border-goldRoyal-300/60 royal-glow">
                        <i class="fa-solid fa-kaaba"></i>
                    </div>
                    <div>
                        <h1 class="text-base md:text-lg font-black tracking-wide text-white flex items-center gap-2">
                            حصن المسلم <span class="text-[10px] px-2.5 py-0.5 rounded-full bg-goldRoyal-500/20 text-goldRoyal-300 border border-goldRoyal-500/50 shadow-inner">النسخة الملكية</span>
                        </h1>
                    </div>
                </div>
            </div>

            <div class="flex items-center gap-2 w-full md:w-auto flex-wrap md:flex-nowrap">
                <button onclick="useCurrentLocation()" class="p-2.5 bg-emerald-900/90 border border-goldRoyal-500/50 hover:bg-goldRoyal-500 hover:text-emerald-950 text-goldRoyal-400 rounded-2xl shadow-inner transition-all shrink-0 flex items-center gap-1.5 text-xs font-bold" title="تحديد موقعي الحالي">
                    <i class="fa-solid fa-crosshairs"></i> <span>موقعي الحالي</span>
                </button>
                <div class="relative w-full md:w-72">
                    <div class="flex items-center gap-2 bg-emerald-950/90 border border-goldRoyal-500/50 rounded-2xl px-3.5 py-2.5 shadow-inner">
                        <i class="fa-solid fa-location-dot text-goldRoyal-400 text-xs"></i>
                        <input type="text" id="city-search-input" placeholder="ابحث عن مدينتك..." class="bg-transparent text-xs text-white placeholder-emerald-300/70 focus:outline-none w-full" oninput="handleCityInput(this.value)" autocomplete="off">
                        <i class="fa-solid fa-magnifying-glass text-emerald-400 text-xs"></i>
                    </div>
                    <div id="city-suggestions" class="absolute right-0 left-0 mt-2 bg-emerald-950/95 backdrop-blur-2xl border border-goldRoyal-500/50 rounded-2xl shadow-2xl z-50 hidden max-h-52 overflow-y-auto custom-scrollbar p-1"></div>
                </div>
            </div>
        </div>
    </header>

    <nav class="relative z-40 bg-emerald-900/40 border-b border-emerald-700/40 py-3 px-4 shadow-md backdrop-blur-md">
        <div class="max-w-6xl mx-auto flex items-center justify-center gap-2.5 overflow-x-auto custom-scrollbar">
            <button onclick="switchTab('prayer')" id="tab-btn-prayer" class="px-4 py-2.5 rounded-2xl text-xs font-bold bg-goldRoyal-500 text-emerald-950 shadow-lg transition-all flex items-center gap-2 shrink-0 border border-goldRoyal-300/60 scale-105">
                <i class="fa-solid fa-mosque"></i> الصلاة والمواقيت
            </button>
            <button onclick="switchTab('athkar')" id="tab-btn-athkar" class="px-4 py-2.5 rounded-2xl text-xs font-bold bg-emerald-900/60 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 transition-all flex items-center gap-2 shrink-0">
                <i class="fa-solid fa-book-open"></i> الأذكار المكتوبة
            </button>
            <button onclick="switchTab('quran')" id="tab-btn-quran" class="px-4 py-2.5 rounded-2xl text-xs font-bold bg-emerald-900/60 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 transition-all flex items-center gap-2 shrink-0">
                <i class="fa-solid fa-quran"></i> المصحف والتلاوات النخبة
            </button>
            <button onclick="switchTab('sebha')" id="tab-btn-sebha" class="px-4 py-2.5 rounded-2xl text-xs font-bold bg-emerald-900/60 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 transition-all flex items-center gap-2 shrink-0">
                <i class="fa-solid fa-circle-dot"></i> السبحة الرقمية
            </button>
            <button onclick="switchTab('calendar')" id="tab-btn-calendar" class="px-4 py-2.5 rounded-2xl text-xs font-bold bg-emerald-900/60 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 transition-all flex items-center gap-2 shrink-0">
                <i class="fa-solid fa-calendar-days"></i> المناسبات والإشعارات
            </button>
            <button onclick="switchTab('advisor')" id="tab-btn-advisor" class="px-4 py-2.5 rounded-2xl text-xs font-bold bg-emerald-900/60 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 transition-all flex items-center gap-2 shrink-0">
                <i class="fa-solid fa-robot"></i> المستشار الذكي AI
            </button>
        </div>
    </nav>

    <main class="relative z-10 flex-1 max-w-6xl w-full mx-auto p-4 md:p-6 pb-20 space-y-6">

        <!-- Prayer Section -->
        <section id="section-prayer" class="space-y-5">
            <div class="glass-card rounded-3xl p-6 md:p-8 relative overflow-hidden">
                <div class="absolute -left-10 -bottom-10 w-40 h-40 bg-goldRoyal-500/10 rounded-full blur-2xl pointer-events-none"></div>
                <div class="flex flex-col md:flex-row items-center justify-between gap-6 relative z-10">
                    <div>
                        <div class="flex items-center gap-2.5 mb-2">
                            <span class="px-3 py-1 rounded-full bg-goldRoyal-500/25 text-goldRoyal-300 text-xs font-black border border-goldRoyal-500/50 shadow-inner">المدينة الحالية</span>
                            <h2 id="prayer-city-display" class="text-2xl font-black text-white">مكة المكرمة</h2>
                        </div>
                        <p id="prayer-date-display" class="text-xs text-emerald-300 font-medium">جاري تحميل التاريخ...</p>
                    </div>
                    <div class="bg-emerald-950/90 border border-goldRoyal-500/40 px-6 py-4 rounded-3xl text-center shadow-xl">
                        <span class="text-[11px] text-emerald-300 block mb-1 font-bold" id="next-prayer-title">الصلاة القادمة</span>
                        <div id="next-prayer-countdown" class="text-xl md:text-2xl font-black font-mono text-goldRoyal-400">00:00:00</div>
                        <span id="next-prayer-name" class="text-xs text-white font-bold mt-1 block">جاري الحساب...</span>
                    </div>
                </div>
            </div>

            <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-6 gap-4" id="prayer-times-grid"></div>
        </section>

        <!-- Athkar Section -->
        <section id="section-athkar" class="hidden space-y-5">
            <div class="glass-card rounded-2xl p-4 flex items-center justify-between gap-4 border border-goldRoyal-500/40">
                <div class="flex items-center gap-3">
                    <div class="w-10 h-10 rounded-xl bg-goldRoyal-500/20 text-goldRoyal-400 flex items-center justify-center text-lg border border-goldRoyal-500/40">
                        <i class="fa-solid fa-book-bookmark"></i>
                    </div>
                    <div>
                        <h3 class="text-xs md:text-sm font-bold text-white">حصن المسلم - الأذكار النبوية الشريفة</h3>
                    </div>
                </div>
            </div>

            <div class="flex items-center gap-2 overflow-x-auto pb-2 custom-scrollbar">
                <button onclick="filterCategory('all')" id="cat-btn-all" class="px-4 py-2 rounded-2xl text-xs font-bold bg-goldRoyal-500 text-emerald-950 shrink-0 shadow border border-goldRoyal-300/50">الكل</button>
                <button onclick="filterCategory('morning')" id="cat-btn-morning" class="px-4 py-2 rounded-2xl text-xs font-bold bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0 transition-all">أذكار الصباح</button>
                <button onclick="filterCategory('evening')" id="cat-btn-evening" class="px-4 py-2 rounded-2xl text-xs font-bold bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0 transition-all">أذكار المساء</button>
                <button onclick="filterCategory('sleep')" id="cat-btn-sleep" class="px-4 py-2 rounded-2xl text-xs font-bold bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0 transition-all">أذكار النوم</button>
                <button onclick="filterCategory('prayer')" id="cat-btn-prayer" class="px-4 py-2 rounded-2xl text-xs font-bold bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0 transition-all">أذكار الصلاة</button>
                <button onclick="filterCategory('quran')" id="cat-btn-quran" class="px-4 py-2 rounded-2xl text-xs font-bold bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0 transition-all">أدعية قرآنية</button>
            </div>

            <div class="relative">
                <i class="fa-solid fa-magnifying-glass absolute right-4 top-4 text-goldRoyal-400 text-xs"></i>
                <input type="text" id="athkar-search" placeholder="ابحث في نص الذكر أو العنوان..." class="w-full glass-card rounded-2xl pr-11 pl-4 py-3.5 text-xs md:text-sm text-white placeholder-emerald-300/70 focus:outline-none focus:border-goldRoyal-400 shadow-inner" oninput="searchAthkar(this.value)">
            </div>

            <div id="athkar-container" class="grid grid-cols-1 md:grid-cols-2 gap-5"></div>
        </section>

        <!-- Quran Section -->
        <section id="section-quran" class="hidden space-y-6">
            <div class="glass-card rounded-3xl p-6 shadow-2xl border border-goldRoyal-500/40">
                <div class="flex flex-col md:flex-row items-center justify-between gap-4 border-b border-emerald-800/80 pb-4 mb-5">
                    <div>
                        <h3 class="text-base md:text-lg font-black text-white flex items-center gap-2">
                            <i class="fa-solid fa-quran text-goldRoyal-400"></i> المصحف الشريف والتلاوات النخبة
                        </h3>
                    </div>
                    <div class="flex items-center gap-3">
                        <button onclick="stopGlobalAudio()" class="px-3 py-2 rounded-2xl bg-red-600 text-white font-bold text-xs shadow hover:bg-red-500 border border-red-400/50">
                            🛑 إيقاف التلاوة
                        </button>
                    </div>
                </div>

                <div class="bg-emerald-950/90 rounded-2xl p-4 border border-goldRoyal-500/40 mb-5 shadow-inner">
                    <label class="text-xs font-bold text-goldRoyal-300 block mb-2"><i class="fa-solid fa-microphone-lines ml-1"></i> اختر القارئ الشيخ:</label>
                    <select id="reciter-select" class="w-full bg-emerald-900 border border-goldRoyal-500/50 rounded-2xl px-4 py-3 text-xs md:text-sm text-white focus:outline-none shadow-inner" onchange="changeReciter(this.value)">
                        <option value="yasser">الشيخ ياسر الدوسري</option>
                        <option value="afasy">الشيخ مشاري بن راشد العفاسي</option>
                        <option value="sudais">الشيخ عبد الرحمن السديس</option>
                        <option value="maher">الشيخ ماهر المعيقلي</option>
                        <option value="ghamdi">الشيخ سعد الغامدي</option>
                    </select>
                </div>

                <div class="bg-emerald-950/80 rounded-2xl p-4 border border-emerald-800/80 mb-6 shadow-inner">
                    <div class="flex items-center justify-between mb-2">
                        <span class="text-xs font-bold text-goldRoyal-300">مستوى إنجاز الختمة القرآنية</span>
                        <span id="khatma-percent" class="text-xs font-black text-white">0%</span>
                    </div>
                    <div class="w-full bg-emerald-900 rounded-full h-3 overflow-hidden border border-emerald-700/60">
                        <div id="khatma-bar" class="bg-gradient-to-r from-goldRoyal-600 via-goldRoyal-400 to-goldRoyal-300 h-3 rounded-full transition-all duration-500" style="width: 0%"></div>
                    </div>
                    <div class="flex items-center justify-between mt-3 text-[11px] text-emerald-300">
                        <span>السورة المكتملة الأخيرة: <strong id="khatma-last-surah" class="text-white">لا يوجد</strong></span>
                        <button onclick="resetKhatma()" class="text-goldRoyal-400 hover:underline"><i class="fa-solid fa-rotate-right ml-1"></i> إعادة الختمة</button>
                    </div>
                </div>

                <div id="surah-list-container" class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-3 max-h-96 overflow-y-auto custom-scrollbar p-1">
                    <div class="text-center py-6 text-emerald-300 text-xs col-span-full">جاري تحميل السور الشريفة...</div>
                </div>

                <div id="quran-reader-modal" class="hidden mt-6 relative">
                    <div class="quran-page p-4 md:p-8 relative overflow-hidden">
                        <div class="quran-border-frame">
                            <div class="flex items-center justify-between border-b-2 border-emerald-900/40 pb-3 mb-4 flex-wrap gap-2">
                                <button onclick="closeQuranReader()" class="px-3 py-1.5 rounded-xl bg-emerald-900 text-white hover:bg-goldRoyal-500 hover:text-emerald-950 text-xs font-bold shadow transition-all">
                                    <i class="fa-solid fa-arrow-right ml-1"></i> إغلاق المصحف
                                </button>
                                <div class="flex items-center gap-2">
                                    <button id="btn-play-surah-audio" onclick="playCurrentSurahAudio()" class="px-4 py-1.5 rounded-xl bg-goldRoyal-500 text-emerald-950 hover:bg-goldRoyal-400 font-black text-xs shadow flex items-center gap-1.5 border border-goldRoyal-300">
                                        <i class="fa-solid fa-circle-play text-sm"></i> <span>تشغيل السورة كاملة بصوت القارئ</span>
                                    </button>
                                    <button onclick="stopGlobalAudio()" class="px-3 py-1.5 rounded-xl bg-red-600 text-white hover:bg-red-500 font-bold text-xs shadow border border-red-400/50">
                                        <i class="fa-solid fa-circle-stop"></i> إيقاف الصوت
                                    </button>
                                </div>
                            </div>

                            <div class="surah-header-frame">
                                <h4 id="reader-surah-title" class="text-2xl font-black amiri-font"></h4>
                            </div>

                            <div class="text-center mb-6 amiri-font text-lg font-bold text-emerald-950">
                                ﷽
                            </div>

                            <div id="reader-verses-container" class="amiri-font text-xl md:text-2xl text-emerald-950 leading-loose text-justify p-2 space-y-2 font-bold" style="direction: rtl;"></div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sebha Section -->
        <section id="section-sebha" class="hidden flex flex-col items-center justify-center py-6 space-y-5">
            <div class="glass-card p-6 md:p-9 rounded-3xl text-center max-w-sm w-full relative overflow-hidden shadow-2xl border border-goldRoyal-500/40">
                <div class="mb-4 text-right">
                    <label class="text-xs text-emerald-300 block mb-1.5 font-bold">اختر الذكر للتسبيح:</label>
                    <select id="sebha-dhikr-select" class="w-full bg-emerald-950/90 border border-goldRoyal-500/50 rounded-2xl px-4 py-3 text-xs text-white focus:outline-none shadow-inner">
                        <option value="سبحان الله">سبحان الله</option>
                        <option value="الحمد لله">الحمد لله</option>
                        <option value="لا إله إلا الله">لا إله إلا الله</option>
                        <option value="الله أكبر">الله أكبر</option>
                        <option value="استغفر الله العظيم">استغفر الله العظيم</option>
                        <option value="لاحول ولا قوة إلا بالله">لاحول ولا قوة إلا بالله</option>
                    </select>
                </div>

                <div class="my-6 relative py-4">
                    <div class="w-44 h-44 mx-auto rounded-full border-4 border-goldRoyal-400/50 flex items-center justify-center bg-emerald-950/85 shadow-2xl royal-glow">
                        <span id="sebha-display-count" class="text-6xl font-black text-white font-mono tracking-wider">0</span>
                    </div>
                </div>

                <div class="space-y-3">
                    <button onclick="incrementSebha()" class="w-full py-4 gold-btn font-black text-base rounded-2xl shadow-xl flex items-center justify-center gap-2 active:scale-95 border border-goldRoyal-300/50">
                        <i class="fa-solid fa-fingerprint text-xl"></i> اضغط للتسبيح
                    </button>
                    <div class="flex items-center gap-2.5">
                        <button onclick="resetSebha()" class="flex-1 py-2.5 bg-emerald-900/70 hover:bg-emerald-800 text-emerald-300 rounded-2xl text-xs font-bold border border-emerald-700/60 shadow">
                            <i class="fa-solid fa-rotate-right ml-1"></i> تصفير
                        </button>
                        <button onclick="vibrateSebha()" id="vibrate-btn" class="px-4 py-2.5 bg-emerald-900/70 hover:bg-emerald-800 text-goldRoyal-400 rounded-2xl text-xs font-bold border border-emerald-700/60 shadow">
                            <i class="fa-solid fa-bell"></i> التنبيه
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Events Calendar Section -->
        <section id="section-calendar" class="hidden space-y-6">
            <div class="glass-card rounded-3xl p-6 shadow-2xl border border-goldRoyal-500/40">
                <div class="flex flex-col md:flex-row items-center justify-between border-b border-emerald-800/80 pb-4 mb-5 gap-3">
                    <div>
                        <h3 class="text-base md:text-lg font-black text-white flex items-center gap-2">
                            <i class="fa-solid fa-calendar-star text-goldRoyal-400"></i> المناسبات الإسلامية والعد التنازلي
                        </h3>
                    </div>
                    <button onclick="toggleNotifications()" id="notif-toggle-btn" class="px-4 py-2.5 rounded-2xl text-xs font-bold bg-emerald-900/90 border border-goldRoyal-500/50 text-goldRoyal-400 flex items-center gap-2 shadow transition-all hover:bg-goldRoyal-500 hover:text-emerald-950">
                        <i class="fa-solid fa-bell" id="notif-icon"></i> <span id="notif-status-text">الإشعارات مفعلة</span>
                    </button>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4" id="events-countdown-grid"></div>
            </div>
        </section>

        <!-- Advisor Section -->
        <section id="section-advisor" class="hidden space-y-3">
            <div class="glass-card rounded-3xl p-5 md:p-6 flex flex-col h-[560px] shadow-2xl">
                <div class="border-b border-emerald-800/80 pb-3 mb-3 flex items-center justify-between">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-2xl bg-goldRoyal-500/20 flex items-center justify-center text-goldRoyal-400 text-base border border-goldRoyal-500/40">
                            <i class="fa-solid fa-robot"></i>
                        </div>
                        <div>
                            <h3 class="text-sm md:text-base font-bold text-white">المستشار الإسلامي الذكي AI</h3>
                        </div>
                    </div>
                    <button onclick="clearChat()" class="text-xs text-emerald-400 hover:text-goldRoyal-400 px-3 py-1.5 rounded-2xl bg-emerald-950/75 border border-emerald-800">
                        <i class="fa-solid fa-trash-can ml-1"></i> مسح المحادثة
                    </button>
                </div>

                <div id="chat-messages" class="flex-1 overflow-y-auto space-y-3.5 pr-2 custom-scrollbar text-xs md:text-sm">
                    <div class="glass-card p-4 rounded-2xl border border-emerald-800/80 max-w-[85%] text-slate-200 leading-relaxed shadow">
                        <span class="text-goldRoyal-400 font-bold block mb-1.5"><i class="fa-solid fa-star"></i> أهلاً بك:</span>
                        أنا مساعدك الإسلامي الذكي. كيف يمكنني مساعدتك اليوم في أذكارك وعباداتك وأسئلتك الشرعية؟
                    </div>
                </div>

                <div class="py-2 flex items-center gap-2 overflow-x-auto custom-scrollbar text-xs">
                    <span class="text-emerald-400 font-bold shrink-0">أسئلة مقترحة:</span>
                    <button onclick="sendQuickPrompt('ما هو فضل أذكار الصباح والمساء؟')" class="px-3 py-1.5 rounded-xl bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0">فضل أذكار الصباح</button>
                    <button onclick="sendQuickPrompt('كيف أخشع في صلاتي وأذكاري؟')" class="px-3 py-1.5 rounded-xl bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0">الخشوع في الصلاة</button>
                    <button onclick="sendQuickPrompt('ما هي أفضل أدعية الاستغفار والتوبة؟')" class="px-3 py-1.5 rounded-xl bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0">أدعية الاستغفار</button>
                </div>

                <div class="pt-3 border-t border-emerald-800/80 flex gap-2.5">
                    <input type="text" id="chat-input" placeholder="اكتب سؤالك هنا..." class="flex-1 bg-emerald-950/90 border border-goldRoyal-500/40 rounded-2xl px-4 py-3 text-xs md:text-sm text-white placeholder-emerald-300/70 focus:outline-none focus:border-goldRoyal-400 shadow-inner" onkeypress="if(event.key==='Enter')sendChatMessage()">
                    <button onclick="sendChatMessage()" class="gold-btn px-6 py-3 rounded-2xl text-xs md:text-sm font-black shadow flex items-center gap-2 border border-goldRoyal-300/40">
                        <i class="fa-solid fa-paper-plane"></i> إرسال
                    </button>
                </div>
            </div>
        </section>
    </main>

    <div id="share-card-modal" class="hidden fixed inset-0 z-50 bg-black/80 backdrop-blur-md flex items-center justify-center p-4">
        <div class="glass-card max-w-md w-full rounded-3xl p-6 relative border border-goldRoyal-500/50 shadow-2xl text-center space-y-4">
            <button onclick="closeShareModal()" class="absolute left-4 top-4 text-emerald-400 hover:text-goldRoyal-400 text-lg"><i class="fa-solid fa-xmark"></i></button>

            <div id="share-card-content" class="bg-gradient-to-b from-emerald-900 to-emerald-950 p-6 rounded-2xl border border-goldRoyal-400/40 shadow-inner text-right space-y-3">
                <div class="flex items-center justify-between border-b border-goldRoyal-500/30 pb-2">
                    <span class="text-xs font-black text-goldRoyal-400" id="share-card-title">ذكر مبارك</span>
                    <i class="fa-solid fa-kaaba text-goldRoyal-400"></i>
                </div>
                <p id="share-card-text" class="amiri-font text-lg text-white leading-relaxed"></p>
                <div class="text-[10px] text-emerald-300 text-center pt-2 border-t border-emerald-800/60">حصن المسلم - النسخة الملكية</div>
            </div>

            <button onclick="copyShareText()" class="w-full gold-btn py-3 rounded-2xl font-black text-xs shadow-lg">
                <i class="fa-solid fa-copy ml-1"></i> نسخ نص بطاقة الذكر
            </button>
        </div>
    </div>

    <footer class="relative z-10 text-center py-4 border-t border-emerald-800/60 bg-emerald-950/90 text-xs text-emerald-300 space-y-2">
        <p>جميع الأذكار مستقاة من كتاب (حصن المسلم) للشيخ سعيد بن علي بن وهف القحطاني رحمه الله.</p>
        <div class="text-goldRoyal-400 font-bold text-xs inline-flex items-center gap-1">
            <i class="fa-solid fa-kaaba"></i> حصن المسلم - النسخة الملكية الفاخرة
        </div>
    </footer>

    <script>
        const recitersData = {
            yasser: { name: "الشيخ ياسر الدوسري", server: "https://server11.mp3quran.net/yasser/" },
            afasy: { name: "الشيخ مشاري العفاسي", server: "https://server8.mp3quran.net/afs/" },
            sudais: { name: "الشيخ عبد الرحمن السديس", server: "https://server11.mp3quran.net/sds/" },
            maher: { name: "الشيخ ماهر المعيقلي", server: "https://server12.mp3quran.net/maher/" },
            ghamdi: { name: "الشيخ سعد الغامدي", server: "https://server7.mp3quran.net/s_gmd/" }
        };

        let currentReciterKey = 'yasser';

        const athkarList = [
            { id: 1, cat: 'morning', title: 'آية الكرسي', text: 'اللّهُ لاَ إِلََهَ إِلاَّ هُوَ الْحَيُّ الْقَيُّومُ لاَ تأْخُذُهُ سِنَةٌ وَلاَ نَوْمٌ لَّهُ مَا فِي السَّمَاوَاتِ وَمَا فِي الأَرْضِ مَن ذَا الذي يَشْفَعُ عِنْدَهُ إِلاَّ بِإِذْنِهِ يَعْلَمُ مَا بَيْنَ أَيْدِيهِمْ وَمَا خَلْفَهُمْ وَلاَ يُحِيطُونَ بِشَيْءٍ مِّنْ عِلْمِهِ إِلاَّ بِمَا شَاء وَسِعَ كُرْسِيُّهُ السَّمَاوَاتِ وَالأَرْضَ وَلاَ يَؤُودُهُ حِفْظُهُمَا وَهُوَ الْعَلِيُّ الْعَظِيمُ', count: 1, maxCount: 1, virtue: 'من قرأها دبر كل صلاة لم يمنعه من دخول الجنة إلا أن يموت.' },
            { id: 2, cat: 'morning', title: 'سورة الإخلاص', text: 'قُلْ هُوَ اللَّهُ أَحَدٌ ۞ اللَّهُ الصَّمَدُ ۞ لَمْ يَلِدْ وَلَمْ يُولَدْ ۞ وَلَمْ يَكُن لَّهُ كُفُوًا أَحَدٌ', count: 3, maxCount: 3, virtue: 'تكفيك من كل شيء حين تصبح وحين تمسي.' },
            { id: 3, cat: 'morning', title: 'سورة الفلق', text: 'قُلْ أَعُوذُ بِرَبِّ الْفَلَقِ ۞ مِن شَرِّ مَا خَلَقَ ۞ وَمِن شَرِّ غَاسِقٍ إِذَا وَقَبَ ۞ وَمِن شَرِّ النَّفَّاثَاتِ فِي الْعُقَدِ ۞ وَمِن شَرِّ حَاسِدٍ إِذَا حَسَدَ', count: 3, maxCount: 3, virtue: 'تحصين من الشرور والحسد.' },
            { id: 4, cat: 'morning', title: 'سورة الناس', text: 'قُلْ أَعُوذُ بِرَبِّ النَّاسِ ۞ مَلِكِ النَّاسِ ۞ إِلَهِ النَّاسِ ۞ مِن شَرِّ الْوَسْوَاسِ الْخَنَّاسِ ۞ الَّذِي يُوَسْوِسُ فِي صُدُورِ النَّاسِ ۞ مِنَ الْجِنَّةِ وَالنَّاسِ', count: 3, maxCount: 3, virtue: 'الحفظ والوقاية من الوساوس.' },
            { id: 5, cat: 'morning', title: 'أصبحنا وأصبح الملك لله', text: 'أصبحنا وأصبح الملك لله، والحمد لله، لا إله إلا الله وحده لا شريك له، له الملك وله الحمد وهو على كل شيء قدير. رب أسألك خير ما في هذا اليوم وخير ما بعده، وأعوذ بك من شر ما في هذا اليوم وشر ما بعده.', count: 1, maxCount: 1, virtue: 'دعاء جامع للبركة والتوفيق في بداية اليوم.' },
            { id: 6, cat: 'morning', title: 'سيد الاستغفار', text: 'اللهم أنت ربي لا إله إلا أنت، خلقتني وأنا عبدك، وأنا على عهدك ووعدك ما استطعت، أعوذ بك من شر ما صنعت، أبوء لك بنعمتك علي، وأبوء لك بذنبي فاغفر لي فإنه لا يغفر الذنوب إلا أنت.', count: 1, maxCount: 1, virtue: 'من قاله موقناً بها من النهار فمات قبل أن يُمسي فهو من أهل الجنة.' },
            { id: 7, cat: 'morning', title: 'رضيت بالله رباً وبالإسلام ديناً', text: 'رضيت بالله رباً، وبالإسلام ديناً، وبمحمد صلى الله عليه وسلم نبياً ورسولاً.', count: 3, maxCount: 3, virtue: 'حق على الله أن يرضيه يوم القيامة.' },
            { id: 8, cat: 'evening', title: 'أمسينا وأمسى الملك لله', text: 'أمسينا وأمسى الملك لله، والحمد لله، لا إله إلا الله وحده لا شريك له، له الملك وله الحمد وهو على كل شيء قدير. رب أسألك خير ما في هذه الليلة وخير ما بعدها، وأعوذ بك من شر هذه الليلة وشر ما بعدها.', count: 1, maxCount: 1, virtue: 'حفظ وأمان في المساء والليل.' },
            { id: 9, cat: 'evening', title: 'أعوذ بكلمات الله التامات من شر ما خلق', text: 'أعوذ بكلمات الله التامات من شر ما خلق.', count: 3, maxCount: 3, virtue: 'لم يضره شيء في تلك الليلة.' },
            { id: 10, cat: 'sleep', title: 'باسمك ربي وضعت جنبي', text: 'باسمك ربي وضعت جنبي وبك أرفعه، إن أمسكت نفسي فارحمني، وإن أرسلتها فاحفظها بما تحفظ به عبادك الصالحين.', count: 1, maxCount: 1, virtue: 'سنة نبوية مباركة قبل النوم.' },
            { id: 11, cat: 'prayer', title: 'أذكار دبر الصلاة المكتوبة', text: 'أستغفر الله، أستغفر الله، أستغفر الله. اللهم أنت السلام ومنك السلام، تباركت يا ذا الجلال والإكرام.', count: 1, maxCount: 1, virtue: 'من أسباب مغفرة الذنوب بعد الفريضة.' },
            { id: 12, cat: 'quran', title: 'دعاء ربنا آتنا في الدنيا حسنة', text: 'رَبَّنَا آتِنَا فِي الدُّنْيَا حَسَنَةً وَفِي الْآخِرَةِ حَسَنَةً وَقِنَا عَذَابَ النَّارِ', count: 1, maxCount: 1, virtue: 'من أكثر الأدعية الجامعة لخيري الدنيا والآخرة.' }
        ];

        const islamicEvents = [
            { id: 1, name: 'شهر رمضان المبارك', dateStr: '2027-02-08', icon: 'fa-moon' },
            { id: 2, name: 'عيد الفطر السعيد', dateStr: '2027-03-10', icon: 'fa-star-and-crescent' },
            { id: 3, name: 'يوم عرفة الفضيل', dateStr: '2027-05-16', icon: 'fa-kaaba' },
            { id: 4, name: 'عيد الأضحى المبارك', dateStr: '2027-05-17', icon: 'fa-gift' }
        ];

        let currentCategory = 'all';
        let searchQuery = '';
        let sebhaCount = localStorage.getItem('royal_sebha_count') ? parseInt(localStorage.getItem('royal_sebha_count')) : 0;
        let soundEnabled = true;
        let notificationsEnabled = localStorage.getItem('royal_notifications') !== 'false';
        let searchTimeout = null;
        let todayTimings = null;
        let completedSurahs = JSON.parse(localStorage.getItem('royal_khatma_surahs') || '[]');
        let activeSurahNumber = null;
        let activeSurahName = '';

        window.addEventListener('DOMContentLoaded', () => {
            renderAthkar();
            fetchPrayerTimesByCity('Makkah');
            fetchSurahsList();
            updateKhatmaUI();
            renderEventsCountdown();
            updateNotificationUI();
            const disp = document.getElementById('sebha-display-count');
            if (disp) disp.innerText = sebhaCount;
            setInterval(updateCountdown, 1000);
        });

        function stopGlobalAudio() {
            const player = document.getElementById('global-audio-player');
            if (player) {
                player.pause();
                player.currentTime = 0;
            }
        }

        function switchTab(tab) {
            ['prayer', 'athkar', 'quran', 'sebha', 'calendar', 'advisor'].forEach(t => {
                const sec = document.getElementById(`section-${t}`);
                if (sec) sec.classList.add('hidden');
                const btn = document.getElementById(`tab-btn-${t}`);
                if (btn) btn.className = "px-4 py-2.5 rounded-2xl text-xs font-bold bg-emerald-900/60 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 transition-all flex items-center gap-2 shrink-0";
            });
            const activeSec = document.getElementById(`section-${tab}`);
            if (activeSec) activeSec.classList.remove('hidden');
            const activeBtn = document.getElementById(`tab-btn-${tab}`);
            if (activeBtn) activeBtn.className = "px-4 py-2.5 rounded-2xl text-xs font-bold bg-goldRoyal-500 text-emerald-950 shadow-lg transition-all flex items-center gap-2 shrink-0 border border-goldRoyal-300/60 scale-105";
        }

        function changeReciter(key) {
            currentReciterKey = key;
        }

        function renderAthkar() {
            const container = document.getElementById('athkar-container');
            if (!container) return;

            let filtered = athkarList.filter(item => {
                const matchCat = currentCategory === 'all' || item.cat === currentCategory;
                const matchSearch = item.title.includes(searchQuery) || item.text.includes(searchQuery);
                return matchCat && matchSearch;
            });

            if (filtered.length === 0) {
                container.innerHTML = `<div class="col-span-full text-center py-12 text-emerald-300 text-xs md:text-sm font-bold glass-card rounded-3xl">لا توجد أذكار مطابقة لبحثك</div>`;
                return;
            }

            container.innerHTML = filtered.map((item) => {
                return `
                <div class="glass-card rounded-3xl p-5 md:p-6 flex flex-col justify-between shadow-2xl">
                    <div>
                        <div class="flex items-center justify-between border-b border-emerald-800/80 pb-3 mb-3">
                            <span class="text-xs md:text-sm font-black gold-gradient-text">${item.title}</span>
                            <span class="text-[11px] bg-emerald-950/90 px-3 py-1 rounded-full text-goldRoyal-300 font-bold border border-goldRoyal-500/40 shadow-inner">متبقي: ${item.count}</span>
                        </div>
                        <p class="amiri-font text-base md:text-lg text-slate-100 leading-relaxed text-right my-3">${item.text}</p>
                        ${item.virtue ? `<div class="text-[11px] text-emerald-200 bg-emerald-950/75 p-3 rounded-2xl border border-emerald-800/70 mb-4 flex items-start gap-2.5 shadow-inner"><i class="fa-solid fa-star text-goldRoyal-400 mt-0.5"></i> <span>${item.virtue}</span></div>` : ''}
                    </div>
                    <div class="flex items-center justify-between pt-3 border-t border-emerald-800/60 gap-2 flex-wrap">
                        <div class="flex items-center gap-2">
                            <button onclick="decrementCount(${item.id})" class="gold-btn px-4 py-2 rounded-2xl text-xs font-black flex items-center gap-2 shadow-lg border border-goldRoyal-300/40">
                                <i class="fa-solid fa-hand-pointer"></i> قرأت الذكر (${item.count})
                            </button>
                        </div>
                        <div class="flex items-center gap-2">
                            <button onclick="openShareModal(${item.id})" class="text-emerald-300 hover:text-goldRoyal-400 text-xs font-bold px-3 py-1.5 rounded-2xl bg-emerald-950/70 border border-emerald-800 shadow" title="مشاركة الذكر">
                                <i class="fa-solid fa-share-nodes"></i> مشاركة
                            </button>
                            <button onclick="resetItemCount(${item.id})" class="text-emerald-300 hover:text-goldRoyal-400 text-xs font-bold px-3 py-1.5 rounded-2xl bg-emerald-950/70 border border-emerald-800 shadow">
                                <i class="fa-solid fa-rotate-right ml-1"></i> إعادة
                            </button>
                        </div>
                    </div>
                </div>
            `;
            }).join('');
        }

        function filterCategory(cat) {
            currentCategory = cat;
            ['all', 'morning', 'evening', 'sleep', 'prayer', 'quran'].forEach(c => {
                const btn = document.getElementById(`cat-btn-${c}`);
                if (!btn) return;
                if (c === cat) {
                    btn.className = "px-4 py-2 rounded-2xl text-xs font-bold bg-goldRoyal-500 text-emerald-950 shrink-0 shadow border border-goldRoyal-300/50";
                } else {
                    btn.className = "px-4 py-2 rounded-2xl text-xs font-bold bg-emerald-900/70 hover:bg-emerald-800 text-emerald-200 border border-emerald-700/60 shrink-0 transition-all";
                }
            });
            renderAthkar();
        }

        function searchAthkar(val) {
            searchQuery = val.trim();
            renderAthkar();
        }

        function decrementCount(id) {
            const item = athkarList.find(i => i.id === id);
            if (item && item.count > 0) {
                item.count--;
                renderAthkar();
            }
        }

        function resetItemCount(id) {
            const item = athkarList.find(i => i.id === id);
            if (item) {
                item.count = item.maxCount;
                renderAthkar();
            }
        }

        function openShareModal(id) {
            const item = athkarList.find(i => i.id === id);
            if (!item) return;
            document.getElementById('share-card-title').innerText = item.title;
            document.getElementById('share-card-text').innerText = item.text;
            document.getElementById('share-card-modal').classList.remove('hidden');
        }

        function closeShareModal() {
            document.getElementById('share-card-modal').classList.add('hidden');
        }

        function copyShareText() {
            const title = document.getElementById('share-card-title').innerText;
            const text = document.getElementById('share-card-text').innerText;
            const fullText = `✨ ${title} ✨\n\n${text}\n\n— من تطبيق حصن المسلم النسخة الملكية`;
            navigator.clipboard.writeText(fullText).then(() => {
                alert("تم نسخ الذكر إلى الحافظة بنجاح!");
            });
        }

        async function fetchSurahsList() {
            const container = document.getElementById('surah-list-container');
            if (!container) return;
            try {
                const res = await fetch('https://api.alquran.cloud/v1/surah');
                const data = await res.json();
                if (data && data.code === 200) {
                    container.innerHTML = data.data.map(s => {
                        const isDone = completedSurahs.includes(s.number);
                        return `
                            <div class="bg-emerald-950/80 p-3 rounded-2xl border ${isDone ? 'border-goldRoyal-400' : 'border-emerald-800/80'} hover:border-goldRoyal-400/80 transition-all flex items-center justify-between">
                                <div>
                                    <span class="text-[10px] text-goldRoyal-400 font-mono block">سورة ${s.number}</span>
                                    <span class="text-xs font-bold text-white">${s.name}</span>
                                </div>
                                <div class="flex items-center gap-1.5">
                                    <button onclick="readSurah(${s.number}, '${s.name}')" class="p-1.5 text-xs text-emerald-300 hover:text-goldRoyal-400" title="قراءة واستماع"><i class="fa-solid fa-book-open"></i></button>
                                    <button onclick="toggleSurahKhatma(${s.number}, '${s.name}')" class="p-1.5 text-xs ${isDone ? 'text-goldRoyal-400' : 'text-emerald-600'}"><i class="fa-solid fa-circle-check"></i></button>
                                </div>
                            </div>
                        `;
                    }).join('');
                }
            } catch (e) {
                container.innerHTML = `<div class="text-center py-4 text-emerald-300 text-xs col-span-full">تعذر تحميل قائمة السور حالياً</div>`;
            }
        }

        async function readSurah(number, name) {
            activeSurahNumber = number;
            activeSurahName = name;
            const modal = document.getElementById('quran-reader-modal');
            const title = document.getElementById('reader-surah-title');
            const container = document.getElementById('reader-verses-container');
            title.innerText = `سورة ${name}`;
            container.innerHTML = 'جاري تحضير نصوص السورة...';
            modal.classList.remove('hidden');

            try {
                const res = await fetch(`https://api.alquran.cloud/v1/surah/${number}`);
                const data = await res.json();
                if (data && data.code === 200) {
                    const verses = data.data.ayahs;
                    container.innerHTML = verses.map(v => `
                        ${v.text} 
                        <span class="text-amber-800 text-sm font-bold font-mono px-1">﴿${v.numberInSurah}﴾</span>
                    `).join(' ');
                }
            } catch (e) {
                container.innerHTML = 'حدث خطأ أثناء تحميل نصوص السورة الشريفة.';
            }
        }

        function playCurrentSurahAudio() {
            if (!activeSurahNumber) return;
            stopGlobalAudio();
            const formattedSurahNum = String(activeSurahNumber).padStart(3, '0');
            const reciter = recitersData[currentReciterKey];
            const audioUrl = `${reciter.server}${formattedSurahNum}.mp3`;
            const player = document.getElementById('global-audio-player');
            player.src = audioUrl;
            player.play().catch(() => {
                alert("تعذر التشغيل تلقائياً. يرجى الضغط مرة أخرى للتأكيد.");
            });
        }

        function closeQuranReader() {
            stopGlobalAudio();
            document.getElementById('quran-reader-modal').classList.add('hidden');
        }

        function toggleSurahKhatma(surahNum, surahName) {
            const idx = completedSurahs.indexOf(surahNum);
            if (idx > -1) {
                completedSurahs.splice(idx, 1);
            } else {
                completedSurahs.push(surahNum);
                localStorage.setItem('royal_last_surah_name', surahName);
            }
            localStorage.setItem('royal_khatma_surahs', JSON.stringify(completedSurahs));
            updateKhatmaUI();
            fetchSurahsList();
        }

        function updateKhatmaUI() {
            const total = 114;
            const pct = Math.round((completedSurahs.length / total) * 100);
            const bar = document.getElementById('khatma-bar');
            const pctTxt = document.getElementById('khatma-percent');
            const lastSurah = document.getElementById('khatma-last-surah');

            if (bar) bar.style.width = `${pct}%`;
            if (pctTxt) pctTxt.innerText = `${pct}%`;
            if (lastSurah) lastSurah.innerText = localStorage.getItem('royal_last_surah_name') || 'لا يوجد';
        }

        function resetKhatma() {
            completedSurahs = [];
            localStorage.removeItem('royal_khatma_surahs');
            localStorage.removeItem('royal_last_surah_name');
            updateKhatmaUI();
            fetchSurahsList();
        }

        function renderEventsCountdown() {
            const container = document.getElementById('events-countdown-grid');
            if (!container) return;

            const now = new Date();

            container.innerHTML = islamicEvents.map(event => {
                const target = new Date(event.dateStr);
                const diffTime = target - now;
                const diffDays = Math.ceil(diffTime / (1000 * 60 * 60 * 24));

                return `
                    <div class="glass-card p-5 rounded-3xl border border-emerald-800/80 text-center flex flex-col justify-between items-center shadow-xl">
                        <div class="w-12 h-12 rounded-2xl bg-goldRoyal-500/20 text-goldRoyal-400 flex items-center justify-center text-xl mb-3 border border-goldRoyal-500/40">
                            <i class="fa-solid ${event.icon}"></i>
                        </div>
                        <h4 class="text-sm font-black text-white mb-2">${event.name}</h4>
                        <div class="my-3 bg-emerald-950/90 px-4 py-3 rounded-2xl border border-goldRoyal-500/30 w-full">
                            <span class="text-2xl font-black text-goldRoyal-400 font-mono block">${diffDays > 0 ? diffDays : 0}</span>
                            <span class="text-[10px] text-emerald-300 font-bold">يوماً متبقياً</span>
                        </div>
                        <span class="text-[10px] text-emerald-400 font-medium">الموعد التقديري: ${event.dateStr}</span>
                    </div>
                `;
            }).join('');
        }

        function toggleNotifications() {
            notificationsEnabled = !notificationsEnabled;
            localStorage.setItem('royal_notifications', notificationsEnabled);
            updateNotificationUI();
        }

        function updateNotificationUI() {
            const btn = document.getElementById('notif-toggle-btn');
            const icon = document.getElementById('notif-icon');
            const txt = document.getElementById('notif-status-text');
            if (!btn) return;

            if (notificationsEnabled) {
                btn.className = "px-4 py-2.5 rounded-2xl text-xs font-bold bg-goldRoyal-500 text-emerald-950 flex items-center gap-2 shadow transition-all";
                icon.className = "fa-solid fa-bell";
                txt.innerText = "الإشعارات مفعلة";
            } else {
                btn.className = "px-4 py-2.5 rounded-2xl text-xs font-bold bg-emerald-900/90 border border-emerald-700/60 text-emerald-300 flex items-center gap-2 shadow transition-all";
                icon.className = "fa-solid fa-bell-slash";
                txt.innerText = "الإشعارات معطلة";
            }
        }

        function incrementSebha() {
            sebhaCount++;
            localStorage.setItem('royal_sebha_count', sebhaCount);
            const disp = document.getElementById('sebha-display-count');
            if (disp) disp.innerText = sebhaCount;
            if (soundEnabled && navigator.vibrate) {
                navigator.vibrate(40);
            }
        }

        function resetSebha() {
            sebhaCount = 0;
            localStorage.setItem('royal_sebha_count', 0);
            const disp = document.getElementById('sebha-display-count');
            if (disp) disp.innerText = sebhaCount;
        }

        function vibrateSebha() {
            soundEnabled = !soundEnabled;
            const btn = document.getElementById('vibrate-btn');
            if (!btn) return;
            if (soundEnabled) {
                btn.innerHTML = `<i class="fa-solid fa-bell"></i> التنبيه مفعل`;
                btn.classList.add('text-goldRoyal-400');
            } else {
                btn.innerHTML = `<i class="fa-solid fa-bell-slash"></i> معطل`;
                btn.classList.remove('text-goldRoyal-400');
            }
        }

        function handleCityInput(val) {
            clearTimeout(searchTimeout);
            const sugBox = document.getElementById('city-suggestions');
            if (!sugBox) return;
            if (!val || val.trim().length < 2) {
                sugBox.classList.add('hidden');
                sugBox.innerHTML = '';
                return;
            }

            searchTimeout = setTimeout(async () => {
                try {
                    const res = await fetch(`https://geocoding-api.open-meteo.com/v1/search?name=${encodeURIComponent(val)}&count=6&language=ar&format=json`);
                    const data = await res.json();
                    if (data && data.results && data.results.length > 0) {
                        sugBox.innerHTML = data.results.map(city => {
                            const cityName = city.name;
                            const countryName = city.country || '';
                            const admin1 = city.admin1 || '';
                            const lat = city.latitude;
                            const lng = city.longitude;
                            return `<div onclick="selectCityCoords('${cityName}', ${lat}, ${lng})" class="px-3.5 py-2.5 text-xs text-slate-100 hover:bg-emerald-900/90 cursor-pointer rounded-xl border-b border-emerald-900/50 flex items-center justify-between transition-all">
                                <span class="font-bold text-white">${cityName}</span>
                                <span class="text-[10px] text-goldRoyal-400">${admin1} - ${countryName}</span>
                            </div>`;
                        }).join('');
                        sugBox.classList.remove('hidden');
                    } else {
                        sugBox.innerHTML = `<div class="p-3 text-xs text-emerald-300 text-center">لا توجد نتائج مطابقة</div>`;
                        sugBox.classList.remove('hidden');
                    }
                } catch (e) {
                    sugBox.classList.add('hidden');
                }
            }, 300);
        }

        function selectCityCoords(cityName, lat, lng) {
            const input = document.getElementById('city-search-input');
            if (input) input.value = cityName;
            const sugBox = document.getElementById('city-suggestions');
            if (sugBox) sugBox.classList.add('hidden');
            const cityDisp = document.getElementById('prayer-city-display');
            if (cityDisp) cityDisp.innerText = cityName;
            
            fetchPrayerTimesByCoords(lat, lng, cityName);
        }

        function useCurrentLocation() {
            if (navigator.geolocation) {
                const cityDisp = document.getElementById('prayer-city-display');
                if (cityDisp) cityDisp.innerText = "جاري تحديد موقعك الجغرافي...";
                navigator.geolocation.getCurrentPosition(
                    async (pos) => {
                        const lat = pos.coords.latitude;
                        const lng = pos.coords.longitude;
                        try {
                            const res = await fetch(`https://api.bigdatacloud.net/data/reverse-geocode-client?latitude=${lat}&longitude=${lng}&localityLanguage=ar`);
                            const data = await res.json();
                            const detectedCity = data.city || data.locality || data.principalSubdivision || "موقعي الحالي";
                            fetchPrayerTimesByCoords(lat, lng, detectedCity);
                        } catch(e) {
                            fetchPrayerTimesByCoords(lat, lng, "موقعي الحالي");
                        }
                    },
                    (err) => {
                        fetchPrayerTimesByCity("Makkah");
                    },
                    { enableHighAccuracy: true, timeout: 8000 }
                );
            } else {
                fetchPrayerTimesByCity("Makkah");
            }
        }

        async function fetchPrayerTimesByCity(city) {
            try {
                const res = await fetch(`https://api.aladhan.com/v1/timingsByCity?city=${encodeURIComponent(city)}&country=Saudi%20Arabia&method=4`);
                const data = await res.json();
                processPrayerData(data, city === 'Makkah' ? 'مكة المكرمة' : city);
            } catch (e) {
                showPrayerError();
            }
        }

        async function fetchPrayerTimesByCoords(lat, lng, labelName) {
            try {
                const timestamp = Math.floor(Date.now() / 1000);
                const res = await fetch(`https://api.aladhan.com/v1/timings/${timestamp}?latitude=${lat}&longitude=${lng}&method=4`);
                const data = await res.json();
                processPrayerData(data, labelName);
            } catch (e) {
                showPrayerError();
            }
        }

        function processPrayerData(data, cityName) {
            if (data && data.code === 200) {
                const timings = data.data.timings;
                todayTimings = timings;
                const dateObj = data.data.date;
                
                const cityDisp = document.getElementById('prayer-city-display');
                if (cityDisp) cityDisp.innerText = cityName;

                const dateDisplay = document.getElementById('prayer-date-display');
                if (dateDisplay) {
                    dateDisplay.innerText = `${dateObj.hijri.weekday.ar}، ${dateObj.hijri.day} ${dateObj.hijri.month.ar} ${dateObj.hijri.year} هـ (${dateObj.gregorian.date})`;
                }
                
                const prayers = [
                    { name: 'الفجر', time: formatTime12(timings.Fajr), raw: timings.Fajr, icon: 'fa-cloud-sun' },
                    { name: 'الشروق', time: formatTime12(timings.Sunrise), raw: timings.Sunrise, icon: 'fa-sun' },
                    { name: 'الظهر', time: formatTime12(timings.Dhuhr), raw: timings.Dhuhr, icon: 'fa-solid fa-sun' },
                    { name: 'العصر', time: formatTime12(timings.Asr), raw: timings.Asr, icon: 'fa-cloud-sun-rain' },
                    { name: 'المغرب', time: formatTime12(timings.Maghrib), raw: timings.Maghrib, icon: 'fa-moon' },
                    { name: 'العشاء', time: formatTime12(timings.Isha), raw: timings.Isha, icon: 'fa-solid fa-moon' }
                ];

                const grid = document.getElementById('prayer-times-grid');
                if (grid) {
                    grid.innerHTML = prayers.map(p => `
                        <div class="glass-card rounded-2xl p-4 text-center flex flex-col items-center justify-center gap-2 border border-emerald-700/60 shadow-xl">
                            <i class="fa-solid ${p.icon} text-goldRoyal-400 text-xl"></i>
                            <span class="text-xs text-emerald-300 font-bold">${p.name}</span>
                            <span class="text-base font-black text-white font-mono dir-ltr">${p.time}</span>
                        </div>
                    `).join('');
                }
                updateCountdown();
            } else {
                showPrayerError();
            }
        }

        function formatTime12(time24) {
            if (!time24) return '';
            const cleanTime = time24.split(' ')[0];
            let [h, m] = cleanTime.split(':').map(Number);
            const period = h >= 12 ? 'م' : 'ص';
            h = h % 12 || 12;
            return `${h}:${String(m).padStart(2, '0')} ${period}`;
        }

        function showPrayerError() {
            const grid = document.getElementById('prayer-times-grid');
            if (grid) {
                grid.innerHTML = `<div class="col-span-full text-center py-6 text-emerald-300 text-xs">تعذر جلب مواقيت الصلاة، يرجى المحاولة لاحقاً</div>`;
            }
        }

        function updateCountdown() {
            if (!todayTimings) return;

            const now = new Date();
            const pList = [
                { name: 'الفجر', time: todayTimings.Fajr },
                { name: 'الشروق', time: todayTimings.Sunrise },
                { name: 'الظهر', time: todayTimings.Dhuhr },
                { name: 'العصر', time: todayTimings.Asr },
                { name: 'المغرب', time: todayTimings.Maghrib },
                { name: 'العشاء', time: todayTimings.Isha }
            ];

            let nextP = null;
            let diffMs = Infinity;

            for (let p of pList) {
                const [h, m] = p.time.split(' ')[0].split(':').map(Number);
                const pDate = new Date();
                pDate.setHours(h, m, 0, 0);

                const diff = pDate - now;
                if (diff > 0 && diff < diffMs) {
                    diffMs = diff;
                    nextP = p.name;
                }
            }

            if (!nextP) {
                nextP = 'الفجر';
                const [h, m] = todayTimings.Fajr.split(' ')[0].split(':').map(Number);
                const tomorrow = new Date();
                tomorrow.setDate(tomorrow.getDate() + 1);
                tomorrow.setHours(h, m, 0, 0);
                diffMs = tomorrow - now;
            }

            const titleEl = document.getElementById('next-prayer-title');
            const countdownEl = document.getElementById('next-prayer-countdown');

            if (titleEl) titleEl.innerText = `المتبقي لصلاة ${nextP}`;

            if (countdownEl && diffMs > 0) {
                const totalSeconds = Math.floor(diffMs / 1000);
                const hrs = String(Math.floor(totalSeconds / 3600)).padStart(2, '0');
                const mins = String(Math.floor((totalSeconds % 3600) / 60)).padStart(2, '0');
                const secs = String(totalSeconds % 60).padStart(2, '0');
                countdownEl.innerText = `${hrs}:${mins}:${secs}`;
            }
        }

        async function sendChatMessage() {
            const input = document.getElementById('chat-input');
            if (!input) return;
            const msg = input.value.trim();
            if (!msg) return;

            const chatContainer = document.getElementById('chat-messages');
            if (!chatContainer) return;

            chatContainer.innerHTML += `
                <div class="glass-card bg-goldRoyal-500/15 text-white p-4 rounded-2xl border border-goldRoyal-500/40 max-w-[85%] ml-auto text-right shadow">
                    <span class="text-goldRoyal-400 font-bold block mb-1">أنت:</span>
                    ${msg}
                </div>
            `;
            input.value = '';
            chatContainer.scrollTop = chatContainer.scrollHeight;

            const loadingId = 'loading-' + Date.now();
            chatContainer.innerHTML += `
                <div id="${loadingId}" class="glass-card p-3.5 rounded-2xl border border-emerald-800/80 max-w-[85%] text-emerald-300 text-xs flex items-center gap-2">
                    <i class="fa-solid fa-spinner fa-spin text-goldRoyal-400"></i> جاري استشارة الذكاء الاصطناعي...
                </div>
            `;
            chatContainer.scrollTop = chatContainer.scrollHeight;

            try {
                const systemPrompt = "أنت مساعد إسلامي عالم وثقة متخصص في الأذكار النبوية، أدعية حصن المسلم، فقه العبادات، والأحكام. أجب بلغة عربية فصحى مبسطة مع ذكر الأدلة من الكتاب والسنة.";
                const apiKey = "";
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-3-flash-preview:generateContent?key=${apiKey}`;

                const payload = {
                    contents: [{ role: 'user', parts: [{ text: msg }] }],
                    systemInstruction: { parts: [{ text: systemPrompt }] }
                };

                const response = await fetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });
                const result = await response.json();
                const loadEl = document.getElementById(loadingId);
                if (loadEl) loadEl.remove();

                const candidate = result.candidates?.[0];
                if (candidate && candidate.content?.parts?.[0]?.text) {
                    const replyText = candidate.content.parts[0].text;
                    chatContainer.innerHTML += `
                        <div class="glass-card bg-emerald-950/95 p-4 rounded-2xl border border-emerald-800/80 max-w-[85%] text-slate-200 leading-relaxed shadow space-y-1.5">
                            <span class="text-goldRoyal-400 font-bold block"><i class="fa-solid fa-robot"></i> المستشار الإسلامي الذكي:</span>
                            <p>${replyText.replace(/\n/g, '<br>')}</p>
                        </div>
                    `;
                } else {
                    throw new Error();
                }
            } catch (e) {
                const loadEl = document.getElementById(loadingId);
                if (loadEl) loadEl.remove();
                chatContainer.innerHTML += `
                    <div class="glass-card p-3.5 rounded-2xl border border-red-500/40 max-w-[85%] text-slate-200 text-xs">
                        عذراً، أواجه مشكلة مؤقتة في الاتصال. يمكنك طرح سؤالك مرة أخرى.
                    </div>
                `;
            }
            chatContainer.scrollTop = chatContainer.scrollHeight;
        }

        function sendQuickPrompt(promptText) {
            const input = document.getElementById('chat-input');
            if (input) input.value = promptText;
            switchTab('advisor');
            sendChatMessage();
        }

        function clearChat() {
            const chatContainer = document.getElementById('chat-messages');
            if (chatContainer) {
                chatContainer.innerHTML = `
                    <div class="glass-card p-4 rounded-2xl border border-emerald-800/80 max-w-[85%] text-slate-200 leading-relaxed shadow">
                        <span class="text-goldRoyal-400 font-bold block mb-1"><i class="fa-star fa-solid"></i> أهلاً بك:</span>
                        تم مسح المحادثة بنجاح. كيف يمكنني مساعدتك اليوم؟
                    </div>
                `;
            }
        }
    </script>
</body>
</html>