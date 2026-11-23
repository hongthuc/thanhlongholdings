<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0">
    <title>CÔNG TY TNHH THÀNH LONG HOLDINGS | Hệ Thống Nha Khoa Chuẩn Quốc Tế Đà Nẵng</title>
    <meta name="description" content="Công Ty TNHH Thành Long Holdings - Hệ thống phòng khám nha khoa uy tín tại 14 Nguyễn Hữu Thọ, Phường Hòa Cường, TP Đà Nẵng. Chuyên Cấy ghép Implant, Niềng răng, Bọc răng sứ thẩm mỹ và Chăm sóc răng tổng quát.">

    <!-- Ảnh Thumbnail đại diện là Logo khi chia sẻ đường link website -->
    <link rel="icon" type="image/png" href="https://drive.google.com/thumbnail?id=1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25&sz=w256">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://thanhlongholdings.vn/">
    <meta property="og:title" content="CÔNG TY TNHH THÀNH LONG HOLDINGS - thanhlongholdings.vn">
    <meta property="og:description" content="Phòng khám nha khoa chuẩn quốc tế tại 14 Nguyễn Hữu Thọ, Phường Hòa Cường, TP Đà Nẵng. Hotline: 0325.274.667">
    <meta property="og:image" content="https://drive.google.com/thumbnail?id=1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25&sz=w1200">
    <meta property="og:image:width" content="1200">
    <meta property="og:image:height" content="630">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="CÔNG TY TNHH THÀNH LONG HOLDINGS - thanhlongholdings.vn">
    <meta name="twitter:description" content="Hệ thống nha khoa uy tín tại Đà Nẵng - Hotline: 0325.274.667">
    <meta name="twitter:image" content="https://drive.google.com/thumbnail?id=1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25&sz=w1200">

    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            primary: '#0B4F8C',    /* Xanh dương đậm y khoa đồng bộ nhận diện logo */
                            dark: '#073561',       /* Xanh navy đậm */
                            light: '#EBF4FC',      /* Xanh nhạt nền nhẹ */
                            accent: '#C89B3C',     /* Vàng đồng sang trọng */
                            accentHover: '#B0842A'
                        }
                    }
                }
            }
        }
    </script>

    <style>
        /* Chống tràn viền ngang và lệch trang trên mọi thiết bị */
        *, *::before, *::after {
            box-sizing: border-box;
        }
        html, body {
            margin: 0;
            padding: 0;
            width: 100%;
            max-width: 100%;
            overflow-x: hidden;
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
            background-color: #FFFFFF;
            color: #1E293B;
        }

        /* Chiều ngang chuẩn 95% trên máy tính, 100% có padding an toàn trên điện thoại */
        .tl-container {
            width: 100%;
            max-width: 100%;
            margin-left: auto;
            margin-right: auto;
            padding-left: 12px;
            padding-right: 12px;
        }
        @media (min-width: 1024px) {
            .tl-container {
                width: 95%;
                max-width: 95%;
                padding-left: 0;
                padding-right: 0;
            }
        }

        /* Banner Slider Grid chồng lớp đảm bảo 2 slide luôn có kích thước bằng nhau tuyệt đối */
        .banner-stage {
            display: grid;
            grid-template-columns: 1fr;
            position: relative;
            width: 100%;
            overflow: hidden;
        }
        .banner-slide {
            grid-area: 1 / 1;
            opacity: 0;
            visibility: hidden;
            pointer-events: none;
            transition: opacity 0.6s ease, transform 0.6s ease;
            transform: scale(1.01);
        }
        .banner-slide.active {
            opacity: 1;
            visibility: visible;
            pointer-events: auto;
            transform: scale(1);
            z-index: 10;
        }

        /* Nhãn giảm giá tròn kiểu Flatsome ở góc trên bên trái thẻ sản phẩm */
        .flatsome-sale-badge {
            position: absolute;
            top: 8px;
            left: 8px;
            width: 42px;
            height: 42px;
            border-radius: 9999px;
            background-color: #C89B3C;
            color: #FFFFFF;
            font-size: 12px;
            font-weight: 700;
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 15;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.16);
            line-height: 1;
        }
        @media (max-width: 639px) {
            .flatsome-sale-badge {
                width: 36px;
                height: 36px;
                font-size: 11px;
                top: 6px;
                left: 6px;
            }
        }

        /* Hiệu ứng nhịp nhẹ cho nút Hotline nổi */
        @keyframes softPulse {
            0% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0.45); }
            70% { box-shadow: 0 0 0 12px rgba(220, 38, 38, 0); }
            100% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0); }
        }
        .hotline-pulse {
            animation: softPulse 2s infinite;
        }

        /* Tránh thanh liên hệ cố định dưới điện thoại che footer */
        @media (max-width: 1023px) {
            body {
                padding-bottom: 62px;
            }
        }
    </style>
</head>
<body class="bg-white text-slate-800 antialiased">

    <!-- ==================== HEADER CHÍNH (KHÔNG CÓ NÚT GỌI NGAY, KHÔNG THANH CHỈNH SỬA UXBUILDER) ==================== -->
    <header id="site-header" class="sticky top-0 z-40 w-full bg-white/95 backdrop-blur-md border-b border-slate-200 shadow-sm">
        <div class="tl-container">
            <div class="flex items-center justify-between gap-3 py-2.5 lg:py-3">
                <!-- Logo chỉnh gọn nhỏ lại -->
                <a href="#trang-chu" class="flex items-center gap-2.5 shrink-0 focus:outline-none">
                    <img
                        src="https://drive.google.com/thumbnail?id=1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25&sz=w600"
                        data-fallback="https://lh3.googleusercontent.com/d/1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25=w600"
                        alt="Logo Công Ty TNHH Thành Long Holdings"
                        class="h-9 sm:h-10 lg:h-11 w-auto max-w-[130px] sm:max-w-[155px] object-contain rounded"
                        onerror="handleImageFallback(this, 'THÀNH LONG')"
                    >
                    <div class="hidden sm:flex flex-col leading-tight">
                        <span class="text-[12px] lg:text-[13px] font-extrabold text-brand-primary tracking-tight uppercase">Thành Long Holdings</span>
                        <span class="text-[10px] text-slate-500 font-medium">thanhlongholdings.vn</span>
                    </div>
                </a>

                <!-- Menu danh mục trên máy tính: chữ nhỏ gọn, viết liền không xuống dòng tên danh mục, tối đa 1-2 hàng cân đối -->
                <nav aria-label="Menu chính" class="hidden lg:flex flex-wrap items-center justify-end gap-x-4 xl:gap-x-5 gap-y-1 flex-1 min-w-0">
                    <a href="#trang-chu" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-brand-primary hover:text-brand-accent transition-colors py-1">Trang chủ</a>
                    <a href="#danh-muc" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Danh mục</a>
                    <a href="#san-pham" onclick="filterProducts('implant')" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Cấy ghép Implant</a>
                    <a href="#san-pham" onclick="filterProducts('nieng-rang')" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Niềng răng</a>
                    <a href="#san-pham" onclick="filterProducts('rang-su')" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Răng sứ thẩm mỹ</a>
                    <a href="#san-pham" onclick="filterProducts('tong-quat')" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Nha khoa tổng quát</a>
                    <a href="#truoc-sau" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Khách hàng</a>
                    <a href="#phong-kham" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Phòng khám</a>
                    <a href="#doi-tac" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Đối tác</a>
                    <a href="#bai-viet" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Tin tức</a>
                    <a href="#bao-gia" class="whitespace-nowrap text-[12.5px] xl:text-[13px] font-semibold text-slate-700 hover:text-brand-primary transition-colors py-1">Liên hệ</a>
                </nav>

                <!-- Nút mở menu trên điện thoại & máy tính bảng -->
                <button
                    id="mobile-menu-btn"
                    type="button"
                    aria-label="Mở menu danh mục"
                    class="lg:hidden inline-flex items-center justify-center w-10 h-10 rounded-lg border border-slate-200 text-brand-primary hover:bg-brand-light transition-colors shrink-0"
                >
                    <i class="fa-solid fa-bars text-lg"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- ==================== MENU NGĂN KÉO TRÊN ĐIỆN THOẠI ==================== -->
    <div id="mobile-drawer-overlay" class="fixed inset-0 bg-slate-900/50 z-50 hidden transition-opacity"></div>
    <aside id="mobile-drawer" class="fixed top-0 left-0 h-full w-72 max-w-[85vw] bg-white z-50 shadow-2xl transform -translate-x-full transition-transform duration-300 flex flex-col">
        <div class="flex items-center justify-between px-4 py-3.5 border-b border-slate-200 bg-brand-light/60">
            <div class="flex items-center gap-2">
                <img
                    src="https://drive.google.com/thumbnail?id=1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25&sz=w300"
                    data-fallback="https://lh3.googleusercontent.com/d/1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25=w300"
                    alt="Logo Thành Long Holdings"
                    class="h-8 w-auto object-contain rounded"
                    onerror="handleImageFallback(this, 'TL')"
                >
                <span class="text-xs font-bold text-brand-primary uppercase">Thành Long Holdings</span>
            </div>
            <button id="mobile-menu-close" type="button" aria-label="Đóng menu" class="w-9 h-9 rounded-lg flex items-center justify-center text-slate-600 hover:bg-white">
                <i class="fa-solid fa-xmark text-lg"></i>
            </button>
        </div>
        <div class="flex-1 overflow-y-auto p-4 space-y-1">
            <a href="#trang-chu" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-semibold text-brand-primary bg-brand-light">Trang chủ</a>
            <a href="#danh-muc" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Danh mục dịch vụ</a>
            <a href="#san-pham" onclick="filterProducts('implant')" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Cấy ghép Implant</a>
            <a href="#san-pham" onclick="filterProducts('nieng-rang')" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Niềng răng chỉnh nha</a>
            <a href="#san-pham" onclick="filterProducts('rang-su')" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Răng sứ thẩm mỹ</a>
            <a href="#san-pham" onclick="filterProducts('tong-quat')" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Chăm sóc răng tổng quát</a>
            <a href="#truoc-sau" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Trước &amp; Sau điều trị</a>
            <a href="#phong-kham" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Hình ảnh phòng khám</a>
            <a href="#doi-tac" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Đối tác chiến lược</a>
            <a href="#bai-viet" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Tin tức &amp; Kiến thức</a>
            <a href="#bao-gia" class="mobile-nav-link block px-3 py-2.5 rounded-lg text-sm font-medium text-slate-700 hover:bg-slate-100">Yêu cầu báo giá &amp; Bản đồ</a>
        </div>
        <div class="p-4 border-t border-slate-200 bg-slate-50 text-xs text-slate-600 space-y-1">
            <p class="font-semibold text-brand-primary">14 Nguyễn Hữu Thọ, P. Hòa Cường, TP Đà Nẵng</p>
            <p>Hotline: <a href="tel:0325274667" class="font-bold text-brand-accent">0325.274.667</a></p>
        </div>
    </aside>

    <main id="trang-chu" class="w-full overflow-x-hidden">

        <!-- ==================== 2 BANNER TỰ TRƯỢT CHUYÊN NGHIỆP (KÍCH THƯỚC BẰNG NHAU, CHỮ & ẢNH NẰM GỌN TRONG KHUNG, CÁCH XA VIỀN) ==================== -->
        <section aria-label="Banner giới thiệu dịch vụ" class="pt-3 sm:pt-5 pb-6 bg-slate-50/70">
            <div class="tl-container">
                <div id="hero-slider" class="relative rounded-2xl overflow-hidden shadow-lg border border-slate-200/80 bg-brand-dark">
                    <div class="banner-stage">

                        <!-- BANNER 1 -->
                        <div class="banner-slide active bg-gradient-to-br from-[#073561] via-[#0B4F8C] to-[#1167B1] text-white">
                            <!-- Khoảng đệm lớn (px-9 sm:px-14 lg:px-20 py-7 sm:py-10 lg:py-12) giúp chữ luôn cách xa viền ảnh và nút điều hướng -->
                            <div class="grid grid-cols-1 md:grid-cols-12 items-center gap-5 md:gap-8 px-9 sm:px-14 lg:px-20 py-7 sm:py-10 lg:py-12 h-full">
                                <div class="md:col-span-7 flex flex-col justify-center space-y-3 sm:space-y-4">
                                    <p class="text-[11px] sm:text-xs font-semibold uppercase tracking-widest text-amber-300">
                                        Công Ty TNHH Thành Long Holdings • Đà Nẵng
                                    </p>
                                    <h1 class="text-xl sm:text-3xl lg:text-4xl font-extrabold leading-snug text-white">
                                        Hệ Thống Nha Khoa Chuẩn Y Khoa Kiến Tạo Nụ Cười Bền Vững
                                    </h1>
                                    <p class="text-xs sm:text-sm lg:text-base text-blue-100 leading-relaxed max-w-xl">
                                        Chuyên sâu Cấy ghép Implant, Niềng răng chỉnh nha, Bọc răng sứ thẩm mỹ với đội ngũ bác sĩ giàu kinh nghiệm và hệ thống vô trùng khép kín tại 14 Nguyễn Hữu Thọ, Hòa Cường, TP Đà Nẵng.
                                    </p>
                                    <div class="pt-1 flex flex-wrap items-center gap-2.5 sm:gap-3">
                                        <a href="#bao-gia" class="inline-flex items-center gap-2 px-4 sm:px-6 py-2.5 sm:py-3 rounded-xl bg-brand-accent hover:bg-brand-accentHover text-white font-semibold text-xs sm:text-sm shadow transition-colors">
                                            <span>Đặt lịch tư vấn</span>
                                            <i class="fa-solid fa-arrow-right text-xs"></i>
                                        </a>
                                        <a href="#san-pham" class="inline-flex items-center gap-2 px-4 sm:px-6 py-2.5 sm:py-3 rounded-xl bg-white/15 hover:bg-white/25 text-white border border-white/30 font-semibold text-xs sm:text-sm transition-colors">
                                            <span>Xem bảng giá dịch vụ</span>
                                        </a>
                                    </div>
                                </div>
                                <div class="md:col-span-5 flex items-center justify-center">
                                    <div class="w-full aspect-[16/10] sm:aspect-[4/3] rounded-xl overflow-hidden border-2 border-white/25 shadow-xl bg-white/10">
                                        <img
                                            src="https://drive.google.com/thumbnail?id=1_e548h9zCJwGndxrtHlDtRoqA-n4NOjV&sz=w1200"
                                            data-fallback="https://lh3.googleusercontent.com/d/1_e548h9zCJwGndxrtHlDtRoqA-n4NOjV=w1200"
                                            alt="Không gian phòng khám nha khoa Thành Long Holdings"
                                            class="w-full h-full object-cover"
                                            onerror="handleImageFallback(this, 'Phòng Khám Thành Long')"
                                        >
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- BANNER 2 -->
                        <div class="banner-slide bg-gradient-to-br from-[#0A3D6E] via-[#0F5A9C] to-[#083B66] text-white">
                            <div class="grid grid-cols-1 md:grid-cols-12 items-center gap-5 md:gap-8 px-9 sm:px-14 lg:px-20 py-7 sm:py-10 lg:py-12 h-full">
                                <div class="md:col-span-7 flex flex-col justify-center space-y-3 sm:space-y-4">
                                    <p class="text-[11px] sm:text-xs font-semibold uppercase tracking-widest text-amber-300">
                                        Chương Trình Ưu Đãi Chăm Sóc Răng Miệng Toàn Diện
                                    </p>
                                    <h2 class="text-xl sm:text-3xl lg:text-4xl font-extrabold leading-snug text-white">
                                        Ưu Đãi Trồng Răng Implant &amp; Bọc Răng Sứ Lên Đến 55%
                                    </h2>
                                    <p class="text-xs sm:text-sm lg:text-base text-blue-100 leading-relaxed max-w-xl">
                                        Miễn phí thăm khám tổng quát, chụp phim kiểm tra tình trạng răng hàm và lên phác đồ điều trị trực tiếp cùng bác sĩ chuyên khoa. Hỗ trợ trả góp linh hoạt, bảo hành chính hãng dài hạn.
                                    </p>
                                    <div class="pt-1 flex flex-wrap items-center gap-2.5 sm:gap-3">
                                        <a href="#bao-gia" class="inline-flex items-center gap-2 px-4 sm:px-6 py-2.5 sm:py-3 rounded-xl bg-brand-accent hover:bg-brand-accentHover text-white font-semibold text-xs sm:text-sm shadow transition-colors">
                                            <span>Nhận báo giá ngay</span>
                                            <i class="fa-solid fa-arrow-right text-xs"></i>
                                        </a>
                                        <a href="#truoc-sau" class="inline-flex items-center gap-2 px-4 sm:px-6 py-2.5 sm:py-3 rounded-xl bg-white/15 hover:bg-white/25 text-white border border-white/30 font-semibold text-xs sm:text-sm transition-colors">
                                            <span>Kết quả điều trị</span>
                                        </a>
                                    </div>
                                </div>
                                <div class="md:col-span-5 flex items-center justify-center">
                                    <div class="w-full aspect-[16/10] sm:aspect-[4/3] rounded-xl overflow-hidden border-2 border-white/25 shadow-xl bg-white/10">
                                        <img
                                            src="https://drive.google.com/thumbnail?id=1xLwA2Ti8Ahg1AqoOuqq4c62i-KJF-Sj5&sz=w1200"
                                            data-fallback="https://lh3.googleusercontent.com/d/1xLwA2Ti8Ahg1AqoOuqq4c62i-KJF-Sj5=w1200"
                                            alt="Trang thiết bị hiện đại tại phòng khám Thành Long Holdings"
                                            class="w-full h-full object-cover"
                                            onerror="handleImageFallback(this, 'Thiết Bị Nha Khoa')"
                                        >
                                    </div>
                                </div>
                            </div>
                        </div>

                    </div>

                    <!-- Nút chuyển slide trái / phải đặt sát rìa ngoài, không đè chữ -->
                    <button
                        id="banner-prev"
                        type="button"
                        aria-label="Banner trước"
                        class="absolute left-1.5 sm:left-3 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-9 sm:h-9 rounded-full bg-white/20 hover:bg-white/35 text-white flex items-center justify-center backdrop-blur-sm transition-colors"
                    >
                        <i class="fa-solid fa-chevron-left text-xs sm:text-sm"></i>
                    </button>
                    <button
                        id="banner-next"
                        type="button"
                        aria-label="Banner tiếp theo"
                        class="absolute right-1.5 sm:right-3 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-9 sm:h-9 rounded-full bg-white/20 hover:bg-white/35 text-white flex items-center justify-center backdrop-blur-sm transition-colors"
                    >
                        <i class="fa-solid fa-chevron-right text-xs sm:text-sm"></i>
                    </button>

                    <!-- Chấm chỉ báo 2 banner -->
                    <div class="absolute bottom-2.5 sm:bottom-3.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
                        <button type="button" data-slide="0" aria-label="Chuyển tới banner 1" class="banner-dot w-6 h-2 rounded-full bg-amber-400 transition-all"></button>
                        <button type="button" data-slide="1" aria-label="Chuyển tới banner 2" class="banner-dot w-2 h-2 rounded-full bg-white/50 hover:bg-white transition-all"></button>
                    </div>
                </div>
            </div>
        </section>

        <!-- ==================== DANH MỤC DỊCH VỤ TRANG CHỦ (CHỮ NHỎ GỌN, TỐI ƯU ĐẸP TRÊN MÁY TÍNH & ĐIỆN THOẠI) ==================== -->
        <section id="danh-muc" class="py-7 sm:py-9 bg-white">
            <div class="tl-container">
                <div class="text-center mb-5 sm:mb-7">
                    <h2 class="text-lg sm:text-2xl font-extrabold text-brand-primary uppercase tracking-tight">Danh Mục Dịch Vụ Nha Khoa</h2>
                    <div class="w-14 h-1 bg-brand-accent mx-auto mt-2 rounded-full"></div>
                </div>

                <!-- Lưới danh mục cân đối: 2 cột trên điện thoại (item cuối căng giữa hoặc 5 cột đều trên máy tính) -->
                <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 gap-2.5 sm:gap-4">
                    <button type="button" onclick="selectCategoryAndScroll('implant')" class="group flex items-center lg:flex-col lg:justify-center gap-2.5 lg:gap-2 p-3 sm:p-4 rounded-xl bg-slate-50 hover:bg-brand-primary border border-slate-200 hover:border-brand-primary transition-all text-left lg:text-center shadow-sm">
                        <span class="w-9 h-9 sm:w-11 sm:h-11 rounded-lg bg-brand-light group-hover:bg-white/20 text-brand-primary group-hover:text-white flex items-center justify-center shrink-0 transition-colors">
                            <i class="fa-solid fa-tooth text-base sm:text-lg"></i>
                        </span>
                        <div class="min-w-0">
                            <div class="text-[12px] sm:text-[13px] font-bold text-slate-800 group-hover:text-white leading-snug">Cấy ghép Implant</div>
                            <div class="text-[11px] text-slate-500 group-hover:text-blue-100 mt-0.5 hidden sm:block">Phục hồi răng mất</div>
                        </div>
                    </button>

                    <button type="button" onclick="selectCategoryAndScroll('nieng-rang')" class="group flex items-center lg:flex-col lg:justify-center gap-2.5 lg:gap-2 p-3 sm:p-4 rounded-xl bg-slate-50 hover:bg-brand-primary border border-slate-200 hover:border-brand-primary transition-all text-left lg:text-center shadow-sm">
                        <span class="w-9 h-9 sm:w-11 sm:h-11 rounded-lg bg-brand-light group-hover:bg-white/20 text-brand-primary group-hover:text-white flex items-center justify-center shrink-0 transition-colors">
                            <i class="fa-regular fa-face-smile text-base sm:text-lg"></i>
                        </span>
                        <div class="min-w-0">
                            <div class="text-[12px] sm:text-[13px] font-bold text-slate-800 group-hover:text-white leading-snug">Niềng răng</div>
                            <div class="text-[11px] text-slate-500 group-hover:text-blue-100 mt-0.5 hidden sm:block">Chỉnh nha thẩm mỹ</div>
                        </div>
                    </button>

                    <button type="button" onclick="selectCategoryAndScroll('rang-su')" class="group flex items-center lg:flex-col lg:justify-center gap-2.5 lg:gap-2 p-3 sm:p-4 rounded-xl bg-slate-50 hover:bg-brand-primary border border-slate-200 hover:border-brand-primary transition-all text-left lg:text-center shadow-sm">
                        <span class="w-9 h-9 sm:w-11 sm:h-11 rounded-lg bg-brand-light group-hover:bg-white/20 text-brand-primary group-hover:text-white flex items-center justify-center shrink-0 transition-colors">
                            <i class="fa-solid fa-gem text-base sm:text-lg"></i>
                        </span>
                        <div class="min-w-0">
                            <div class="text-[12px] sm:text-[13px] font-bold text-slate-800 group-hover:text-white leading-snug">Răng sứ thẩm mỹ</div>
                            <div class="text-[11px] text-slate-500 group-hover:text-blue-100 mt-0.5 hidden sm:block">Bọc sứ &amp; Veneer</div>
                        </div>
                    </button>

                    <button type="button" onclick="selectCategoryAndScroll('tong-quat')" class="group flex items-center lg:flex-col lg:justify-center gap-2.5 lg:gap-2 p-3 sm:p-4 rounded-xl bg-slate-50 hover:bg-brand-primary border border-slate-200 hover:border-brand-primary transition-all text-left lg:text-center shadow-sm">
                        <span class="w-9 h-9 sm:w-11 sm:h-11 rounded-lg bg-brand-light group-hover:bg-white/20 text-brand-primary group-hover:text-white flex items-center justify-center shrink-0 transition-colors">
                            <i class="fa-solid fa-shield-heart text-base sm:text-lg"></i>
                        </span>
                        <div class="min-w-0">
                            <div class="text-[12px] sm:text-[13px] font-bold text-slate-800 group-hover:text-white leading-snug">Nha khoa tổng quát</div>
                            <div class="text-[11px] text-slate-500 group-hover:text-blue-100 mt-0.5 hidden sm:block">Cạo vôi &amp; Tẩy trắng</div>
                        </div>
                    </button>

                    <button type="button" onclick="selectCategoryAndScroll('tre-em')" class="col-span-2 sm:col-span-1 group flex items-center justify-center lg:flex-col gap-2.5 lg:gap-2 p-3 sm:p-4 rounded-xl bg-slate-50 hover:bg-brand-primary border border-slate-200 hover:border-brand-primary transition-all text-left lg:text-center shadow-sm">
                        <span class="w-9 h-9 sm:w-11 sm:h-11 rounded-lg bg-brand-light group-hover:bg-white/20 text-brand-primary group-hover:text-white flex items-center justify-center shrink-0 transition-colors">
                            <i class="fa-solid fa-child-reaching text-base sm:text-lg"></i>
                        </span>
                        <div class="min-w-0">
                            <div class="text-[12px] sm:text-[13px] font-bold text-slate-800 group-hover:text-white leading-snug">Nha khoa trẻ em</div>
                            <div class="text-[11px] text-slate-500 group-hover:text-blue-100 mt-0.5 hidden sm:block">Tiền chỉnh nha &amp; Nhổ răng</div>
                        </div>
                    </button>
                </div>
            </div>
        </section>

        <!-- ==================== DANH MỤC SẢN PHẨM & DỊCH VỤ TRANG CHỦ (CHUẨN FLATSOME: 2 CỘT MOBILE, % GIẢM GIÁ GÓC TRÊN TRÁI) ==================== -->
        <section id="san-pham" class="py-9 sm:py-12 bg-slate-50 border-y border-slate-200/70">
            <div class="tl-container">
                <div class="text-center mb-6">
                    <h2 class="text-lg sm:text-2xl font-extrabold text-brand-primary uppercase tracking-tight">Các Dịch Vụ &amp; Sản Phẩm Nổi Bật</h2>
                    <div class="w-14 h-1 bg-brand-accent mx-auto mt-2 rounded-full"></div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-2.5 max-w-2xl mx-auto">
                        Bảng giá niêm yết minh bạch, ưu đãi trực tiếp theo từng hạng mục dịch vụ tại Công Ty TNHH Thành Long Holdings.
                    </p>
                </div>

                <!-- Bộ lọc danh mục gọn gàng theo chuẩn Flatsome UX Tabs -->
                <div id="category-tabs" class="flex flex-wrap items-center justify-center gap-2 mb-6 sm:mb-8">
                    <button type="button" data-cat="all" class="cat-tab active px-3.5 py-2 rounded-full text-xs sm:text-[13px] font-semibold bg-brand-primary text-white border border-brand-primary transition-colors">Tất cả dịch vụ</button>
                    <button type="button" data-cat="tong-quat" class="cat-tab px-3.5 py-2 rounded-full text-xs sm:text-[13px] font-semibold bg-white text-slate-700 hover:text-brand-primary border border-slate-200 transition-colors">Chăm sóc răng tổng quát</button>
                    <button type="button" data-cat="rang-su" class="cat-tab px-3.5 py-2 rounded-full text-xs sm:text-[13px] font-semibold bg-white text-slate-700 hover:text-brand-primary border border-slate-200 transition-colors">Răng sứ thẩm mỹ</button>
                    <button type="button" data-cat="nieng-rang" class="cat-tab px-3.5 py-2 rounded-full text-xs sm:text-[13px] font-semibold bg-white text-slate-700 hover:text-brand-primary border border-slate-200 transition-colors">Niềng răng</button>
                    <button type="button" data-cat="implant" class="cat-tab px-3.5 py-2 rounded-full text-xs sm:text-[13px] font-semibold bg-white text-slate-700 hover:text-brand-primary border border-slate-200 transition-colors">Cấy ghép Implant</button>
                    <button type="button" data-cat="tre-em" class="cat-tab px-3.5 py-2 rounded-full text-xs sm:text-[13px] font-semibold bg-white text-slate-700 hover:text-brand-primary border border-slate-200 transition-colors">Nha khoa trẻ em</button>
                </div>

                <!-- Lưới sản phẩm: 2 cột trên điện thoại, 3 cột tablet, 4 cột desktop -->
                <div id="product-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-5">
                    <!-- Sản phẩm được render tự động từ dữ liệu chuẩn để dễ quản lý & lọc -->
                </div>
            </div>
        </section>

        <!-- ==================== HIỆU QUẢ TRƯỚC VÀ SAU KHI ĐIỀU TRỊ NHA KHOA ==================== -->
        <section id="truoc-sau" class="py-10 sm:py-14 bg-white">
            <div class="tl-container">
                <div class="text-center mb-7 sm:mb-9">
                    <h2 class="text-lg sm:text-2xl font-extrabold text-brand-primary uppercase tracking-tight">Hiệu Quả Trước Và Sau Khi Điều Trị</h2>
                    <div class="w-14 h-1 bg-brand-accent mx-auto mt-2 rounded-full"></div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-2.5 max-w-2xl mx-auto">
                        Hình ảnh thực tế khách hàng thay đổi nụ cười sau liệu trình chỉnh nha, phục hình sứ thẩm mỹ và cấy ghép Implant.
                    </p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 gap-5 sm:gap-7">
                    <!-- Case 1 -->
                    <article class="bg-slate-50 rounded-2xl overflow-hidden border border-slate-200 shadow-sm flex flex-col">
                        <div class="relative aspect-[16/10] bg-slate-100 overflow-hidden cursor-pointer" onclick="openLightbox('https://drive.google.com/thumbnail?id=1wn1LLAyx6ZTEMmkWtuyr57Pa9Mt9na6s&sz=w1400', 'Kết quả trước và sau điều trị nha khoa - Trường hợp 1')">
                            <img
                                src="https://drive.google.com/thumbnail?id=1wn1LLAyx6ZTEMmkWtuyr57Pa9Mt9na6s&sz=w1200"
                                data-fallback="https://lh3.googleusercontent.com/d/1wn1LLAyx6ZTEMmkWtuyr57Pa9Mt9na6s=w1200"
                                alt="Kết quả trước và sau khi điều trị nha khoa trường hợp 1"
                                class="w-full h-full object-cover hover:scale-105 transition-transform duration-500"
                                onerror="handleImageFallback(this, 'Trước & Sau Điều Trị 1')"
                            >
                        </div>
                        <div class="p-4 sm:p-6 flex-1 flex flex-col justify-between">
                            <div>
                                <h3 class="text-base sm:text-lg font-bold text-brand-primary">Phục Hình &amp; Chỉnh Nha Thẩm Mỹ Toàn Diện</h3>
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 mt-3 text-xs sm:text-sm">
                                    <div class="bg-white p-3 rounded-xl border border-slate-200/80">
                                        <p class="font-bold text-slate-800 mb-1">Trước điều trị:</p>
                                        <ul class="text-slate-600 space-y-1 list-disc list-inside">
                                            <li>Răng chen chúc, không đều</li>
                                            <li>Sai lệch khớp cắn nhẹ</li>
                                            <li>Màu sắc men răng kém hài hòa</li>
                                        </ul>
                                    </div>
                                    <div class="bg-brand-light/60 p-3 rounded-xl border border-brand-primary/15">
                                        <p class="font-bold text-brand-primary mb-1">Sau điều trị:</p>
                                        <ul class="text-slate-700 space-y-1 list-disc list-inside">
                                            <li>Sắp đều cung hàm, khớp cắn chuẩn</li>
                                            <li>Form răng hài hòa khuôn mặt</li>
                                            <li>Ăn nhai chắc khỏe, nụ cười tự tin</li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </article>

                    <!-- Case 2 -->
                    <article class="bg-slate-50 rounded-2xl overflow-hidden border border-slate-200 shadow-sm flex flex-col">
                        <div class="relative aspect-[16/10] bg-slate-100 overflow-hidden cursor-pointer" onclick="openLightbox('https://drive.google.com/thumbnail?id=1uljfP3PwL_kkLmukmveUaBJlshC0ffqk&sz=w1400', 'Kết quả trước và sau điều trị nha khoa - Trường hợp 2')">
                            <img
                                src="https://drive.google.com/thumbnail?id=1uljfP3PwL_kkLmukmveUaBJlshC0ffqk&sz=w1200"
                                data-fallback="https://lh3.googleusercontent.com/d/1uljfP3PwL_kkLmukmveUaBJlshC0ffqk=w1200"
                                alt="Kết quả trước và sau khi điều trị nha khoa trường hợp 2"
                                class="w-full h-full object-cover hover:scale-105 transition-transform duration-500"
                                onerror="handleImageFallback(this, 'Trước & Sau Điều Trị 2')"
                            >
                        </div>
                        <div class="p-4 sm:p-6 flex-1 flex flex-col justify-between">
                            <div>
                                <h3 class="text-base sm:text-lg font-bold text-brand-primary">Cải Thiện Cung Hàm &amp; Nụ Cười Rạng Rỡ</h3>
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 mt-3 text-xs sm:text-sm">
                                    <div class="bg-white p-3 rounded-xl border border-slate-200/80">
                                        <p class="font-bold text-slate-800 mb-1">Trước điều trị:</p>
                                        <ul class="text-slate-600 space-y-1 list-disc list-inside">
                                            <li>Răng thưa, hình thể răng thiếu cân đối</li>
                                            <li>Tình trạng khớp cắn chưa ổn định</li>
                                            <li>Khách hàng ngại cười khi giao tiếp</li>
                                        </ul>
                                    </div>
                                    <div class="bg-brand-light/60 p-3 rounded-xl border border-brand-primary/15">
                                        <p class="font-bold text-brand-primary mb-1">Sau điều trị:</p>
                                        <ul class="text-slate-700 space-y-1 list-disc list-inside">
                                            <li>Khắc phục triệt để khuyết điểm răng</li>
                                            <li>Nụ cười đều đẹp tự nhiên</li>
                                            <li>Đảm bảo chức năng ăn nhai bền lâu</li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </article>
                </div>
            </div>
        </section>

        <!-- ==================== HÌNH ẢNH THỰC TẾ PHÒNG KHÁM (ĐẦY ĐỦ 8 ẢNH THỰC TẾ) ==================== -->
        <section id="phong-kham" class="py-10 sm:py-14 bg-slate-50 border-y border-slate-200/70">
            <div class="tl-container">
                <div class="text-center mb-7 sm:mb-9">
                    <h2 class="text-lg sm:text-2xl font-extrabold text-brand-primary uppercase tracking-tight">Hình Ảnh Thực Tế Phòng Khám</h2>
                    <div class="w-14 h-1 bg-brand-accent mx-auto mt-2 rounded-full"></div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-2.5 max-w-2xl mx-auto">
                        Cơ sở vật chất khang trang, hệ thống trang thiết bị nha khoa hiện đại cùng quy trình vô trùng chuẩn Bộ Y Tế tại 14 Nguyễn Hữu Thọ, TP Đà Nẵng.
                    </p>
                </div>

                <!-- 2 cột trên điện thoại, 4 cột trên máy tính -->
                <div class="grid grid-cols-2 lg:grid-cols-4 gap-3 sm:gap-4" id="clinic-gallery">
                    <!-- Render 8 ảnh thực tế phòng khám -->
                </div>
            </div>
        </section>

        <!-- ==================== DANH MỤC CÁC ĐỐI TÁC CHIẾN LƯỢC ==================== -->
        <section id="doi-tac" class="py-10 sm:py-12 bg-white">
            <div class="tl-container">
                <div class="text-center mb-7">
                    <h2 class="text-lg sm:text-2xl font-extrabold text-brand-primary uppercase tracking-tight">Đối Tác Chiến Lược &amp; Thương Hiệu Vật Liệu</h2>
                    <div class="w-14 h-1 bg-brand-accent mx-auto mt-2 rounded-full"></div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-2.5 max-w-2xl mx-auto">
                        Đồng hành cùng các thương hiệu Implant, chỉnh nha, răng sứ hàng đầu thế giới và đối tác bảo lãnh viện phí uy tín.
                    </p>
                </div>

                <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 sm:gap-4">
                    <!-- Đối tác 1 -->
                    <div class="p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-200 hover:border-brand-primary/40 hover:shadow-md transition-all flex flex-col items-center justify-center text-center">
                        <span class="text-base sm:text-lg font-extrabold tracking-tight text-brand-primary">STRAUMANN</span>
                        <span class="text-[11px] text-slate-500 mt-1">Implant Thụy Sĩ</span>
                    </div>
                    <!-- Đối tác 2 -->
                    <div class="p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-200 hover:border-brand-primary/40 hover:shadow-md transition-all flex flex-col items-center justify-center text-center">
                        <span class="text-base sm:text-lg font-extrabold tracking-tight text-brand-dark">OSSTEM</span>
                        <span class="text-[11px] text-slate-500 mt-1">Implant Hàn Quốc</span>
                    </div>
                    <!-- Đối tác 3 -->
                    <div class="p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-200 hover:border-brand-primary/40 hover:shadow-md transition-all flex flex-col items-center justify-center text-center">
                        <span class="text-base sm:text-lg font-extrabold tracking-tight text-brand-primary">DENTIUM</span>
                        <span class="text-[11px] text-slate-500 mt-1">Hệ thống Implant</span>
                    </div>
                    <!-- Đối tác 4 -->
                    <div class="p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-200 hover:border-brand-primary/40 hover:shadow-md transition-all flex flex-col items-center justify-center text-center">
                        <span class="text-base sm:text-lg font-extrabold tracking-tight text-sky-700">invisalign</span>
                        <span class="text-[11px] text-slate-500 mt-1">Niềng răng Hoa Kỳ</span>
                    </div>
                    <!-- Đối tác 5 -->
                    <div class="p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-200 hover:border-brand-primary/40 hover:shadow-md transition-all flex flex-col items-center justify-center text-center">
                        <span class="text-base sm:text-lg font-extrabold tracking-tight text-slate-800">CERCON HT</span>
                        <span class="text-[11px] text-slate-500 mt-1">Răng sứ Đức</span>
                    </div>
                    <!-- Đối tác 6 -->
                    <div class="p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-200 hover:border-brand-primary/40 hover:shadow-md transition-all flex flex-col items-center justify-center text-center">
                        <span class="text-base sm:text-lg font-extrabold tracking-tight text-red-700">3M ESPE</span>
                        <span class="text-[11px] text-slate-500 mt-1">Sứ Lava Plus Hoa Kỳ</span>
                    </div>
                    <!-- Đối tác 7 -->
                    <div class="p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-200 hover:border-brand-primary/40 hover:shadow-md transition-all flex flex-col items-center justify-center text-center">
                        <span class="text-base sm:text-lg font-extrabold tracking-tight text-brand-primary">BẢO HIỂM PVI</span>
                        <span class="text-[11px] text-slate-500 mt-1">Bảo lãnh viện phí</span>
                    </div>
                    <!-- Đối tác 8 -->
                    <div class="p-4 sm:p-5 rounded-xl bg-slate-50 border border-slate-200 hover:border-brand-primary/40 hover:shadow-md transition-all flex flex-col items-center justify-center text-center">
                        <span class="text-base sm:text-lg font-extrabold tracking-tight text-amber-700">BẢO VIỆT</span>
                        <span class="text-[11px] text-slate-500 mt-1">Đối tác bảo hiểm y tế</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- ==================== DANH MỤC CÁC BÀI VIẾT TRANG CHỦ ==================== -->
        <section id="bai-viet" class="py-10 sm:py-14 bg-slate-50 border-y border-slate-200/70">
            <div class="tl-container">
                <div class="text-center mb-7 sm:mb-9">
                    <h2 class="text-lg sm:text-2xl font-extrabold text-brand-primary uppercase tracking-tight">Tin Tức &amp; Kiến Thức Nha Khoa</h2>
                    <div class="w-14 h-1 bg-brand-accent mx-auto mt-2 rounded-full"></div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-2.5 max-w-2xl mx-auto">
                        Cập nhật kiến thức chăm sóc răng miệng, quy trình điều trị chuẩn y khoa và thông tin ưu đãi mới nhất.
                    </p>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 sm:gap-5" id="articles-grid">
                    <!-- Render 4 bài viết chuyên môn -->
                </div>
            </div>
        </section>

        <!-- ==================== FORM YÊU CẦU & BÁO GIÁ + GOOGLE MAP + FANPAGE RA NGOÀI TRANG CHỦ ==================== -->
        <section id="bao-gia" class="py-10 sm:py-14 bg-white">
            <div class="tl-container">
                <div class="text-center mb-7 sm:mb-9">
                    <h2 class="text-lg sm:text-2xl font-extrabold text-brand-primary uppercase tracking-tight">Đăng Ký Tư Vấn &amp; Nhận Báo Giá</h2>
                    <div class="w-14 h-1 bg-brand-accent mx-auto mt-2 rounded-full"></div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-2.5 max-w-2xl mx-auto">
                        Để lại thông tin bên dưới, chuyên viên Công Ty TNHH Thành Long Holdings sẽ liên hệ tư vấn và gửi báo giá chi tiết trong vòng 5 phút.
                    </p>
                </div>

                <!-- Hàng 1: Form Yêu Cầu & Báo Giá + Thông tin & Fanpage -->
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-stretch">
                    <!-- Cột Trái (7/12): Form Yêu Cầu và Báo Giá -->
                    <div class="lg:col-span-7 bg-slate-50 rounded-2xl p-5 sm:p-7 border border-slate-200 shadow-sm flex flex-col justify-between">
                        <div>
                            <h3 class="text-base sm:text-lg font-bold text-brand-primary mb-1">Biểu Mẫu Yêu Cầu Báo Giá &amp; Đặt Lịch Hẹn</h3>
                            <p class="text-xs sm:text-sm text-slate-600 mb-5">Miễn phí thăm khám trực tiếp và tư vấn phác đồ điều trị phù hợp.</p>

                            <form id="quote-form" class="space-y-4">
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                    <div>
                                        <label for="q-name" class="block text-xs sm:text-sm font-semibold text-slate-700 mb-1.5">Họ và tên <span class="text-red-500">*</span></label>
                                        <input id="q-name" type="text" required placeholder="Nhập họ và tên của bạn" class="w-full px-3.5 py-2.5 rounded-xl border border-slate-300 bg-white text-sm focus:outline-none focus:ring-2 focus:ring-brand-primary/30 focus:border-brand-primary">
                                    </div>
                                    <div>
                                        <label for="q-phone" class="block text-xs sm:text-sm font-semibold text-slate-700 mb-1.5">Số điện thoại <span class="text-red-500">*</span></label>
                                        <input id="q-phone" type="tel" required placeholder="Ví dụ: 0325 274 667" class="w-full px-3.5 py-2.5 rounded-xl border border-slate-300 bg-white text-sm focus:outline-none focus:ring-2 focus:ring-brand-primary/30 focus:border-brand-primary">
                                    </div>
                                </div>

                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                    <div>
                                        <label for="q-service" class="block text-xs sm:text-sm font-semibold text-slate-700 mb-1.5">Dịch vụ quan tâm</label>
                                        <select id="q-service" class="w-full px-3.5 py-2.5 rounded-xl border border-slate-300 bg-white text-sm focus:outline-none focus:ring-2 focus:ring-brand-primary/30 focus:border-brand-primary">
                                            <option value="Cạo Vôi Răng & Đánh Bóng">Cạo Vôi Răng &amp; Đánh Bóng</option>
                                            <option value="Bọc Răng Sứ Thẩm Mỹ">Bọc Răng Sứ Thẩm Mỹ</option>
                                            <option value="Niềng Răng Chỉnh Nha">Niềng Răng Chỉnh Nha</option>
                                            <option value="Trồng Răng Implant">Trồng Răng Implant</option>
                                            <option value="Nha Khoa Trẻ Em">Nha Khoa Trẻ Em</option>
                                            <option value="Tư Vấn Trả Góp & Bảng Giá">Tư Vấn Trả Góp &amp; Bảng Giá</option>
                                        </select>
                                    </div>
                                    <div>
                                        <label for="q-date" class="block text-xs sm:text-sm font-semibold text-slate-700 mb-1.5">Ngày dự kiến thăm khám</label>
                                        <input id="q-date" type="date" class="w-full px-3.5 py-2.5 rounded-xl border border-slate-300 bg-white text-sm focus:outline-none focus:ring-2 focus:ring-brand-primary/30 focus:border-brand-primary">
                                    </div>
                                </div>

                                <div>
                                    <label for="q-note" class="block text-xs sm:text-sm font-semibold text-slate-700 mb-1.5">Yêu cầu chi tiết / Tình trạng răng miệng</label>
                                    <textarea id="q-note" rows="3" placeholder="Mô tả ngắn gọn tình trạng hoặc dịch vụ bạn cần nhận báo giá..." class="w-full px-3.5 py-2.5 rounded-xl border border-slate-300 bg-white text-sm focus:outline-none focus:ring-2 focus:ring-brand-primary/30 focus:border-brand-primary resize-none"></textarea>
                                </div>

                                <div id="quote-feedback" class="hidden p-3.5 rounded-xl text-xs sm:text-sm font-medium"></div>

                                <button type="submit" class="w-full sm:w-auto px-7 py-3 rounded-xl bg-brand-primary hover:bg-brand-dark text-white font-bold text-sm shadow transition-colors inline-flex items-center justify-center gap-2">
                                    <i class="fa-solid fa-paper-plane text-xs"></i>
                                    <span>Gửi yêu cầu báo giá ngay</span>
                                </button>
                            </form>
                        </div>
                    </div>

                    <!-- Cột Phải (5/12): Fanpage Facebook chính thức hiển thị ngay ngoài trang chủ -->
                    <div class="lg:col-span-5 bg-slate-50 rounded-2xl p-5 sm:p-6 border border-slate-200 shadow-sm flex flex-col justify-between">
                        <div>
                            <div class="flex items-center justify-between gap-2 mb-4">
                                <h3 class="text-base sm:text-lg font-bold text-brand-primary flex items-center gap-2">
                                    <i class="fa-brands fa-facebook text-[#1877F2] text-xl"></i>
                                    <span>Fanpage Chính Thức</span>
                                </h3>
                                <a href="https://www.facebook.com/" target="_blank" rel="noopener noreferrer" class="text-xs font-semibold text-[#1877F2] hover:underline">Mở Facebook</a>
                            </div>

                            <!-- Khung hiển thị Fanpage trực quan ngoài trang chủ -->
                            <div class="rounded-xl overflow-hidden border border-slate-200 bg-white shadow-sm">
                                <!-- Ảnh bìa Fanpage -->
                                <div class="relative h-36 sm:h-40 bg-brand-dark overflow-hidden">
                                    <img
                                        src="https://drive.google.com/thumbnail?id=1_hbY6U7-qZEkTrRwf3XAsZ1Ob7ES57EM&sz=w1000"
                                        data-fallback="https://lh3.googleusercontent.com/d/1_hbY6U7-qZEkTrRwf3XAsZ1Ob7ES57EM=w1000"
                                        alt="Ảnh bìa Fanpage Thành Long Holdings"
                                        class="w-full h-full object-cover opacity-90"
                                        onerror="handleImageFallback(this, 'Fanpage Thành Long')"
                                    >
                                    <div class="absolute inset-0 bg-gradient-to-t from-slate-900/80 via-slate-900/20 to-transparent"></div>
                                    <div class="absolute bottom-3 left-3 right-3 flex items-center gap-3">
                                        <div class="w-12 h-12 rounded-xl bg-white p-1 shadow shrink-0 flex items-center justify-center">
                                            <img
                                                src="https://drive.google.com/thumbnail?id=1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25&sz=w256"
                                                data-fallback="https://lh3.googleusercontent.com/d/1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25=w256"
                                                alt="Avatar Fanpage Thành Long Holdings"
                                                class="w-full h-full object-contain rounded-lg"
                                                onerror="handleImageFallback(this, 'TL')"
                                            >
                                        </div>
                                        <div class="min-w-0 text-white">
                                            <p class="text-sm font-bold leading-tight truncate">Thành Long Holdings - Nha Khoa Đà Nẵng</p>
                                            <p class="text-[11px] text-slate-200 mt-0.5">Phòng khám nha khoa • 14 Nguyễn Hữu Thọ</p>
                                        </div>
                                    </div>
                                </div>

                                <!-- Nội dung & nút tương tác Fanpage -->
                                <div class="p-4 space-y-3">
                                    <p class="text-xs text-slate-600 leading-relaxed">
                                        Theo dõi Fanpage để cập nhật hình ảnh thực tế khách hàng, lịch làm việc và các chương trình ưu đãi chăm sóc răng miệng hàng tháng tại Đà Nẵng.
                                    </p>
                                    <div class="flex flex-wrap items-center gap-2">
                                        <a href="https://www.facebook.com/" target="_blank" rel="noopener noreferrer" class="flex-1 inline-flex items-center justify-center gap-1.5 px-3 py-2 rounded-lg bg-[#1877F2] hover:bg-[#1465D1] text-white text-xs font-semibold transition-colors">
                                            <i class="fa-solid fa-thumbs-up"></i>
                                            <span>Thích Trang</span>
                                        </a>
                                        <a href="https://m.me/" target="_blank" rel="noopener noreferrer" class="flex-1 inline-flex items-center justify-center gap-1.5 px-3 py-2 rounded-lg bg-slate-100 hover:bg-slate-200 text-slate-800 text-xs font-semibold transition-colors">
                                            <i class="fa-brands fa-facebook-messenger text-[#0084FF]"></i>
                                            <span>Nhắn tin tư vấn</span>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- Thông tin liên hệ nhanh bổ sung -->
                        <div class="mt-4 pt-4 border-t border-slate-200 text-xs sm:text-sm space-y-1.5 text-slate-700">
                            <p class="flex items-start gap-2">
                                <i class="fa-solid fa-location-dot text-brand-accent mt-1 shrink-0"></i>
                                <span><strong>Địa chỉ:</strong> 14 Nguyễn Hữu Thọ, Phường Hòa Cường, TP Đà Nẵng</span>
                            </p>
                            <p class="flex items-center gap-2">
                                <i class="fa-solid fa-phone text-brand-primary shrink-0"></i>
                                <span><strong>Hotline:</strong> <a href="tel:0325274667" class="font-bold text-brand-primary hover:underline">0325.274.667</a></span>
                            </p>
                            <p class="flex items-center gap-2">
                                <i class="fa-solid fa-clock text-brand-primary shrink-0"></i>
                                <span><strong>Giờ làm việc:</strong> 08:00 – 18:30 (Tất cả các ngày trong tuần)</span>
                            </p>
                        </div>
                    </div>
                </div>

                <!-- Hàng 2: Bản đồ Google Maps hiển thị trực tiếp ra ngoài trang chủ -->
                <div class="mt-6 sm:mt-8 bg-slate-50 rounded-2xl p-4 sm:p-5 border border-slate-200 shadow-sm">
                    <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2 mb-3.5">
                        <div>
                            <h3 class="text-base sm:text-lg font-bold text-brand-primary flex items-center gap-2">
                                <i class="fa-solid fa-map-location-dot text-brand-accent"></i>
                                <span>Bản Đồ Chỉ Đường Google Maps</span>
                            </h3>
                            <p class="text-xs sm:text-sm text-slate-600 mt-0.5">14 Nguyễn Hữu Thọ, Phường Hòa Cường, TP Đà Nẵng</p>
                        </div>
                        <a
                            href="https://www.google.com/maps/search/?api=1&query=14+Nguy%E1%BB%85n+H%E1%BB%AFu+Th%E1%BB%8D,+Ph%C6%B0%E1%BB%9Dng+H%C3%B2a+C%C6%B0%E1%BB%9Dng,+TP+%C4%90%C3%A0+N%E1%BA%B5ng"
                            target="_blank"
                            rel="noopener noreferrer"
                            class="inline-flex items-center justify-center gap-2 px-4 py-2 rounded-xl bg-brand-primary hover:bg-brand-dark text-white text-xs sm:text-sm font-semibold transition-colors shrink-0"
                        >
                            <i class="fa-solid fa-diamond-turn-right"></i>
                            <span>Mở chỉ đường Google Maps</span>
                        </a>
                    </div>
                    <div class="w-full h-[280px] sm:h-[360px] rounded-xl overflow-hidden border border-slate-200 bg-white">
                        <iframe
                            title="Bản đồ Công Ty TNHH Thành Long Holdings - 14 Nguyễn Hữu Thọ, Hòa Cường, Đà Nẵng"
                            src="https://maps.google.com/maps?q=14%20Nguy%E1%BB%85n%20H%E1%BB%AFu%20Th%E1%BB%8D,%20H%C3%B2a%20C%C6%B0%E1%BB%9Dng,%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=16&ie=UTF8&iwloc=&output=embed"
                            class="w-full h-full border-0"
                            loading="lazy"
                            referrerpolicy="no-referrer-when-downgrade"
                        ></iframe>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- ==================== FOOTER CHUẨN FLATSOME ==================== -->
    <footer class="bg-brand-dark text-blue-100 pt-10 pb-8 border-t-4 border-brand-accent">
        <div class="tl-container">
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-7 pb-8 border-b border-white/15">
                <!-- Cột 1: Thông tin doanh nghiệp -->
                <div class="space-y-3">
                    <div class="inline-flex items-center gap-2.5 bg-white px-3 py-2 rounded-xl">
                        <img
                            src="https://drive.google.com/thumbnail?id=1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25&sz=w400"
                            data-fallback="https://lh3.googleusercontent.com/d/1bJulmsPvS9gcyv7rU_fGI4GvNFyJzH25=w400"
                            alt="Logo Công Ty TNHH Thành Long Holdings"
                            class="h-8 w-auto object-contain"
                            onerror="handleImageFallback(this, 'THÀNH LONG')"
                        >
                    </div>
                    <h3 class="text-sm font-extrabold text-white uppercase tracking-wide">CÔNG TY TNHH THÀNH LONG HOLDINGS</h3>
                    <p class="text-xs leading-relaxed text-blue-100/90">
                        Hệ thống chăm sóc sức khỏe răng miệng toàn diện tại Đà Nẵng, chuyên sâu Cấy ghép Implant, Niềng răng thẩm mỹ và Bọc răng sứ chuẩn y khoa.
                    </p>
                    <p class="text-xs text-amber-300 font-semibold">Website: thanhlongholdings.vn</p>
                </div>

                <!-- Cột 2: Danh mục dịch vụ -->
                <div>
                    <h4 class="text-sm font-bold text-white uppercase tracking-wide mb-3">Danh Mục Dịch Vụ</h4>
                    <ul class="space-y-2 text-xs">
                        <li><a href="#san-pham" onclick="filterProducts('implant')" class="hover:text-amber-300 transition-colors">Cấy ghép Implant chính hãng</a></li>
                        <li><a href="#san-pham" onclick="filterProducts('nieng-rang')" class="hover:text-amber-300 transition-colors">Niềng răng mắc cài &amp; Trong suốt</a></li>
                        <li><a href="#san-pham" onclick="filterProducts('rang-su')" class="hover:text-amber-300 transition-colors">Bọc răng sứ thẩm mỹ &amp; Veneer</a></li>
                        <li><a href="#san-pham" onclick="filterProducts('tong-quat')" class="hover:text-amber-300 transition-colors">Cạo vôi răng &amp; Chăm sóc tổng quát</a></li>
                        <li><a href="#san-pham" onclick="filterProducts('tre-em')" class="hover:text-amber-300 transition-colors">Nha khoa trẻ em &amp; Tiền chỉnh nha</a></li>
                    </ul>
                </div>

                <!-- Cột 3: Hỗ trợ khách hàng -->
                <div>
                    <h4 class="text-sm font-bold text-white uppercase tracking-wide mb-3">Thông Tin Hữu Ích</h4>
                    <ul class="space-y-2 text-xs">
                        <li><a href="#truoc-sau" class="hover:text-amber-300 transition-colors">Kết quả trước &amp; sau điều trị</a></li>
                        <li><a href="#phong-kham" class="hover:text-amber-300 transition-colors">Hình ảnh thực tế phòng khám</a></li>
                        <li><a href="#doi-tac" class="hover:text-amber-300 transition-colors">Đối tác chiến lược</a></li>
                        <li><a href="#bai-viet" class="hover:text-amber-300 transition-colors">Tin tức &amp; Kiến thức nha khoa</a></li>
                        <li><a href="#bao-gia" class="hover:text-amber-300 transition-colors">Đăng ký tư vấn &amp; Nhận báo giá</a></li>
                    </ul>
                </div>

                <!-- Cột 4: Liên hệ trực tiếp -->
                <div>
                    <h4 class="text-sm font-bold text-white uppercase tracking-wide mb-3">Liên Hệ Phòng Khám</h4>
                    <ul class="space-y-2.5 text-xs">
                        <li class="flex items-start gap-2">
                            <i class="fa-solid fa-location-dot text-amber-300 mt-0.5 shrink-0"></i>
                            <span>14 Nguyễn Hữu Thọ, Phường Hòa Cường, TP Đà Nẵng</span>
                        </li>
                        <li class="flex items-center gap-2">
                            <i class="fa-solid fa-phone-volume text-amber-300 shrink-0"></i>
                            <a href="tel:0325274667" class="font-bold text-white hover:text-amber-300 transition-colors">0325.274.667</a>
                        </li>
                        <li class="flex items-center gap-2">
                            <i class="fa-solid fa-globe text-amber-300 shrink-0"></i>
                            <span>thanhlongholdings.vn</span>
                        </li>
                        <li class="flex items-center gap-2">
                            <i class="fa-solid fa-clock text-amber-300 shrink-0"></i>
                            <span>08:00 – 18:30 (Thứ 2 – Chủ Nhật)</span>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="pt-5 flex flex-col sm:flex-row items-center justify-between gap-2 text-[11px] sm:text-xs text-blue-200/80 text-center sm:text-left">
                <p>© 2026 CÔNG TY TNHH THÀNH LONG HOLDINGS. Bảo lưu mọi quyền.</p>
                <p>14 Nguyễn Hữu Thọ, Phường Hòa Cường, TP Đà Nẵng • Hotline: 0325.274.667</p>
            </div>
        </div>
    </footer>

    <!-- ==================== CÁC NÚT LIÊN HỆ NỔI BẬT: ZALO, FACEBOOK, HOTLINE ==================== -->
    <!-- 1. Phiên bản Máy Tính (Cột nổi bên phải, gọn gàng, không che nội dung) -->
    <div class="hidden lg:flex fixed right-4 bottom-6 z-40 flex-col items-end gap-2.5">
        <!-- Zalo -->
        <a
            href="https://zalo.me/0325274667"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="Nhắn Zalo 0325.274.667"
            class="group flex items-center gap-2 bg-[#0068FF] hover:bg-[#0055D4] text-white px-3.5 py-2.5 rounded-full shadow-lg transition-all"
        >
            <span class="w-6 h-6 rounded-full bg-white text-[#0068FF] font-extrabold text-[10px] flex items-center justify-center shrink-0">Zalo</span>
            <span class="text-xs font-bold whitespace-nowrap">Chat Zalo</span>
        </a>
        <!-- Facebook -->
        <a
            href="https://www.facebook.com/"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="Nhắn Facebook Fanpage"
            class="group flex items-center gap-2 bg-[#1877F2] hover:bg-[#1465D1] text-white px-3.5 py-2.5 rounded-full shadow-lg transition-all"
        >
            <i class="fa-brands fa-facebook-f w-6 h-6 rounded-full bg-white text-[#1877F2] text-xs flex items-center justify-center shrink-0"></i>
            <span class="text-xs font-bold whitespace-nowrap">Facebook</span>
        </a>
        <!-- Hotline -->
        <a
            href="tel:0325274667"
            aria-label="Gọi Hotline 0325.274.667"
            class="hotline-pulse flex items-center gap-2 bg-red-600 hover:bg-red-700 text-white px-4 py-2.5 rounded-full shadow-xl transition-all"
        >
            <i class="fa-solid fa-phone-volume text-sm"></i>
            <span class="text-xs font-extrabold tracking-wide whitespace-nowrap">0325.274.667</span>
        </a>
    </div>

    <!-- 2. Phiên bản Điện Thoại & Tablet (Thanh cố định gọn dưới đáy màn hình, dễ chạm, không lệch viền) -->
    <div class="lg:hidden fixed bottom-0 left-0 right-0 z-40 bg-white border-t border-slate-200 shadow-[0_-4px_15px_rgba(0,0,0,0.08)] px-2 py-1.5">
        <div class="grid grid-cols-3 gap-1.5 max-w-full">
            <a
                href="https://zalo.me/0325274667"
                target="_blank"
                rel="noopener noreferrer"
                class="flex items-center justify-center gap-1.5 py-2.5 px-2 rounded-xl bg-[#0068FF] text-white font-bold text-xs shadow-sm active:scale-95 transition-transform"
            >
                <span class="w-5 h-5 rounded-full bg-white text-[#0068FF] text-[9px] font-extrabold flex items-center justify-center shrink-0">Zalo</span>
                <span>Zalo</span>
            </a>
            <a
                href="https://www.facebook.com/"
                target="_blank"
                rel="noopener noreferrer"
                class="flex items-center justify-center gap-1.5 py-2.5 px-2 rounded-xl bg-[#1877F2] text-white font-bold text-xs shadow-sm active:scale-95 transition-transform"
            >
                <i class="fa-brands fa-facebook-messenger text-sm"></i>
                <span>Facebook</span>
            </a>
            <a
                href="tel:0325274667"
                class="flex items-center justify-center gap-1.5 py-2.5 px-2 rounded-xl bg-red-600 text-white font-bold text-xs shadow-sm active:scale-95 transition-transform"
            >
                <i class="fa-solid fa-phone text-xs"></i>
                <span>Hotline</span>
            </a>
        </div>
    </div>

    <!-- ==================== MODAL CHI TIẾT SẢN PHẨM / BÀI VIẾT / PHÓNG TO ẢNH ==================== -->
    <div id="info-modal" class="fixed inset-0 z-50 hidden items-center justify-center p-4 bg-slate-900/65 backdrop-blur-xs">
        <div class="bg-white rounded-2xl max-w-xl w-full max-h-[88vh] overflow-y-auto shadow-2xl border border-slate-200 relative">
            <button id="modal-close" type="button" aria-label="Đóng cửa sổ" class="sticky top-3 float-right mr-3 mt-3 z-10 w-9 h-9 rounded-full bg-slate-100 hover:bg-slate-200 text-slate-700 flex items-center justify-center">
                <i class="fa-solid fa-xmark"></i>
            </button>
            <div id="modal-content" class="p-5 sm:p-6"></div>
        </div>
    </div>

    <!-- ==================== JAVASCRIPT XỬ LÝ TƯƠNG TÁC ==================== -->
    <script>
        /**
         * Hàm dự phòng tải ảnh từ Google Drive nếu link thumbnail đầu tiên bị chậm hoặc lỗi
         */
        function handleImageFallback(img, labelText) {
            if (!img.dataset.triedFallback && img.dataset.fallback) {
                img.dataset.triedFallback = '1';
                img.src = img.dataset.fallback;
                return;
            }
            img.onerror = null;
            const encoded = encodeURIComponent(labelText || 'Thành Long Holdings');
            img.src = `https://placehold.co/800x600/0B4F8C/FFFFFF?text=${encoded}`;
        }

        /**
         * Helper tạo URL ảnh Google Drive chuẩn
         */
        function gdriveImg(id, size = 'w1000') {
            return {
                primary: `https://drive.google.com/thumbnail?id=${id}&sz=${size}`,
                fallback: `https://lh3.googleusercontent.com/d/${id}=${size}`
            };
        }

        /**
         * DỮ LIỆU DANH MỤC SẢN PHẨM & DỊCH VỤ (ĐỒNG BỘ THEO MẪU NHA KHOA APEC & ẢNH THỰC TẾ)
         */
        const PRODUCTS = [
            {
                id: 'cao-voi-rang',
                category: 'tong-quat',
                categoryLabel: 'Chăm sóc răng tổng quát',
                name: 'Cạo Vôi Răng & Đánh Bóng',
                originalPrice: '400.000 ₫',
                salePrice: '200.000 ₫',
                discount: '-50%',
                imgId: '1XyC68CoBLFU9BmuEUAIxB894qYr5ziGY',
                summary: 'Loại bỏ mảng bám, cao răng nhẹ nhàng bằng công nghệ siêu âm hiện đại, giúp hơi thở thơm mát và bảo vệ nướu chắc khỏe.',
                highlights: [
                    'Lấy cao răng bằng máy siêu âm êm ái, hạn chế ê buốt',
                    'Đánh bóng bề mặt men răng sáng sạch tự nhiên',
                    'Kiểm tra tổng quát sức khỏe răng miệng cùng bác sĩ'
                ]
            },
            {
                id: 'boc-rang-su',
                category: 'rang-su',
                categoryLabel: 'Răng sứ thẩm mỹ',
                name: 'Bọc Răng Sứ Thẩm Mỹ',
                originalPrice: '7.000.000 ₫',
                salePrice: '3.500.000 ₫',
                discount: '-50%',
                imgId: '1G-ZbgroUjxsIEb-OZLWsjmqAaEPhBE-W',
                summary: 'Phục hình răng sứ thẩm mỹ tự nhiên, khắc phục tình trạng răng xỉn màu, sứt mẻ, răng thưa với chế độ bảo hành dài hạn.',
                highlights: [
                    'Đa dạng dòng sứ chính hãng cao cấp từ Đức, Mỹ, Nhật',
                    'Thiết kế dáng răng hài hòa đường cười khuôn mặt',
                    'Chế độ bảo hành chính hãng từ 10 năm đến trọn đời'
                ]
            },
            {
                id: 'nieng-rang',
                category: 'nieng-rang',
                categoryLabel: 'Niềng răng',
                name: 'Niềng Răng Chỉnh Nha Mắc Cài',
                originalPrice: '40.000.000 ₫',
                salePrice: '30.000.000 ₫',
                discount: '-25%',
                imgId: '1Rm15eXtU4bwtgeMy3FqK4_EaiBC6CXI2',
                summary: 'Điều chỉnh răng hô, móm, thưa, khấp khểnh chuẩn khớp cắn cùng phác đồ cá nhân hóa và chính sách trả góp linh hoạt.',
                highlights: [
                    'Miễn phí thăm khám và chụp phim chẩn đoán khớp cắn',
                    'Hỗ trợ trả góp 0% lãi suất hàng tháng nhẹ nhàng',
                    'Bác sĩ chỉnh nha trực tiếp theo sát xuyên suốt liệu trình'
                ]
            },
            {
                id: 'trong-rang-implant',
                category: 'implant',
                categoryLabel: 'Cấy ghép Implant',
                name: 'Trồng Răng Implant Chính Hãng',
                originalPrice: '9.900.000 ₫',
                salePrice: '4.500.000 ₫',
                discount: '-55%',
                imgId: '14ADxcu0oIo8V0vZRvQERTTJevBchJTxD',
                summary: 'Giải pháp phục hồi răng mất độc lập bền chắc như răng thật, ngăn ngừa tiêu xương hàm với trụ Implant chính hãng.',
                highlights: [
                    'Trụ Implant chính hãng Hàn Quốc, Thụy Sĩ có mã kiểm tra',
                    'Quy trình cấy ghép vô trùng tuyệt đối chuẩn y khoa',
                    'Khôi phục khả năng ăn nhai ổn định và thẩm mỹ tự nhiên'
                ]
            },
            {
                id: 'su-cercon-ht',
                category: 'rang-su',
                categoryLabel: 'Răng sứ thẩm mỹ',
                name: 'Răng Sứ Cercon HT (BH 15 Năm)',
                originalPrice: '7.500.000 ₫',
                salePrice: '5.600.000 ₫',
                discount: '-25%',
                imgId: '1G-ZbgroUjxsIEb-OZLWsjmqAaEPhBE-W',
                summary: 'Dòng răng toàn sứ cao cấp từ Đức với độ trong mờ tự nhiên, độ bền chịu lực cao và tương thích sinh học tuyệt vời.',
                highlights: [
                    'Phôi sứ Cercon HT nhập khẩu chính hãng từ Đức',
                    'Không đen viền nướu, màu sắc trong bóng tự nhiên',
                    'Thẻ bảo hành chính hãng 15 năm'
                ]
            },
            {
                id: 'invisalign',
                category: 'nieng-rang',
                categoryLabel: 'Niềng răng',
                name: 'Niềng Răng Trong Suốt Invisalign',
                originalPrice: '120.000.000 ₫',
                salePrice: '70.000.000 ₫',
                discount: '-42%',
                imgId: '1Rm15eXtU4bwtgeMy3FqK4_EaiBC6CXI2',
                summary: 'Khay niềng trong suốt thẩm mỹ cao, dễ dàng tháo lắp khi ăn uống và vệ sinh, biết trước kết quả dịch chuyển răng.',
                highlights: [
                    'Khay niềng nhập khẩu chính hãng từ Hoa Kỳ',
                    'Thoải mái giao tiếp, gần như vô hình khi đeo',
                    'Giảm số lần tái khám, phù hợp người bận rộn'
                ]
            },
            {
                id: 'implant-all-on-4',
                category: 'implant',
                categoryLabel: 'Cấy ghép Implant',
                name: 'Trồng Răng Implant All-on-4 Toàn Hàm',
                originalPrice: '150.000.000 ₫',
                salePrice: '135.000.000 ₫',
                discount: '-10%',
                imgId: '14ADxcu0oIo8V0vZRvQERTTJevBchJTxD',
                summary: 'Phục hồi nguyên hàm răng đã mất chỉ với 4 trụ Implant nâng đỡ vững chắc, tiết kiệm thời gian và chi phí tối ưu.',
                highlights: [
                    'Giải pháp tối ưu cho khách hàng mất răng toàn hàm lâu năm',
                    'Lên kế hoạch cấy ghép chính xác với phim CT ConeBeam 3D',
                    'Ăn nhai thoải mái, cải thiện rõ rệt thẩm mỹ khuôn mặt'
                ]
            },
            {
                id: 'tien-chinh-nha-tre-em',
                category: 'tre-em',
                categoryLabel: 'Nha khoa trẻ em',
                name: 'Tiền Chỉnh Nha (Niềng Răng Trẻ Em)',
                originalPrice: '595.000 ₫',
                salePrice: '210.000 ₫',
                discount: '-65%',
                imgId: '1PLpou5lBLqx_rKsh-Ol0j5kL0BmXthz5',
                summary: 'Theo dõi mọc răng và định hướng cung hàm sớm cho trẻ trong độ tuổi vàng, hạn chế nguy cơ lệch khớp cắn về sau.',
                highlights: [
                    'Định hướng xương hàm phát triển cân đối từ sớm',
                    'Không gian phòng khám thân thiện, bác sĩ nhẹ nhàng với bé',
                    'Giảm thiểu tối đa nhu cầu nhổ răng khi trưởng thành'
                ]
            }
        ];

        /**
         * DỮ LIỆU 8 ẢNH THỰC TẾ PHÒNG KHÁM
         */
        const CLINIC_PHOTOS = [
            { id: '1_e548h9zCJwGndxrtHlDtRoqA-n4NOjV', caption: 'Không gian phòng khám hiện đại' },
            { id: '1xLwA2Ti8Ahg1AqoOuqq4c62i-KJF-Sj5', caption: 'Trang thiết bị nha khoa tiêu chuẩn' },
            { id: '1_hbY6U7-qZEkTrRwf3XAsZ1Ob7ES57EM', caption: 'Khu vực sảnh tiếp đón khách hàng' },
            { id: '1aNeZw-QsARSC3XrioPFVkKasrHFKXJ2R', caption: 'Phòng điều trị chuyên biệt vô trùng' },
            { id: '186cqtOqzzcX4i6pBL3OotnPQXtpO0Lje', caption: 'Hệ thống ghế nha khoa cao cấp' },
            { id: '14vcyRWdnHlNtwctljBtFmHGzqFTlDLHb', caption: 'Khu vực tư vấn và thăm khám' },
            { id: '1PLpou5lBLqx_rKsh-Ol0j5kL0BmXthz5', caption: 'Không gian chăm sóc răng miệng tận tâm' },
            { id: '16xV5GO86_HTdrtH76Fl9ykTYYj0UEE1k', caption: 'Cơ sở vật chất chuẩn Bộ Y Tế' }
        ];

        /**
         * DỮ LIỆU 4 BÀI VIẾT TRANG CHỦ
         */
        const ARTICLES = [
            {
                title: 'Chi Phí Trồng Răng Implant Có Được Hỗ Trợ Trả Góp Không?',
                date: '18/11/2026',
                category: 'Cấy ghép Implant',
                imgId: '14ADxcu0oIo8V0vZRvQERTTJevBchJTxD',
                excerpt: 'Tìm hiểu chính sách trả góp linh hoạt khi cấy ghép Implant giúp giảm áp lực tài chính mà vẫn đảm bảo trụ chính hãng.',
                content: 'Trồng răng Implant là giải pháp phục hồi răng mất bền vững hàng đầu hiện nay. Tại Công Ty TNHH Thành Long Holdings, khách hàng được hỗ trợ chính sách thanh toán theo từng giai đoạn điều trị hoặc trả góp linh hoạt lãi suất 0%. Trước khi thực hiện, bác sĩ sẽ thăm khám, chụp phim kiểm tra mật độ xương và báo giá trọn gói minh bạch không phát sinh.'
            },
            {
                title: 'Cập Nhật Quy Trình Niềng Răng Mắc Cài & Trong Suốt Chuẩn Y Khoa',
                date: '12/11/2026',
                category: 'Chỉnh nha',
                imgId: '1Rm15eXtU4bwtgeMy3FqK4_EaiBC6CXI2',
                excerpt: 'Các bước thăm khám, lấy dấu răng, lập phác đồ chỉnh nha an toàn giúp rút ngắn thời gian và ổn định khớp cắn lâu dài.',
                content: 'Một liệu trình niềng răng hiệu quả đòi hỏi quy trình chuẩn xác từ bước khảo sát xương hàm, đánh giá khớp cắn cho đến lựa chọn loại mắc cài kim loại, mắc cài tự khóa hay khay trong suốt Invisalign. Việc tái khám định kỳ đúng lịch giúp kiểm soát lực kéo ổn định và mang lại nụ cười đều đẹp tự nhiên.'
            },
            {
                title: 'Thoát Khỏi Nỗi Lo Mất Răng Toàn Hàm Với Kỹ Thuật Implant All-on-4',
                date: '05/11/2026',
                category: 'Kiến thức nha khoa',
                imgId: '1aNeZw-QsARSC3XrioPFVkKasrHFKXJ2R',
                excerpt: 'Chỉ với 4 trụ Implant đặt chuẩn xác, khách hàng mất răng toàn hàm có thể khôi phục chức năng ăn nhai chắc khỏe.',
                content: 'Mất răng toàn hàm ảnh hưởng nghiêm trọng đến khả năng ăn nhai, tiêu hóa và gây lão hóa khuôn mặt sớm do tiêu xương hàm. Kỹ thuật Implant All-on-4 sử dụng 4 trụ Titanium tương thích sinh học cao làm bệ đỡ vững chắc cho cầu răng cố định nguyên hàm, hạn chế phẫu thuật ghép xương phức tạp.'
            },
            {
                title: 'Bí Quyết Chăm Sóc Răng Sứ Thẩm Mỹ Luôn Sáng Đẹp Và Bền Lâu',
                date: '28/10/2026',
                category: 'Răng sứ thẩm mỹ',
                imgId: '1G-ZbgroUjxsIEb-OZLWsjmqAaEPhBE-W',
                excerpt: 'Hướng dẫn vệ sinh răng miệng đúng cách với bàn chải lông mềm, máy tăm nước và lịch kiểm tra định kỳ 6 tháng/lần.',
                content: 'Sau khi bọc răng sứ thẩm mỹ hoặc dán sứ Veneer, khách hàng nên duy trì chải răng 2 lần mỗi ngày bằng bàn chải lông mềm, kết hợp chỉ nha khoa hoặc máy tăm nước để làm sạch kẽ răng. Tránh cắn trực tiếp vật quá cứng và duy trì lịch cạo vôi, kiểm tra khớp cắn định kỳ 6 tháng/lần tại phòng khám.'
            }
        ];

        let activeCategory = 'all';

        /**
         * Render danh sách sản phẩm chuẩn Flatsome:
         * - 2 cột trên điện thoại, 4 cột trên máy tính
         * - Nhãn % giảm giá góc trên trái
         * - Tên sản phẩm hiển thị đầy đủ, không cắt chữ, không tràn khung
         */
        function renderProducts(filterCat = 'all') {
            const grid = document.getElementById('product-grid');
            if (!grid) return;

            const list = filterCat === 'all'
                ? PRODUCTS
                : PRODUCTS.filter(p => p.category === filterCat);

            grid.innerHTML = list.map(product => {
                const img = gdriveImg(product.imgId, 'w800');
                return `
                    <article class="bg-white rounded-xl sm:rounded-2xl border border-slate-200 hover:border-brand-primary/40 shadow-sm hover:shadow-md transition-all overflow-hidden flex flex-col h-full">
                        <div class="relative aspect-[4/3] bg-slate-100 overflow-hidden cursor-pointer" onclick="openProductModal('${product.id}')">
                            <span class="flatsome-sale-badge">${product.discount}</span>
                            <img
                                src="${img.primary}"
                                data-fallback="${img.fallback}"
                                alt="${product.name}"
                                loading="lazy"
                                class="w-full h-full object-cover hover:scale-105 transition-transform duration-500"
                                onerror="handleImageFallback(this, '${product.name}')"
                            >
                        </div>
                        <div class="p-2.5 sm:p-4 flex flex-col flex-1 justify-between gap-2.5">
                            <div>
                                <p class="text-[10px] sm:text-[11px] font-medium text-slate-500 uppercase tracking-wide mb-1">${product.categoryLabel}</p>
                                <h3 class="text-[13px] sm:text-[15px] font-bold text-slate-800 leading-snug break-words cursor-pointer hover:text-brand-primary transition-colors" onclick="openProductModal('${product.id}')">
                                    ${product.name}
                                </h3>
                            </div>
                            <div class="space-y-2.5">
                                <div class="flex flex-wrap items-baseline gap-x-2 gap-y-0.5">
                                    <span class="text-[11px] sm:text-xs text-slate-400 line-through">${product.originalPrice}</span>
                                    <span class="text-sm sm:text-base font-extrabold text-brand-primary">${product.salePrice}</span>
                                </div>
                                <div class="grid grid-cols-2 gap-1.5 sm:gap-2">
                                    <button type="button" onclick="openProductModal('${product.id}')" class="py-1.5 sm:py-2 px-1.5 sm:px-2.5 rounded-lg border border-brand-primary text-brand-primary hover:bg-brand-light font-semibold text-[11px] sm:text-xs transition-colors text-center">
                                        Chi tiết
                                    </button>
                                    <button type="button" onclick="bookService('${product.name}')" class="py-1.5 sm:py-2 px-1.5 sm:px-2.5 rounded-lg bg-brand-primary hover:bg-brand-dark text-white font-semibold text-[11px] sm:text-xs transition-colors text-center">
                                        Đặt lịch
                                    </button>
                                </div>
                            </div>
                        </div>
                    </article>
                `;
            }).join('');
        }

        /**
         * Lọc sản phẩm theo danh mục
         */
        function filterProducts(cat) {
            activeCategory = cat;
            document.querySelectorAll('.cat-tab').forEach(btn => {
                const isActive = btn.dataset.cat === cat;
                btn.classList.toggle('bg-brand-primary', isActive);
                btn.classList.toggle('text-white', isActive);
                btn.classList.toggle('border-brand-primary', isActive);
                btn.classList.toggle('bg-white', !isActive);
                btn.classList.toggle('text-slate-700', !isActive);
                btn.classList.toggle('border-slate-200', !isActive);
            });
            renderProducts(cat);
        }

        function selectCategoryAndScroll(cat) {
            filterProducts(cat);
            const target = document.getElementById('san-pham');
            if (target) {
                target.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }
        }

        /**
         * Chọn dịch vụ và cuộn tới Form yêu cầu báo giá
         */
        function bookService(serviceName) {
            const selectEl = document.getElementById('q-service');
            const noteEl = document.getElementById('q-note');
            if (selectEl) {
                let matched = false;
                for (let opt of selectEl.options) {
                    if (serviceName.toLowerCase().includes(opt.value.toLowerCase().split(' ')[0])) {
                        selectEl.value = opt.value;
                        matched = true;
                        break;
                    }
                }
                if (!matched) {
                    const customOpt = new Option(serviceName, serviceName, true, true);
                    selectEl.add(customOpt);
                }
            }
            if (noteEl && !noteEl.value.trim()) {
                noteEl.value = `Tôi muốn nhận tư vấn và báo giá chi tiết cho dịch vụ: ${serviceName}.`;
            }
            closeModal();
            const formSection = document.getElementById('bao-gia');
            if (formSection) {
                formSection.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }
        }

        /**
         * Render 8 hình ảnh thực tế phòng khám
         */
        function renderClinicGallery() {
            const container = document.getElementById('clinic-gallery');
            if (!container) return;

            container.innerHTML = CLINIC_PHOTOS.map((photo, idx) => {
                const img = gdriveImg(photo.id, 'w900');
                const largeUrl = gdriveImg(photo.id, 'w1400').primary;
                return `
                    <div class="group bg-white rounded-xl overflow-hidden border border-slate-200 shadow-sm cursor-pointer" onclick="openLightbox('${largeUrl}', '${photo.caption}')">
                        <div class="aspect-[4/3] overflow-hidden bg-slate-100">
                            <img
                                src="${img.primary}"
                                data-fallback="${img.fallback}"
                                alt="${photo.caption} - Thành Long Holdings ${idx + 1}"
                                loading="lazy"
                                class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
                                onerror="handleImageFallback(this, 'Phòng Khám ${idx + 1}')"
                            >
                        </div>
                        <div class="px-2.5 py-2 text-center">
                            <p class="text-[11px] sm:text-xs font-medium text-slate-700 leading-snug">${photo.caption}</p>
                        </div>
                    </div>
                `;
            }).join('');
        }

        /**
         * Render 4 bài viết trang chủ
         */
        function renderArticles() {
            const container = document.getElementById('articles-grid');
            if (!container) return;

            container.innerHTML = ARTICLES.map((article, index) => {
                const img = gdriveImg(article.imgId, 'w800');
                return `
                    <article class="bg-white rounded-2xl border border-slate-200 overflow-hidden shadow-sm hover:shadow-md transition-all flex flex-col">
                        <div class="aspect-[16/10] bg-slate-100 overflow-hidden cursor-pointer" onclick="openArticleModal(${index})">
                            <img
                                src="${img.primary}"
                                data-fallback="${img.fallback}"
                                alt="${article.title}"
                                loading="lazy"
                                class="w-full h-full object-cover hover:scale-105 transition-transform duration-500"
                                onerror="handleImageFallback(this, 'Tin Tức Nha Khoa')"
                            >
                        </div>
                        <div class="p-4 flex flex-col flex-1 justify-between gap-3">
                            <div>
                                <div class="flex items-center justify-between text-[11px] text-slate-500 mb-1.5">
                                    <span class="font-semibold text-brand-primary">${article.category}</span>
                                    <span>${article.date}</span>
                                </div>
                                <h3 class="text-sm font-bold text-slate-800 leading-snug cursor-pointer hover:text-brand-primary transition-colors" onclick="openArticleModal(${index})">
                                    ${article.title}
                                </h3>
                                <p class="text-xs text-slate-600 mt-2 leading-relaxed">
                                    ${article.excerpt}
                                </p>
                            </div>
                            <button type="button" onclick="openArticleModal(${index})" class="inline-flex items-center gap-1.5 text-xs font-bold text-brand-primary hover:text-brand-accent transition-colors self-start">
                                <span>Đọc tiếp</span>
                                <i class="fa-solid fa-arrow-right text-[10px]"></i>
                            </button>
                        </div>
                    </article>
                `;
            }).join('');
        }

        /**
         * Modal hiển thị chi tiết sản phẩm, bài viết hoặc ảnh phóng to
         */
        const modalEl = document.getElementById('info-modal');
        const modalContent = document.getElementById('modal-content');

        function openModal(html) {
            modalContent.innerHTML = html;
            modalEl.classList.remove('hidden');
            modalEl.classList.add('flex');
            document.body.style.overflow = 'hidden';
        }

        function closeModal() {
            modalEl.classList.add('hidden');
            modalEl.classList.remove('flex');
            document.body.style.overflow = '';
        }

        function openProductModal(productId) {
            const p = PRODUCTS.find(item => item.id === productId);
            if (!p) return;
            const img = gdriveImg(p.imgId, 'w1000');
            openModal(`
                <div class="space-y-4">
                    <div class="relative aspect-[16/10] rounded-xl overflow-hidden bg-slate-100">
                        <span class="flatsome-sale-badge">${p.discount}</span>
                        <img src="${img.primary}" data-fallback="${img.fallback}" alt="${p.name}" class="w-full h-full object-cover" onerror="handleImageFallback(this, '${p.name}')">
                    </div>
                    <div>
                        <p class="text-xs font-semibold text-brand-accent uppercase">${p.categoryLabel}</p>
                        <h3 class="text-lg sm:text-xl font-extrabold text-brand-primary mt-1">${p.name}</h3>
                        <div class="flex items-baseline gap-3 mt-2">
                            <span class="text-sm text-slate-400 line-through">${p.originalPrice}</span>
                            <span class="text-xl font-extrabold text-brand-primary">${p.salePrice}</span>
                        </div>
                    </div>
                    <p class="text-sm text-slate-600 leading-relaxed">${p.summary}</p>
                    <div class="bg-slate-50 rounded-xl p-4 border border-slate-200">
                        <p class="text-xs font-bold text-slate-800 uppercase mb-2">Ưu điểm nổi bật:</p>
                        <ul class="space-y-1.5 text-xs sm:text-sm text-slate-700 list-disc list-inside">
                            ${p.highlights.map(h => `<li>${h}</li>`).join('')}
                        </ul>
                    </div>
                    <div class="flex flex-wrap gap-2.5 pt-1">
                        <button type="button" onclick="bookService('${p.name}')" class="flex-1 py-2.5 px-4 rounded-xl bg-brand-primary hover:bg-brand-dark text-white font-bold text-sm transition-colors">
                            Đăng ký báo giá dịch vụ này
                        </button>
                        <a href="tel:0325274667" class="py-2.5 px-4 rounded-xl border border-brand-primary text-brand-primary hover:bg-brand-light font-bold text-sm transition-colors">
                            Gọi 0325.274.667
                        </a>
                    </div>
                </div>
            `);
        }

        function openArticleModal(index) {
            const a = ARTICLES[index];
            if (!a) return;
            const img = gdriveImg(a.imgId, 'w1000');
            openModal(`
                <div class="space-y-4">
                    <div class="aspect-[16/9] rounded-xl overflow-hidden bg-slate-100">
                        <img src="${img.primary}" data-fallback="${img.fallback}" alt="${a.title}" class="w-full h-full object-cover" onerror="handleImageFallback(this, 'Bài Viết')">
                    </div>
                    <div class="flex items-center gap-3 text-xs text-slate-500">
                        <span class="font-bold text-brand-primary">${a.category}</span>
                        <span>•</span>
                        <span>${a.date}</span>
                    </div>
                    <h3 class="text-lg sm:text-xl font-extrabold text-slate-900 leading-snug">${a.title}</h3>
                    <p class="text-sm text-slate-700 leading-relaxed">${a.content}</p>
                    <div class="pt-2 border-t border-slate-200 flex items-center justify-between gap-2">
                        <span class="text-xs text-slate-500">CÔNG TY TNHH THÀNH LONG HOLDINGS</span>
                        <button type="button" onclick="bookService('${a.category}')" class="px-4 py-2 rounded-xl bg-brand-primary hover:bg-brand-dark text-white text-xs font-bold transition-colors">
                            Đặt lịch tư vấn
                        </button>
                    </div>
                </div>
            `);
        }

        function openLightbox(imgUrl, caption) {
            openModal(`
                <div class="space-y-3 pt-2">
                    <div class="rounded-xl overflow-hidden bg-slate-100">
                        <img src="${imgUrl}" alt="${caption}" class="w-full max-h-[65vh] object-contain mx-auto" onerror="handleImageFallback(this, '${caption}')">
                    </div>
                    <p class="text-center text-sm font-semibold text-slate-700">${caption}</p>
                </div>
            `);
        }

        /**
         * Khởi chạy Slider 2 banner tự trượt (hỗ trợ cả click nút & vuốt cảm ứng trên điện thoại)
         */
        function initBannerSlider() {
            const slides = document.querySelectorAll('.banner-slide');
            const dots = document.querySelectorAll('.banner-dot');
            const prevBtn = document.getElementById('banner-prev');
            const nextBtn = document.getElementById('banner-next');
            const sliderEl = document.getElementById('hero-slider');
            let currentIndex = 0;
            let autoTimer = null;

            function showSlide(index) {
                currentIndex = (index + slides.length) % slides.length;
                slides.forEach((s, i) => {
                    s.classList.toggle('active', i === currentIndex);
                });
                dots.forEach((d, i) => {
                    if (i === currentIndex) {
                        d.classList.add('w-6', 'bg-amber-400');
                        d.classList.remove('w-2', 'bg-white/50');
                    } else {
                        d.classList.remove('w-6', 'bg-amber-400');
                        d.classList.add('w-2', 'bg-white/50');
                    }
                });
            }

            function startAuto() {
                stopAuto();
                autoTimer = setInterval(() => showSlide(currentIndex + 1), 5000);
            }

            function stopAuto() {
                if (autoTimer) clearInterval(autoTimer);
            }

            prevBtn?.addEventListener('click', () => { showSlide(currentIndex - 1); startAuto(); });
            nextBtn?.addEventListener('click', () => { showSlide(currentIndex + 1); startAuto(); });
            dots.forEach(dot => {
                dot.addEventListener('click', () => {
                    showSlide(Number(dot.dataset.slide));
                    startAuto();
                });
            });

            // Hỗ trợ vuốt trái/phải trên điện thoại
            let touchStartX = 0;
            sliderEl?.addEventListener('touchstart', (e) => {
                touchStartX = e.changedTouches[0].screenX;
            }, { passive: true });
            sliderEl?.addEventListener('touchend', (e) => {
                const diff = e.changedTouches[0].screenX - touchStartX;
                if (Math.abs(diff) > 45) {
                    if (diff < 0) showSlide(currentIndex + 1);
                    else showSlide(currentIndex - 1);
                    startAuto();
                }
            }, { passive: true });

            sliderEl?.addEventListener('mouseenter', stopAuto);
            sliderEl?.addEventListener('mouseleave', startAuto);

            showSlide(0);
            startAuto();
        }

        /**
         * Menu điện thoại & xử lý form báo giá
         */
        document.addEventListener('DOMContentLoaded', () => {
            try {
                renderProducts('all');
                renderClinicGallery();
                renderArticles();
                initBannerSlider();

                // Tabs lọc sản phẩm
                document.querySelectorAll('.cat-tab').forEach(btn => {
                    btn.addEventListener('click', () => filterProducts(btn.dataset.cat));
                });

                // Đóng modal
                document.getElementById('modal-close')?.addEventListener('click', closeModal);
                modalEl?.addEventListener('click', (e) => {
                    if (e.target === modalEl) closeModal();
                });

                // Drawer menu trên điện thoại
                const drawer = document.getElementById('mobile-drawer');
                const overlay = document.getElementById('mobile-drawer-overlay');
                const openBtn = document.getElementById('mobile-menu-btn');
                const closeBtn = document.getElementById('mobile-menu-close');

                function openDrawer() {
                    drawer.classList.remove('-translate-x-full');
                    overlay.classList.remove('hidden');
                    document.body.style.overflow = 'hidden';
                }
                function closeDrawer() {
                    drawer.classList.add('-translate-x-full');
                    overlay.classList.add('hidden');
                    document.body.style.overflow = '';
                }

                openBtn?.addEventListener('click', openDrawer);
                closeBtn?.addEventListener('click', closeDrawer);
                overlay?.addEventListener('click', closeDrawer);
                document.querySelectorAll('.mobile-nav-link').forEach(link => {
                    link.addEventListener('click', closeDrawer);
                });

                // Form yêu cầu & báo giá (không dùng alert())
                const quoteForm = document.getElementById('quote-form');
                const feedback = document.getElementById('quote-feedback');
                quoteForm?.addEventListener('submit', (e) => {
                    e.preventDefault();
                    const name = document.getElementById('q-name').value.trim();
                    const phone = document.getElementById('q-phone').value.trim();
                    const service = document.getElementById('q-service').value;

                    if (!name || phone.length < 9) {
                        feedback.className = 'p-3.5 rounded-xl text-xs sm:text-sm font-medium bg-red-50 text-red-700 border border-red-200';
                        feedback.textContent = 'Vui lòng nhập đầy đủ họ tên và số điện thoại hợp lệ để chúng tôi liên hệ báo giá.';
                        feedback.classList.remove('hidden');
                        return;
                    }

                    feedback.className = 'p-3.5 rounded-xl text-xs sm:text-sm font-medium bg-emerald-50 text-emerald-800 border border-emerald-200';
                    feedback.innerHTML = `Cảm ơn <strong>${name}</strong>! Yêu cầu báo giá dịch vụ <strong>${service}</strong> đã được ghi nhận. Chuyên viên Thành Long Holdings sẽ gọi lại qua số <strong>${phone}</strong> trong ít phút.`;
                    feedback.classList.remove('hidden');
                    quoteForm.reset();
                });
            } catch (err) {
                console.error('Lỗi khởi tạo giao diện:', err);
            }
        });
    </script>
</body>
</html>
