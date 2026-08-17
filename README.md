
<html lang="bn">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SS Network · ISP</title>
  
  <!-- Favicon Link -->
  <link rel="icon" type="image/x-icon" href="favicon.ico" />

  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- Google Fonts: Poppins + Kalpurush -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700;800&family=Kalpurush:wght@400;500;600;700&display=swap" rel="stylesheet" />
  
  <!-- Font Awesome 6 -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Kalpurush', 'Poppins', sans-serif;
      background: #ffffff;
      color: #1a1a1a;
      scroll-behavior: smooth;
    }
    h1, h2, h3, h4, .font-poppins {
      font-family: 'Poppins', sans-serif;
    }
    
    /* ========== Kalpurush ফন্ট ========== */
    p, li, label, select, input, textarea, .description, .service-text, 
    .form-label, .btn-submit, .text-base, .text-sm, .text-xs,
    .font-medium, .font-semibold, .font-bold {
      font-family: 'Kalpurush', sans-serif !important;
    }
    
    /* প্যারাগ্রাফ টেক্সট বড়, গাঢ় ও স্পষ্ট */
    p, li, label, select, input, textarea, .description, .service-text {
      font-size: 18px !important;
      font-weight: 500 !important;
      line-height: 1.9 !important;
      color: #1a1a1a !important;
    }
    
    /* ছোট টেক্সটের জন্য */
    .text-xs, .text-sm {
      font-size: 15px !important;
      font-weight: 400 !important;
      line-height: 1.6 !important;
    }
    
    /* প্যাকেজের লিস্ট আইটেমগুলো */
    .space-y-2 li, .space-y-2\.5 li {
      font-size: 17px !important;
      font-weight: 500 !important;
    }

    /* ========== SS NETWORK নীল করা ========== */
    .ss-network-blue {
      color: #2196F3 !important;
    }

    /* ========== ফুটার টেক্সট দৃশ্যমান করা ========== */
    footer p, footer li, footer a, footer span, footer h4 {
      color: #d1d5db !important;
    }
    footer a:hover {
      color: #ffffff !important;
    }
    footer .text-white {
      color: #ffffff !important;
    }
    footer .text-red-primary {
      color: #E31E24 !important;
    }
    footer .fa-map-marker-alt {
      color: #E31E24 !important;
    }

    .bg-red-primary { background-color: #E31E24; }
    .text-red-primary { color: #E31E24; }
    .border-red-primary { border-color: #E31E24; }
    .bg-blue-primary { background-color: #2196F3; }
    .text-blue-primary { color: #2196F3; }
    .bg-green-primary { background-color: #4CAF50; }
    .text-green-primary { color: #4CAF50; }
    .bg-orange-primary { background-color: #FF6600; }
    .text-orange-primary { color: #FF6600; }
    .bg-purple-primary { background-color: #8E24AA; }
    .text-purple-primary { color: #8E24AA; }
    .bg-yellow-primary { background-color: #D81B60; }
    .text-yellow-primary { color: #D81B60; }

    .gradient-accent {
      background: linear-gradient(135deg, #E31E24, #FF6600, #2196F3, #4CAF50);
      background-size: 300% 300%;
      animation: gradientMove 6s ease infinite;
    }
    @keyframes gradientMove {
      0% { background-position: 0% 0%; }
      50% { background-position: 100% 100%; }
      100% { background-position: 0% 0%; }
    }

    .header-scrolled {
      background: rgba(255, 255, 255, 0.95) !important;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.07);
      backdrop-filter: blur(4px);
    }

    /* FLOATING WHATSAPP - RIGHT SIDE */
    .whatsapp-float {
      position: fixed;
      bottom: 28px;
      right: 28px;
      z-index: 9999;
      background: #25D366;
      width: 64px;
      height: 64px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-size: 36px;
      box-shadow: 0 6px 20px rgba(37, 211, 102, 0.4);
      transition: 0.25s ease;
      text-decoration: none;
      animation: pulse-bounce 2.2s infinite;
    }
    .whatsapp-float:hover {
      transform: scale(1.08);
      background: #20b85f;
      box-shadow: 0 10px 28px rgba(37, 211, 102, 0.5);
    }
    .whatsapp-float .tooltip {
      position: absolute;
      right: 72px;
      background: rgba(0, 0, 0, 0.75);
      color: #fff;
      padding: 6px 16px;
      border-radius: 40px;
      font-size: 14px;
      white-space: nowrap;
      opacity: 0;
      pointer-events: none;
      transition: 0.2s;
      font-family: 'Poppins', sans-serif;
      font-weight: 500;
    }
    .whatsapp-float:hover .tooltip { opacity: 1; }
    @keyframes pulse-bounce {
      0% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.5); }
      70% { box-shadow: 0 0 0 20px rgba(37, 211, 102, 0); }
      100% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0); }
    }

    .card-hover {
      transition: transform 0.25s ease, box-shadow 0.3s ease;
    }
    .card-hover:hover {
      transform: translateY(-6px);
      box-shadow: 0 20px 35px -10px rgba(0, 0, 0, 0.12);
    }

    .mobile-menu {
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.35s ease;
    }
    .mobile-menu.open { max-height: 380px; }

    .bg-soft-gray { background-color: #F8F9FA; }
    .text-dark { color: #1a1a1a; }

    .form-input {
      width: 100%;
      padding: 12px 16px;
      border: 1px solid #e2e8f0;
      border-radius: 12px;
      font-size: 1.05rem;
      transition: 0.2s;
      background: white;
      font-family: 'Kalpurush', sans-serif !important;
    }
    .form-input:focus {
      outline: none;
      border-color: #E31E24;
      box-shadow: 0 0 0 3px rgba(227, 30, 36, 0.1);
    }
    .form-label {
      display: block;
      font-weight: 600;
      margin-bottom: 6px;
      color: #1a1a1a;
      font-size: 1.05rem;
    }
    .btn-submit {
      background: #E31E24;
      color: white;
      font-weight: 700;
      padding: 14px 32px;
      border-radius: 50px;
      border: none;
      font-size: 1.15rem;
      cursor: pointer;
      transition: 0.2s;
      width: 100%;
      font-family: 'Kalpurush', sans-serif !important;
    }
    .btn-submit:hover {
      background: #b8151a;
      transform: scale(1.01);
      box-shadow: 0 8px 20px rgba(227, 30, 36, 0.3);
    }

    /* THANK YOU MODAL OVERLAY */
    .thankyou-overlay {
      position: fixed;
      inset: 0;
      background: rgba(0, 0, 0, 0.6);
      backdrop-filter: blur(5px);
      z-index: 99999;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
    }
    .thankyou-overlay.active { display: flex; }
    .thankyou-card {
      background: white;
      max-width: 440px;
      width: 100%;
      padding: 40px 28px;
      border-radius: 24px;
      text-align: center;
      box-shadow: 0 25px 50px rgba(0, 0, 0, 0.25);
      animation: popIn 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }
    @keyframes popIn {
      0% { transform: scale(0.8); opacity: 0; }
      100% { transform: scale(1); opacity: 1; }
    }
    .thankyou-card i { font-size: 60px; color: #4CAF50; margin-bottom: 16px; }

    /* ========== SLIDER SECTION STYLES ========== */
    .slider-container {
      width: 100%;
      max-width: 1280px;
      margin: 0 auto;
      padding: 0 16px;
      position: relative;
      overflow: hidden;
      background: #f9fafb;
    }

    .slider-wrapper {
      position: relative;
      width: 100%;
      aspect-ratio: 16 / 9;
      overflow: hidden;
      border-radius: 20px;
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.08);
      background: #e5e7eb;
    }

    .slider-track {
      display: flex;
      transition: transform 0.6s cubic-bezier(0.25, 0.46, 0.45, 0.94);
      height: 100%;
      width: 100%;
      will-change: transform;
    }

    .slide {
      flex: 0 0 100%;
      height: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      background: #e5e7eb;
    }

    .slide img {
      display: block;
      width: 100%;
      height: 100%;
      object-fit: cover;
      aspect-ratio: 16 / 9;
      background: #d1d5db;
    }

    .slider-btn {
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      background: rgba(255, 255, 255, 0.85);
      backdrop-filter: blur(4px);
      border: none;
      width: 44px;
      height: 44px;
      border-radius: 50%;
      font-size: 20px;
      color: #1a1a1a;
      cursor: pointer;
      z-index: 20;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      transition: 0.2s;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .slider-btn:hover {
      background: white;
      transform: translateY(-50%) scale(1.05);
      box-shadow: 0 6px 16px rgba(0,0,0,0.15);
    }
    .slider-btn.prev { left: 16px; }
    .slider-btn.next { right: 16px; }

    .slider-dots {
      display: flex;
      justify-content: center;
      gap: 12px;
      margin-top: 16px;
      padding-bottom: 8px;
      flex-wrap: wrap;
    }
    .slider-dot {
      width: 14px;
      height: 14px;
      border-radius: 50%;
      background: #d1d5db;
      border: none;
      cursor: pointer;
      transition: 0.25s;
      padding: 0;
    }
    .slider-dot.active {
      background: #E31E24;
      transform: scale(1.2);
      box-shadow: 0 0 0 4px rgba(227, 30, 36, 0.15);
    }
    .slider-dot:hover {
      background: #a0aec0;
    }
    .slider-dot.active:hover {
      background: #E31E24;
    }

    @media (max-width: 640px) {
      .slider-container {
        padding: 0 8px;
      }
      .slider-wrapper {
        border-radius: 14px;
      }
      .slider-btn {
        width: 36px;
        height: 36px;
        font-size: 16px;
      }
      .slider-btn.prev { left: 8px; }
      .slider-btn.next { right: 8px; }
      .slider-dots {
        gap: 10px;
        margin-top: 12px;
      }
      .slider-dot {
        width: 12px;
        height: 12px;
      }
    }

    .slider-wrapper {
      touch-action: pan-y;
      user-select: none;
      -webkit-user-select: none;
    }
  </style>
</head>
<body>

  <!-- ========== HEADER ========== -->
  <header id="mainHeader" class="fixed top-0 left-0 w-full z-50 bg-white/90 transition-all duration-300 border-b border-gray-100">
    <div class="max-w-7xl mx-auto px-4 md:px-8 flex items-center justify-between h-20">
      <div class="flex items-center gap-2.5">
        <div class="flex items-center gap-2">
          <img src="logo.png" alt="SS Network Logo" class="w-11 h-11 object-contain rounded-full shadow-sm" onerror="this.onerror=null; this.src='https://via.placeholder.com/44?text=SS';" />
          <div class="leading-tight">
            <span class="font-poppins font-bold text-xl tracking-wide text-dark">SS NETWORK</span>
            <span class="block text-[10px] font-medium text-gray-500 tracking-widest">WE ALWAYS PROVIDE BEST SERVICE</span>
          </div>
        </div>
      </div>

      <nav class="hidden md:flex items-center gap-8 font-poppins font-medium text-sm text-gray-700">
        <a href="#home" class="hover:text-red-primary transition">Home</a>
        <a href="#why" class="hover:text-red-primary transition">Why SS</a>
        <a href="#packages" class="hover:text-red-primary transition">Packages</a>
        <a href="#contact" class="hover:text-red-primary transition">Contact</a>
      </nav>

      <div class="flex items-center gap-4">
        <a href="tel:01716729140" class="hidden md:flex items-center gap-1.5 bg-red-primary/10 text-red-primary font-semibold px-4 py-2 rounded-full text-sm hover:bg-red-primary hover:text-white transition">
          <i class="fas fa-phone"></i> <span>01716729140</span>
        </a>
        <button id="menuToggle" class="md:hidden text-2xl text-gray-700 focus:outline-none" aria-label="menu">
          <i class="fas fa-bars"></i>
        </button>
      </div>
    </div>

    <!-- মোবাইল মেনু -->
    <div id="mobileMenu" class="mobile-menu md:hidden bg-white px-4 pb-4 border-t border-gray-100">
      <div class="flex flex-col gap-3 font-poppins font-medium text-gray-700 text-base pt-3">
        <a href="#home" class="hover:text-red-primary py-1 border-b border-gray-50">Home</a>
        <a href="#why" class="hover:text-red-primary py-1 border-b border-gray-50">Why SS</a>
        <a href="#packages" class="hover:text-red-primary py-1 border-b border-gray-50">Packages</a>
        <a href="#contact" class="hover:text-red-primary py-1 border-b border-gray-50">Contact</a>
        
        <a href="tel:01716729140" class="mt-2 bg-red-primary/10 text-red-primary font-semibold px-4 py-2 rounded-full text-center flex items-center justify-center gap-2">
          <i class="fas fa-phone"></i> <span>01716729140</span>
        </a>
      </div>
    </div>
  </header>

  <!-- ============================================================ -->
  <!-- ========== SLIDER SECTION (হেডার ও হিরোর মাঝে) ========= -->
  <!-- ============================================================ -->
  <section class="slider-container pt-28 md:pt-36 pb-4">
    <div class="slider-wrapper" id="sliderWrapper">
      <div class="slider-track" id="sliderTrack">
        
        <!-- ===== আপনার GitHub ইমেজ এখানে বসান ===== -->
        <!-- Slide 1 -->
        <div class="slide">
          <img src="slide1.jpg" alt="SS Network অফার ১" loading="lazy" />
        </div>
        <!-- Slide 2 -->
        <div class="slide">
          <img src="slide2.jpg" alt="SS Network অফার ২" loading="lazy" />
        </div>
        <!-- Slide 3 -->
        <div class="slide">
          <img src="slide3.jpg" alt="SS Network অফার ৩" loading="lazy" />
        </div>
        <!-- Slide 4 -->
        <div class="slide">
          <img src="slide4.jpg" alt="SS Network অফার ৪" loading="lazy" />
        </div>
        <!-- Slide 5 -->
        <div class="slide">
          <img src="slide5.jpg" alt="SS Network অফার ৫" loading="lazy" />
        </div>
        <!-- ===== ইমেজ শেষ ===== -->
        
      </div>

      <!-- Prev / Next Buttons -->
      <button class="slider-btn prev" id="prevBtn" aria-label="Previous slide">
        <i class="fas fa-chevron-left"></i>
      </button>
      <button class="slider-btn next" id="nextBtn" aria-label="Next slide">
        <i class="fas fa-chevron-right"></i>
      </button>
    </div>

    <!-- Dots / Indicators -->
    <div class="slider-dots" id="sliderDots"></div>
  </section>

  <!-- ========== HERO SECTION ========== -->
  <section id="home" class="pt-8 pb-8 bg-gradient-to-br from-red-50 via-blue-50/20 to-white">
    <div class="max-w-6xl mx-auto px-4 md:px-8 flex flex-col md:flex-row items-center gap-10">
      <div class="flex-1 text-center md:text-left">
        <h1 class="font-poppins font-extrabold text-3xl sm:text-4xl md:text-5xl lg:text-5xl leading-tight text-dark max-w-fit mx-auto md:mx-0">
          <span class="block whitespace-nowrap">হাই-স্পিড ইন্টারনেট</span>
          <span class="block whitespace-nowrap text-red-primary mt-1">এখন আপনার শহরে</span>
        </h1>
        
        <div class="mt-4 text-lg md:text-xl font-semibold text-gray-700">
          <span class="gradient-accent text-transparent bg-clip-text">WE ALWAYS PROVIDE BEST SERVICE</span>
        </div>

        <div class="mt-8 flex flex-wrap gap-4 justify-center md:justify-start">
          <a href="#packages" class="bg-red-primary hover:bg-red-700 text-white font-semibold px-8 py-3.5 rounded-full shadow-lg transition flex items-center gap-2">
            <i class="fas fa-wifi"></i> প্যাকেজ দেখুন
          </a>
          <a href="https://wa.me/8801716729140" target="_blank" class="bg-green-primary hover:bg-green-700 text-white font-semibold px-8 py-3.5 rounded-full shadow-lg transition flex items-center gap-2">
            <i class="fab fa-whatsapp"></i> যোগাযোগ করুন
          </a>
        </div>
      </div>

      <div class="flex-1 flex justify-center mt-2 md:mt-0">
        <div class="w-56 h-56 md:w-72 md:h-72 rounded-full gradient-accent opacity-20 blur-3xl"></div>
      </div>
    </div>
  </section>

  <!-- ========== WHY SS NETWORK SECTION ========== -->
  <section id="why" class="py-14 bg-white border-t border-gray-100">
    <div class="max-w-6xl mx-auto px-4">
      <h2 class="font-poppins font-bold text-3xl md:text-4xl text-center text-dark mb-3">
        কেন <span class="ss-network-blue">SS NETWORK</span> ব্যবহার করবেন?
      </h2>
      <p class="text-center text-gray-600 text-base md:text-lg mb-12 max-w-2xl mx-auto">আমরা গ্রাহকদের সর্বোচ্চ মানের সেবা নিশ্চিত করতে সর্বদা প্রস্তুত। দেখে নিন কেন আমরা সেরা:</p>

      <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
        <div class="bg-soft-gray p-6 rounded-2xl card-hover border-t-4 border-red-primary">
          <div class="text-red-primary text-3xl mb-4"><i class="fas fa-tachometer-alt"></i></div>
          <h3 class="font-bold text-lg mb-3 border-b pb-2">স্পিড ও কানেকশন</h3>
          <ul class="space-y-2.5 text-gray-700">
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>হাই-স্পিড, স্টেবল কানেকশন — কোনো বাফারিং নেই</li>
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>লো ল্যাটেন্সি — গেমিং ও অনলাইন ক্লাসের জন্য পারফেক্ট</li>
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>২৪ ঘণ্টা আনলিমিটেড ডেটা, কোনো FUP লিমিট নেই</li>
          </ul>
        </div>

        <div class="bg-soft-gray p-6 rounded-2xl card-hover border-t-4 border-blue-primary">
          <div class="text-blue-primary text-3xl mb-4"><i class="fas fa-headset"></i></div>
          <h3 class="font-bold text-lg mb-3 border-b pb-2">সার্ভিস ও সাপোর্ট</h3>
          <ul class="space-y-2.5 text-gray-700">
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>২৪/৭ কাস্টমার সাপোর্ট — যেকোনো সমস্যায় সাথে সাথে সমাধান</li>
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>দ্রুত টেকনিক্যাল টিম রেসপন্স</li>
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>সহজ পেমেন্ট সিস্টেম (bKash/Nagad/ক্যাশ)</li>
          </ul>
        </div>

        <div class="bg-soft-gray p-6 rounded-2xl card-hover border-t-4 border-orange-primary">
          <div class="text-orange-primary text-3xl mb-4"><i class="fas fa-shield-alt"></i></div>
          <h3 class="font-bold text-lg mb-3 border-b pb-2">মূল্য ও বিশ্বাসযোগ্যতা</h3>
          <ul class="space-y-2.5 text-gray-700">
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>সাশ্রয়ী মূল্যে সেরা সার্ভিস — কোনো হিডেন চার্জ নেই</li>
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>লোকাল এরিয়ার মধ্যে বিশ্বস্ত ও পরিচিত প্রোভাইডার</li>
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>নমনীয় প্যাকেজ — প্রয়োজন অনুযায়ী প্যাকেজ পরিবর্তনের সুবিধা</li>
          </ul>
        </div>

        <div class="bg-soft-gray p-6 rounded-2xl card-hover border-t-4 border-green-primary">
          <div class="text-green-primary text-3xl mb-4"><i class="fas fa-network-wired"></i></div>
          <h3 class="font-bold text-lg mb-3 border-b pb-2">ইনফ্রাস্ট্রাকচার</h3>
          <ul class="space-y-2.5 text-gray-700">
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>আধুনিক ফাইবার অপটিক নেটওয়ার্ক</li>
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>৯৯.৯% আপটাইম গ্যারান্টি</li>
            <li><i class="fas fa-check-circle text-green-500 mr-2"></i>ওয়েদার-প্রুফ স্টেবল কানেকশন (বৃষ্টি/ঝড়েও নেট বন্ধ হয় না)</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== PACKAGES SECTION ========== -->
  <section id="packages" class="py-16 bg-soft-gray border-t border-gray-200/60">
    <div class="max-w-6xl mx-auto px-4">
      <h2 class="font-poppins font-bold text-4xl text-center text-dark mb-2">আমাদের <span class="text-red-primary">প্যাকেজ</span></h2>
      <p class="text-center text-gray-600 text-base md:text-lg mb-12">আপনার পছন্দ অনুযায়ী যেকোনো প্যাকেজ বেছে নিন</p>
      
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- 20 Mbps -->
        <div class="bg-white rounded-2xl p-6 shadow-md card-hover border-t-4 border-blue-primary flex flex-col justify-between">
          <div>
            <h3 class="font-poppins font-bold text-2xl">20 Mbps</h3>
            <div class="text-3xl font-poppins font-bold text-red-primary mt-1">৳৫০০ <span class="text-sm font-normal text-gray-500">/মাস</span></div>
            <ul class="mt-4 space-y-2 text-gray-700">
              <li><i class="fas fa-check text-green-primary mr-2"></i>আনলিমিটেড ডেটা</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>২৪/৭ সাপোর্ট</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>ফাইবার অপটিক সংযোগ</li>
            </ul>
          </div>
          <a href="#contact" class="mt-6 block text-center bg-blue-primary hover:bg-blue-600 text-white font-semibold py-2.5 rounded-full transition">সংযোগ নিন</a>
        </div>

        <!-- 30 Mbps -->
        <div class="bg-white rounded-2xl p-6 shadow-xl card-hover border-t-4 border-orange-primary flex flex-col justify-between relative">
          <span class="absolute -top-3 left-1/2 -translate-x-1/2 bg-orange-primary text-white text-xs font-bold px-3 py-1 rounded-full">Most Popular</span>
          <div>
            <h3 class="font-poppins font-bold text-2xl">30 Mbps</h3>
            <div class="text-3xl font-poppins font-bold text-red-primary mt-1">৳৬৫০ <span class="text-sm font-normal text-gray-500">/মাস</span></div>
            <ul class="mt-4 space-y-2 text-gray-700">
              <li><i class="fas fa-check text-green-primary mr-2"></i>আনলিমিটেড ডেটা</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>২৪/৭ সাপোর্ট</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>হাই-স্পিড ফাইবার</li>
            </ul>
          </div>
          <a href="#contact" class="mt-6 block text-center bg-orange-primary hover:bg-orange-600 text-white font-semibold py-2.5 rounded-full transition">সংযোগ নিন</a>
        </div>

        <!-- 50 Mbps -->
        <div class="bg-white rounded-2xl p-6 shadow-md card-hover border-t-4 border-green-primary flex flex-col justify-between">
          <div>
            <h3 class="font-poppins font-bold text-2xl">50 Mbps</h3>
            <div class="text-3xl font-poppins font-bold text-red-primary mt-1">৳৮২০ <span class="text-sm font-normal text-gray-500">/মাস</span></div>
            <ul class="mt-4 space-y-2 text-gray-700">
              <li><i class="fas fa-check text-green-primary mr-2"></i>আনলিমিটেড ডেটা</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>২৪/৭ সাপোর্ট</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>গেমিং ও স্ট্রিমিং</li>
            </ul>
          </div>
          <a href="#contact" class="mt-6 block text-center bg-green-primary hover:bg-green-600 text-white font-semibold py-2.5 rounded-full transition">সংযোগ নিন</a>
        </div>

        <!-- 70 Mbps -->
        <div class="bg-white rounded-2xl p-6 shadow-md card-hover border-t-4 border-red-primary flex flex-col justify-between">
          <div>
            <h3 class="font-poppins font-bold text-2xl">70 Mbps</h3>
            <div class="text-3xl font-poppins font-bold text-red-primary mt-1">৳৯৯৯ <span class="text-sm font-normal text-gray-500">/মাস</span></div>
            <ul class="mt-4 space-y-2 text-gray-700">
              <li><i class="fas fa-check text-green-primary mr-2"></i>আনলিমিটেড ডেটা</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>২৪/৭ সাপোর্ট</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>আল্ট্রা ফাস্ট ফাইবার</li>
            </ul>
          </div>
          <a href="#contact" class="mt-6 block text-center bg-red-primary hover:bg-red-700 text-white font-semibold py-2.5 rounded-full transition">সংযোগ নিন</a>
        </div>

        <!-- সিলভার (Silver) - 85 Mbps -->
        <div class="bg-white rounded-2xl p-6 shadow-md card-hover border-t-4 border-purple-primary flex flex-col justify-between">
          <div>
            <div class="flex justify-between items-center">
              <h3 class="font-poppins font-bold text-2xl">85 Mbps</h3>
              <span class="bg-purple-primary/10 text-purple-primary text-xs font-bold px-2.5 py-1 rounded-full">Silver</span>
            </div>
            <div class="text-3xl font-poppins font-bold text-red-primary mt-1">৳১০৯৯ <span class="text-sm font-normal text-gray-500">/মাস</span></div>
            <ul class="mt-4 space-y-2 text-gray-700">
              <li><i class="fas fa-check text-green-primary mr-2"></i>আনলিমিটেড ডেটা</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>২৪/৭ প্রাইওরিটি সাপোর্ট</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>হেভি ডাউনলোডিং ও 4K স্ট্রিমিং</li>
            </ul>
          </div>
          <a href="#contact" class="mt-6 block text-center bg-purple-primary hover:bg-purple-700 text-white font-semibold py-2.5 rounded-full transition">সংযোগ নিন</a>
        </div>

        <!-- গোল্ড (Gold) - 100 Mbps -->
        <div class="bg-white rounded-2xl p-6 shadow-md card-hover border-t-4 border-yellow-primary flex flex-col justify-between">
          <div>
            <div class="flex justify-between items-center">
              <h3 class="font-poppins font-bold text-2xl">100 Mbps</h3>
              <span class="bg-yellow-primary/10 text-yellow-primary text-xs font-bold px-2.5 py-1 rounded-full">Gold</span>
            </div>
            <div class="text-3xl font-poppins font-bold text-red-primary mt-1">৳১২০০ <span class="text-sm font-normal text-gray-500">/মাস</span></div>
            <ul class="mt-4 space-y-2 text-gray-700">
              <li><i class="fas fa-check text-green-primary mr-2"></i>আনলিমিটেড ডেটা</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>ডেডিকেটেড VIP সাপোর্ট</li>
              <li><i class="fas fa-check text-green-primary mr-2"></i>বাফারিং ছাড়া ৪K/৮K কন্টেন্ট</li>
            </ul>
          </div>
          <a href="#contact" class="mt-6 block text-center bg-yellow-primary hover:bg-yellow-700 text-white font-semibold py-2.5 rounded-full transition">সংযোগ নিন</a>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== CONTACT FORM SECTION ========== -->
  <section id="contact" class="py-16 bg-white">
    <div class="max-w-3xl mx-auto px-4">
      <h2 class="font-poppins font-bold text-3xl md:text-4xl text-center text-dark mb-2">নতুন কানেকশনের জন্য <span class="text-red-primary">যোগাযোগ করুন</span></h2>
      <p class="text-center text-gray-600 text-base md:text-lg mb-10">নিচের ফর্মটি পূরণ করুন, আমরা আপনার সাথে দ্রুত যোগাযোগ করবো</p>

      <div class="bg-soft-gray p-6 sm:p-10 rounded-3xl shadow-sm border border-gray-100">
        <form id="connectionForm">
          <div class="space-y-4">
            <div>
              <label class="form-label" for="userName">নাম :</label>
              <input type="text" id="userName" class="form-input" placeholder="আপনার পুরো নাম লিখুন" required />
            </div>

            <div>
              <label class="form-label" for="userMobile">মোবাইল নাম্বার :</label>
              <input type="tel" id="userMobile" class="form-input" placeholder="01XXXXXXXXX" required />
            </div>

            <div>
              <label class="form-label" for="userEmail">ইমেইল :</label>
              <input type="email" id="userEmail" class="form-input" placeholder="example@mail.com" />
            </div>

            <div>
              <label class="form-label" for="userAddress">সম্পূর্ণ ঠিকানা :</label>
              <textarea id="userAddress" class="form-input" rows="2" placeholder="আপনার বিস্তারিত ঠিকানা লিখুন" required></textarea>
            </div>

            <div>
              <label class="form-label" for="connectionType">কানেকশন টাইপ :</label>
              <select id="connectionType" class="form-input cursor-pointer">
                <option value="হোম" selected>হোম</option>
                <option value="অফিস">অফিস</option>
                <option value="শপ">শপ</option>
                <option value="কর্পোরেট">কর্পোরেট</option>
              </select>
            </div>

            <div>
              <label class="form-label" for="packageSelect">প্যাকেজ সিলেক্ট :</label>
              <select id="packageSelect" class="form-input cursor-pointer">
                <option value="20 Mbps - ৳৫০০/মাস">20 Mbps (৳৫০০/মাস)</option>
                <option value="30 Mbps - ৳৬৫০/মাস">30 Mbps (৳৬৫০/মাস)</option>
                <option value="50 Mbps - ৳৮২০/মাস">50 Mbps (৳৮২০/মাস)</option>
                <option value="70 Mbps - ৳৯৯৯/মাস">70 Mbps (৳৯৯৯/মাস)</option>
                <option value="Silver (85 Mbps) - ৳১০৯৯/মাস">Silver - 85 Mbps (৳১০৯৯/মাস)</option>
                <option value="Gold (100 Mbps) - ৳১২০০/মাস">Gold - 100 Mbps (৳১২০০/মাস)</option>
              </select>
            </div>

            <div class="pt-4">
              <button type="submit" class="btn-submit">
                Submit
              </button>
            </div>

          </div>
        </form>
      </div>
    </div>
  </section>

  <!-- ========== FOOTER ========== -->
  <footer class="bg-[#1a1a1a] pt-16 pb-6">
    <div class="max-w-6xl mx-auto px-4 grid sm:grid-cols-2 lg:grid-cols-3 gap-8">
      <div>
        <div class="flex items-center gap-2">
          <img src="logo.png" alt="SS Network Logo" class="w-10 h-10 object-contain rounded-full shadow-sm" onerror="this.onerror=null; this.src='https://via.placeholder.com/40?text=SS';" />
          <span class="font-poppins font-bold text-xl text-white">SS NETWORK</span>
        </div>
        <p class="mt-3 text-sm font-semibold text-gray-300">WE ALWAYS PROVIDE BEST SERVICE</p>
        
        <p class="mt-4 text-sm leading-relaxed text-gray-300 flex items-start gap-2">
          <i class="fas fa-map-marker-alt text-red-primary text-base mt-1"></i>
          <span class="text-gray-300">Alom House, 2nd floor, Islamia Road, Sonapur, Sadar, Noakhali.</span>
        </p>
      </div>

      <div>
        <h4 class="font-poppins font-semibold text-white mb-3">Quick Links</h4>
        <ul class="space-y-2 text-base">
          <li><a href="#home" class="text-gray-300 hover:text-white transition">Home</a></li>
          <li><a href="#why" class="text-gray-300 hover:text-white transition">Why SS</a></li>
          <li><a href="#packages" class="text-gray-300 hover:text-white transition">Packages</a></li>
          <li><a href="#contact" class="text-gray-300 hover:text-white transition">Contact</a></li>
        </ul>
      </div>

      <div>
        <h4 class="font-poppins font-semibold text-white mb-3">যোগাযোগ</h4>
        
        <p class="text-base mb-2">
          <a href="tel:01716729140" class="text-gray-300 hover:text-white transition flex items-center gap-2">
            <i class="fas fa-phone text-red-primary"></i> 01716729140
          </a>
        </p>

        <p class="text-base mb-4">
          <a href="mailto:ssnetwork41@gmail.com" class="text-gray-300 hover:text-white transition flex items-center gap-2">
            <i class="fas fa-envelope text-red-primary"></i> ssnetwork41@gmail.com
          </a>
        </p>

        <div class="flex gap-4 text-xl">
          <a href="https://www.facebook.com/share/14psW5MGT5i/" target="_blank" class="text-gray-300 hover:text-blue-500 transition" aria-label="Facebook">
            <i class="fab fa-facebook"></i>
          </a>
          <a href="https://wa.me/8801716729140" target="_blank" class="text-gray-300 hover:text-green-400 transition" aria-label="WhatsApp">
            <i class="fab fa-whatsapp"></i>
          </a>
        </div>
      </div>
    </div>

    <div class="border-t border-white/10 mt-10 pt-6 text-center text-xs text-white/40">
      © 2026 SS Network. All Rights Reserved.
    </div>
  </footer>

  <!-- ========== FLOATING WHATSAPP ========== -->
  <a href="https://wa.me/8801716729140" target="_blank" class="whatsapp-float" aria-label="WhatsApp chat">
    <i class="fab fa-whatsapp"></i>
    <span class="tooltip">WhatsApp-এ নক দিন</span>
  </a>

  <!-- ========== THANK YOU OVERLAY MODAL ========== -->
  <div id="thankYouModal" class="thankyou-overlay">
    <div class="thankyou-card">
      <i class="fas fa-check-circle"></i>
      <h3 class="font-poppins font-bold text-2xl text-dark mb-2">Thank You!</h3>
      <p class="text-gray-600 text-base mb-6">আপনার তথ্যসমূহ সফলভাবে জমা নেওয়া হয়েছে। আমাদের প্রতিনিধি শীঘ্রই আপনার দেওয়া নাম্বারে যোগাযোগ করবে।</p>
      <button id="closeModalBtn" class="bg-red-primary hover:bg-red-700 text-white font-semibold px-6 py-2.5 rounded-full transition w-full">
        ঠিক আছে
      </button>
    </div>
  </div>

  <!-- ============================================================ -->
  <!-- ========== SLIDER JAVASCRIPT ========= -->
  <!-- ============================================================ -->
  <script>
    (function() {
      "use strict";

      const track = document.getElementById('sliderTrack');
      const slides = track.querySelectorAll('.slide');
      const totalSlides = slides.length;
      const dotsContainer = document.getElementById('sliderDots');
      const prevBtn = document.getElementById('prevBtn');
      const nextBtn = document.getElementById('nextBtn');

      let currentIndex = 0;
      let autoSlideInterval = null;
      let isTransitioning = false;

      // Create dots
      function createDots() {
        dotsContainer.innerHTML = '';
        for (let i = 0; i < totalSlides; i++) {
          const dot = document.createElement('button');
          dot.className = 'slider-dot';
          dot.setAttribute('data-index', i);
          dot.setAttribute('aria-label', `Go to slide ${i+1}`);
          if (i === 0) dot.classList.add('active');
          dot.addEventListener('click', () => goToSlide(i));
          dotsContainer.appendChild(dot);
        }
      }
      createDots();

      function updateDots(index) {
        const allDots = dotsContainer.querySelectorAll('.slider-dot');
        allDots.forEach((dot, i) => {
          dot.classList.toggle('active', i === index);
        });
      }

      function goToSlide(index) {
        if (isTransitioning) return;
        if (index < 0) index = totalSlides - 1;
        if (index >= totalSlides) index = 0;
        currentIndex = index;
        const offset = -currentIndex * 100;
        track.style.transform = `translateX(${offset}%)`;
        updateDots(currentIndex);
        resetAutoSlide();
      }

      function nextSlide() {
        if (isTransitioning) return;
        goToSlide(currentIndex + 1);
      }

      function prevSlide() {
        if (isTransitioning) return;
        goToSlide(currentIndex - 1);
      }

      function startAutoSlide() {
        if (autoSlideInterval) clearInterval(autoSlideInterval);
        autoSlideInterval = setInterval(nextSlide, 4500);
      }

      function resetAutoSlide() {
        if (autoSlideInterval) {
          clearInterval(autoSlideInterval);
          startAutoSlide();
        }
      }

      function onTransitionEnd() {
        isTransitioning = false;
      }

      track.addEventListener('transitionend', onTransitionEnd);

      // --- DRAG / SWIPE ---
      let startX = 0;
      let endX = 0;
      let isDragging = false;

      function handleDragStart(e) {
        const event = e.touches ? e.touches[0] : e;
        startX = event.clientX;
        isDragging = true;
        track.style.transition = 'none';
      }

      function handleDragMove(e) {
        if (!isDragging) return;
        const event = e.touches ? e.touches[0] : e;
        const diff = event.clientX - startX;
        const currentOffset = -currentIndex * 100;
        const newOffset = currentOffset + (diff / track.parentElement.offsetWidth) * 100;
        track.style.transform = `translateX(${newOffset}%)`;
      }

      function handleDragEnd(e) {
        if (!isDragging) return;
        isDragging = false;
        track.style.transition = 'transform 0.6s cubic-bezier(0.25, 0.46, 0.45, 0.94)';
        const event = e.changedTouches ? e.changedTouches[0] : e;
        const diff = event.clientX - startX;
        const threshold = 50;
        if (diff > threshold) {
          prevSlide();
        } else if (diff < -threshold) {
          nextSlide();
        } else {
          goToSlide(currentIndex);
        }
      }

      const wrapper = document.getElementById('sliderWrapper');
      wrapper.addEventListener('mousedown', handleDragStart);
      window.addEventListener('mousemove', handleDragMove);
      window.addEventListener('mouseup', handleDragEnd);

      wrapper.addEventListener('touchstart', handleDragStart, { passive: true });
      window.addEventListener('touchmove', handleDragMove, { passive: true });
      window.addEventListener('touchend', handleDragEnd, { passive: true });

      prevBtn.addEventListener('click', prevSlide);
      nextBtn.addEventListener('click', nextSlide);

      wrapper.addEventListener('keydown', (e) => {
        if (e.key === 'ArrowLeft') prevSlide();
        if (e.key === 'ArrowRight') nextSlide();
      });
      wrapper.setAttribute('tabindex', '0');

      startAutoSlide();

      wrapper.addEventListener('mouseenter', () => {
        if (autoSlideInterval) clearInterval(autoSlideInterval);
      });
      wrapper.addEventListener('mouseleave', () => {
        if (autoSlideInterval) clearInterval(autoSlideInterval);
        startAutoSlide();
      });

      window.addEventListener('beforeunload', function() {
        if (autoSlideInterval) clearInterval(autoSlideInterval);
      });

    })();
  </script>

  <!-- ========== MAIN JAVASCRIPT (Header, Form, Modal) ========= -->
  <script>
    // Header Scroll Shadow
    const header = document.getElementById('mainHeader');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 20) {
        header.classList.add('header-scrolled');
      } else {
        header.classList.remove('header-scrolled');
      }
    });

    // Mobile Menu Toggle
    const menuToggle = document.getElementById('menuToggle');
    const mobileMenu = document.getElementById('mobileMenu');
    menuToggle.addEventListener('click', () => {
      mobileMenu.classList.toggle('open');
    });

    // Form Submission Logic to WhatsApp
    const connectionForm = document.getElementById('connectionForm');
    const thankYouModal = document.getElementById('thankYouModal');
    const closeModalBtn = document.getElementById('closeModalBtn');

    connectionForm.addEventListener('submit', function(e) {
      e.preventDefault();

      const name = document.getElementById('userName').value;
      const mobile = document.getElementById('userMobile').value;
      const email = document.getElementById('userEmail').value || 'দেওয়া হয়নি';
      const address = document.getElementById('userAddress').value;
      const connectionType = document.getElementById('connectionType').value;
      const selectedPackage = document.getElementById('packageSelect').value;

      const whatsappMessage = `*নতুন কানেকশন রিকোয়েস্ট*%0A%0A` +
        `*নাম:* ${encodeURIComponent(name)}%0A` +
        `*মোবাইল:* ${encodeURIComponent(mobile)}%0A` +
        `*ইমেইল:* ${encodeURIComponent(email)}%0A` +
        `*ঠিকানা:* ${encodeURIComponent(address)}%0A` +
        `*কানেকশন টাইপ:* ${encodeURIComponent(connectionType)}%0A` +
        `*প্যাকেজ:* ${encodeURIComponent(selectedPackage)}`;

      const targetWhatsAppNumber = "8801716729140";
      const whatsappApiUrl = `https://api.whatsapp.com/send?phone=${targetWhatsAppNumber}&text=${whatsappMessage}`;

      window.open(whatsappApiUrl, '_blank');
      connectionForm.reset();
      thankYouModal.classList.add('active');
    });

    closeModalBtn.addEventListener('click', () => {
      thankYouModal.classList.remove('active');
    });
  </script>

</body>
</html>
