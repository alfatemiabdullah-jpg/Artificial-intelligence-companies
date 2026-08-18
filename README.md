# Artificial-intelligence-companies<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ماث-جينيس AI | المنصة الأقوى عالمياً لتعلم الرياضيات</title>
    <style>
        :root {
            --bg-dark: #090d16;
            --card-dark: #131c2e;
            --primary-blue: #2563eb;
            --accent-cyan: #06b6d4;
            --accent-green: #10b981;
            --premium-gold: #f59e0b;
            --text-light: #f8fafc;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, sans-serif; }
        body { background-color: var(--bg-dark); color: var(--text-light); line-height: 1.6; padding-bottom: 40px; }
        
        /* الهيدر الاحترافي */
        header { background-color: rgba(9, 13, 22, 0.85); border-bottom: 1px solid #1e293b; position: fixed; width: 100%; top: 0; z-index: 100; backdrop-filter: blur(12px); }
        .nav-container { max-width: 1200px; margin: 0 auto; padding: 1rem 2rem; display: flex; justify-content: space-between; align-items: center; }
        .logo { font-size: 1.5rem; font-weight: bold; background: linear-gradient(to left, var(--accent-cyan), var(--primary-blue)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
        
        .score-badge { background: #1e293b; padding: 0.5rem 1rem; border-radius: 50px; font-weight: bold; border: 1px solid var(--accent-cyan); display: flex; align-items: center; gap: 0.5rem; }

        /* حاوية التصميم الرئيسية */
        .container { max-width: 1200px; margin: 8rem auto 2rem auto; padding: 0 2rem; display: grid; grid-template-columns: 2fr 1fr; gap: 2rem; }
        @media (max-width: 900px) { .container { grid-template-columns: 1fr; margin-top: 6rem; } }

        .main-content, .sidebar { background-color: var(--card-dark); padding: 2rem; border-radius: 16px; border: 1px solid #1e293b; box-shadow: 0 10px 25px rgba(0,0,0,0.3); }
        
        .lesson-box h2 { color: var(--accent-cyan); margin-bottom: 1rem; font-size: 1.8rem; }
        .quiz-box { margin-top: 2rem; padding-top: 2rem; border-top: 1px solid #1e293b; }
        
        /* أزرار الخيارات */
        .option-btn { display: block; width: 100%; padding: 1rem; margin: 0.6rem 0; background-color: #1e293b; color: white; border: 1px solid #334155; border-radius: 8px; cursor: pointer; text-align: right; font-size: 1rem; transition: all 0.2s; }
        .option-btn:hover { background-color: #2563eb; transform: scale(1.01); border-color: var(--accent-cyan); }
        
        /* نظام الدردشة المطور */
        .chat-container { position: relative; }
        .chat-area { height: 280px; overflow-y: auto; border: 1px solid #1e293b; background: #090d16; padding: 1rem; border-radius: 8px; margin-bottom: 1rem; }
        .chat-input-group { display: flex; gap: 0.5rem; }
        .chat-input { flex: 1; padding: 0.75rem; border-radius: 8px; border: 1px solid #334155; background: #1e293b; color: white; }
        .send-btn { background: var(--primary-blue); color: white; border: none; padding: 0 1.5rem; border-radius: 8px; cursor: pointer; font-weight: bold; }
        
        .msg { margin-bottom: 0.8rem; padding: 0.6rem 0.9rem; border-radius: 8px; max-width: 85%; font-size: 0.95rem; }
        .bot { background: #1e293b; border-right: 4px solid var(--primary-blue); }
        .user { background: var(--primary-blue); margin-right: auto; text-align: left; }
        
        /* جدار الحماية للاشتراك المدفوع (Paywall) */
        .paywall-overlay { position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: rgba(19, 28, 46, 0.95); backdrop-filter: blur(8px); display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; padding: 2rem; border-radius: 8px; z-index: 10; border: 2px solid var(--premium-gold); }
        .premium-btn { background: linear-gradient(45deg, var(--premium-gold), #ed8936); color: #090d16; font-weight: bold; padding: 0.8rem 2rem; border: none; border-radius: 50px; font-size: 1.1rem; cursor: pointer; margin-top: 1rem; transition: transform 0.2s; width: 100%; }
        .premium-btn:hover { transform: scale(1.05); box-shadow: 0 0 15px rgba(245, 158, 11, 0.4); }

        /* لوحة الصدارة وعناصر حماسية */
        .leaderboard { margin-top: 2rem; background: #090d16; padding: 1rem; border-radius: 8px; border: 1px solid #1e293b; }
        .leaderboard-title { color: var(--premium-gold); font-size: 1rem; margin-bottom: 0.5rem; display: flex; align-items: center; gap: 0.5rem; }
        .user-row { display: flex; justify-content: space-between; padding: 0.4rem 0; border-bottom: 1px solid #131c2e; font-size: 0.85rem; }
        .user-row.active { color: var(--accent-cyan); font-weight: bold; }
    </style>
</head>
<body>

    <!-- الهيدر ولوحة النقاط -->
    <header>
        <div class="nav-container">
            <div class="logo">⚡ MATH-GENIUS AI</div>
            <div class="score-badge">
                <span>🏆 نقاطك:</span>
                <span id="userPoints">0</span>
            </div>
        </div>
    </header>

    <div class="container">
        <!-- منطقة التعلم والتفاعل -->
        <main class="main-content">
            <div class="lesson-box">
                <span style="color: var(--accent-cyan); font-weight: bold; font-size: 0.85rem; text-transform: uppercase;">المستوى 1: الجبر الذكي</span>
                <h2>المعادلات من الدرجة الأولى 📐</h2>
                <p style="color: #94a3b8; margin-bottom: 1.5rem;">أهلاً بك يا عبقري! لجعل "س" فائزاً وحيداً، انقل أي رقم للطرف الآخر واعكس إشارته فوراً!</p>
                <div style="background: #090d16; padding: 1.5rem; border-radius: 8px; text-align: center; font-size: 1.5rem; color: var(--accent-green); border: 1px solid #1e293b;">
                    س + 5 = 12 <br>
                    س = 12 - 5 <br>
                    <strong>س = 7 ✨</strong>
                </div>
            </div>

            <!-- التمارين التفاعلية لتجميع النقاط -->
            <div class="quiz-box">
                <h3>📝 تحدي السرعة (اكسب +10 نقاط):</h3>
                <p style="margin: 0.8rem 0; font-size: 1.1rem; color: #cbd5e1;">إذا كان: <span style="color: var(--premium-gold);">٣س = ١٥</span> ، فما هي قيمة س؟</p>
                <button class="option-btn" onclick="checkAnswer(this, false)">أ) س = ٣</button>
                <button class="option-btn" onclick="checkAnswer(this, true)">ب) س = ٥ (اضغط هنا لتجربة الإجابة)</button>
                <button class="option-btn" onclick="checkAnswer(this, false)">ج) س = ٤٥</button>
                <p id="quiz-feedback" style="margin-top: 1rem; font-weight: bold; text-align: center; font-size: 1.1rem;"></p>
            </div>
        </main>

        <!-- السايدبار مع المساعد الذكي المقفل بنظام الدفع -->
        <aside class="sidebar">
            <h3 style="margin-bottom: 1rem; display: flex; align-items: center; gap: 0.5rem;">🤖 مساعد الذكاء الاصطناعي</h3>
            
            <div class="chat-container">
                <!-- جدار الدفع الحقيقي (Paywall) -->
                <div class="paywall-overlay" id="paywall">
                    <span style="font-size: 2.5rem;">👑</span>
                    <h3 style="color: var(--premium-gold); margin-bottom: 0.5rem;">افتح العبقرية الكاملة</h3>
                    <p style="font-size: 0.85rem; color: #94a3b8;">المساعد الذكي مقفل حالياً. اشترك لتسأل ذكاءنا الاصطناعي عن أي مسألة صعبة خطوة بخطوة!</p>
                    <button class="premium-btn" onclick="unlockPremium()">اشترك الآن بـ 5 رينجت (1$) فقط 💳</button>
                </div>

                <!-- صندوق الدردشة (يفتح بعد الدفع) -->
                <div class="chat-area" id="chatBox">
                    <div class="msg bot">تم تفعيل النسخة المدفوعة بنجاح! 🎉 أنا الآن جاهز لحل أي معادلة مستعصية معك. اكتب سؤالك!</div>
                </div>
                <div class="chat-input-group">
                    <input type="text" id="userInput" class="chat-input" placeholder="اكتب مسألتك الصعبة..." disabled>
                    <button class="send-btn" id="sendBtn" onclick="sendMessage()" disabled>إرسال</button>
                </div>
            </div>

            <!-- لوحة المتصدرين لإشعال الحماس -->
            <div class="leaderboard">
                <div class="leaderboard-title">🏆 لوحة عباقرة العالم اليوم</div>
                <div class="user-row"><span>1. أحمد المالي (ماليزيا)</span><span>⭐ 150 نقطة</span></div>
                <div class="user-row"><span>2. سارة علي (السعودية)</span><span>⭐ 120 نقطة</span></div>
                <div class="user-row active"><span>3. أنت (عبقري مستقبلي)</span><span id="leaderboardPoints">⭐ 0 نقطة</span></div>
            </div>
        </aside>
    </div>

    <script>
        let points = 0;

        // ميزة تفاعلية: التحقق من الإجابة وزيادة النقاط وتحديث لوحة المتصدرين
        function checkAnswer(button, isCorrect) {
            const feedback = document.getElementById('quiz-feedback');
            if(isCorrect) {
                feedback.innerHTML = "🎉 رائـع! إجابة صحيحة. تم إضافة +10 نقاط لرصيدك!";
                feedback.style.color = "var(--accent-green)";
                if(points === 0) {
                    points += 10;
                    document.getElementById('userPoints').innerText = points;
                    document.getElementById('leaderboardPoints').innerText = "⭐ " + points + " نقطة";
                }
            } else {
                feedback.innerHTML = "❌ ركز قليلاً! تذكر أن تقسم الطرفين على ٣ للتخلص من المعامل.";
                feedback.style.color = "#ef4444";
            }
        }

        // ميزة الاشتراك الفوري: إخفاء حائط الدفع وتفعيل المساعد الذكي
        function unlockPremium() {
            // محاكاة لعملية دفع ناجحة بـ 5 رينجت / 1 دولار
            alert("💳 جاري الاتصال ببوابة الدفع الآمنة...\nتمت عملية الدفع بنجاح! شكراً لاشتراكك في MATH-GENIUS AI.");
            document.getElementById('paywall').style.display = 'none';
