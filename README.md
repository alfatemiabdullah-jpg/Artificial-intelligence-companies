# Artificial-intelligence-companies <!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تكنو-ستور AI | حلول الذكاء الاصطناعي للتجارة الإلكترونية</title>
    <style>
        :root {
            --primary-color: #0f172a;
            --secondary-color: #2563eb;
            --accent-color: #38bdf8;
            --text-color: #f8fafc;
            --bg-light: #1e293b;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--primary-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        /* الهيدر والقائمة */
        header {
            background-color: rgba(15, 23, 42, 0.9);
            backdrop-filter: blur(10px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid #334155;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--accent-color);
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            color: var(--text-color);
            text-decoration: none;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--accent-color);
        }

        /* القسم الرئيسي */
        .hero {
            padding: 10rem 2rem 6rem 2rem;
            text-align: center;
            background: radial-gradient(circle at center, #1e3a8a 0%, var(--primary-color) 70%);
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            color: #fff;
        }

        .hero h1 span {
            color: var(--accent-color);
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto 2rem auto;
            color: #cbd5e1;
        }

        .btn {
            background-color: var(--secondary-color);
            color: white;
            padding: 0.75rem 2rem;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            text-decoration: none;
            transition: background 0.3s;
            display: inline-block;
        }

        .btn:hover {
            background-color: #1d4ed8;
        }

        /* قسم الخدمات */
        .services {
            max-width: 1200px;
            margin: 0 auto;
            padding: 5rem 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 3rem;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background-color: var(--bg-light);
            padding: 2.5rem;
            border-radius: 10px;
            border: 1px solid #334155;
            transition: transform 0.3s, border-color 0.3s;
        }

        .service-card:hover {
            transform: translateY(-5px);
            border-color: var(--accent-color);
        }

        .service-card h3 {
            margin-bottom: 1rem;
            color: var(--accent-color);
        }

        /* الفوتر */
        footer {
            background-color: #090d16;
            text-align: center;
            padding: 2rem;
            margin-top: 5rem;
            border-top: 1px solid #334155;
            font-size: 0.9rem;
            color: #64748b;
        }
    </style>
</head>
<body>

    <!-- الهيدر -->
    <header>
        <div class="nav-container">
            <div class="logo">🚀 تكنو-ستور AI</div>
            <ul class="nav-links">
                <li><a href="#home">الرئيسية</a></li>
                <li><a href="#services">خدماتنا</a></li>
                <li><a href="#contact">اتصل بنا</a></li>
            </ul>
        </div>
    </header>

    <!-- القسم الرئيسي -->
    <section class="hero" id="home">
        <h1>ضاعف مبيعات متجرك الإلكتروني بـ <span>الذكاء الاصطناعي</span></h1>
        <p>نحن نساعد المتاجر الإلكترونية الكبرى والناشئة على أتمتة خدمة العملاء، وتخصيص تجربة الشراء، وزيادة الأرباح الذكية بدون عناء.</p>
        <a href="#services" class="btn">اكتشف حلولنا الذكية</a>
    </section>

    <!-- قسم الخدمات -->
    <section class="services" id="services">
        <h2 class="section-title">حلولنا الذكية للمتاجر</h2>
        <div class="services-grid">
            <div class="service-card">
                <h3>💬 مساعد خدمة العملاء الذكي</h3>
                <p>ردود فورية وذكية على استفسارات المشترين وحل مشاكل الشحن والطلب على مدار الساعة طوال الأسبوع.</p>
            </div>
            <div class="service-card">
                <h3>🎯 محرك التوصيات الشخصية</h3>
                <p>تحليل سلوك الزوار واقتراح المنتجات المناسبة لكل عميل بدقة لرفع قيمة السلة الشرائية.</p>
            </div>
            <div class="service-card">
                <h3>✍️ توليد محتوى المنتجات</h3>
                <p>كتابة وصف احترافي، عناوين، وإعلانات تسويقية لآلاف المنتجات بضغطة زر واحدة بذكاء وموثوقية.</p>
            </div>
        </div>
    </section>

    <!-- الفوتر -->
    <footer>
        <p>&copy; 2026 جميع الحقوق محفوظة لشركة تكنو-ستور AI</p>
    </footer>

</body>
</html>
