# Artificial-intelligence-companies<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ماث-جينيس AI | تعلم الرياضيات بذكاء</title>
    <style>
        :root {
            --bg-dark: #0f172a;
            --card-dark: #1e293b;
            --primary-blue: #3b82f6;
            --accent-green: #10b981;
            --text-light: #f8fafc;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, sans-serif; }
        body { background-color: var(--bg-dark); color: var(--text-light); line-height: 1.6; padding-bottom: 60px; }
        
        header { background-color: rgba(15, 23, 42, 0.9); border-bottom: 1px solid #334155; position: fixed; width: 100%; top: 0; z-index: 100; backdrop-filter: blur(10px); }
        .nav-container { max-width: 1100px; margin: 0 auto; padding: 1rem 2rem; display: flex; justify-content: space-between; align-items: center; }
        .logo { font-size: 1.4rem; font-weight: bold; color: var(--primary-blue); }

        .container { max-width: 1100px; margin: 8rem auto 2rem auto; padding: 0 2rem; display: grid; grid-template-columns: 2fr 1fr; gap: 2rem; }
        @media (max-width: 768px) { .container { grid-template-columns: 1fr; margin-top: 6rem; } }

        .main-content, .sidebar { background-color: var(--card-dark); padding: 2rem; border-radius: 12px; border: 1px solid #334155; }
        
        .lesson-box h2 { color: var(--primary-blue); margin-bottom: 1rem; }
        .quiz-box { margin-top: 2rem; padding-top: 2rem; border-top: 1px solid #334155; }
        
        .option-btn { display: block; width: 100%; padding: 0.75rem; margin: 0.5rem 0; background-color: #334155; color: white; border: 1px solid #475569; border-radius: 6px; cursor: pointer; text-align: right; font-size: 1rem; transition: 0.2s; }
        .option-btn:hover { background-color: #475569; }
        
        .chat-area { height: 250px; overflow-y: auto; border: 1px solid #334155; background: #0f172a; padding: 1rem; border-radius: 6px; margin-bottom: 1rem; }
        .chat-input-group { display: flex; gap: 0.5rem; }
        .chat-input { flex: 1; padding: 0.75rem; border-radius: 6px; border: 1px solid #334155; background: #1e293b; color: white; }
        .send-btn { background: var(--primary-blue); color: white; border: none; padding: 0 1.5rem; border-radius: 6px; cursor: pointer; }
        
        .msg { margin-bottom: 0.8rem; padding: 0.5rem 0.8rem; border-radius: 6px; max-width: 85%; font-size: 0.9rem; }
        .bot { background: #2563eb; align-self: flex-start; }
        .user { background: #475569; margin-right: auto; text-align: left; }
        
        .premium-badge { background: #f59e0b; color: #0f172a; padding: 0.2rem 0.5rem; font-size: 0.7rem; font-weight: bold; border-radius: 4px; inline-size: max-content; margin-bottom: 0.5rem; }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo">📐 ماث-جينيس AI</div>
            <span style="color: #64748b; font-size: 0.9rem;">نسخة تجريبية مجانية v1.0</span>
        </div>
    </header>

    <div class="container">
        <!-- منطقة الشرح والتمارين (شغل شريك المنتج) -->
        <main class="main-content">
            <div class="lesson-box">
                <h2>الدرس الأول: حل المعادلات من الدرجة الأولى</h2>
                <p style="color: #94a3b8; margin-bottom: 1rem;">المعادلة هي كفة ميزان متساوية، هدفنا دائماً هو جعل الحرف (س) وحيداً في طرف.</p>
                <div style="background: #0f172a; padding: 1rem; border-radius: 6px; font-family: monospace; text-align: center; font-size: 1.3rem; color: var(--accent-green);">
                    س + 5 = 12 <br>
                    س = 12 - 5 <br>
                    <strong>س = 7</strong>
                </div>
            </div>

            <div class="quiz-box">
                <h3>📝 اختبر فهمك الآن:</h3>
                <p style="margin: 0.5rem 0; color: #94a3b8;">إذا كان: ٢س = ١٠ ، فما هي قيمة س؟</p>
                <button class="option-btn" onclick="checkAnswer(this, false)">أ) س = ٢</button>
                <button class="option-btn" onclick="checkAnswer(this, true)">ب) س = ٥ (إجابة صحيحة)</button>
                <button class="option-btn" onclick="checkAnswer(this, false)">ج) س = ١٢</button>
                <p id="quiz-feedback" style="margin-top: 1rem; font-weight: bold;"></p>
            </div>
        </main>

        <!-- المساعد الذكي التجريبي والميزات المدفوعة -->
        <aside class="sidebar">
            <div class="premium-badge">ميزة تجريبية محدودة</div>
            <h3 style="margin-bottom: 1rem;">🤖 مساعد الرياضيات الذكي</h3>
            <div class="chat-area" id="chatBox">
                <div class="msg bot">أهلاً بك! أنا مساعدك الذكي في الرياضيات. اسألني أي سؤال في درس اليوم!</div>
            </div>
            <div class="chat-input-group">
                <input type="text" id="userInput" class="chat-input" placeholder="اكتب سؤالك هنا...">
                <button class="send-btn" onclick="sendMessage()">إرسال</button>
            </div>
            
            <div style="margin-top: 2rem; background: #2d3748; padding: 1rem; border-radius: 6px; border: 1px dashed #f59e0b;">
                <h4 style="color: #f59e0b; margin-bottom: 0.5rem;">👑 الباقة الممتازة ($5/شهرياً)</h4>
                <p style="font-size: 0.8rem; color: #cbd5e1;">احصل على غرف زووم أسبوعية لحل الواجبات ومساعد ذكي غير محدود لـ 500 مسألة.</p>
            </div>
        </aside>
    </div>

    <script>
        function checkAnswer(button, isCorrect) {
            const feedback = document.getElementById('quiz-feedback');
            if(isCorrect) {
                feedback.innerHTML = "🎉 أحسنت! إجابة صحيحة تماماً.";
                feedback.style.color = "#10b981";
            } else {
                feedback.innerHTML = "❌ حاول مرة أخرى، تذكر أن تقسم الطرفين على ٢.";
                feedback.style.color = "#ef4444";
            }
        }

        function sendMessage() {
            const input = document.getElementById('userInput');
            const chatBox = document.getElementById('chatBox');
            if(input.value.trim() === '') return;

            // رسالة المستخدم
            let userDiv = document.createElement('div');
            userDiv.className = 'msg user';
            userDiv.innerText = input.value;
            chatBox.appendChild(userDiv);

            // رد محاكي تلقائي ذكي
            setTimeout(() => {
                let botDiv = document.createElement('div');
                botDiv.className = 'msg bot';
                botDiv.innerText = "سؤال ممتاز! لحل هذا النوع من المسائل، يجب أولاً التخلص من الأرقام المضافة بجانب المتغير. هل تود أن نحلها خطوة بخطوة؟";
                chatBox.appendChild(botDiv);
                chatBox.scrollTop = chatBox.scrollHeight;
            }, 800);

            input.value = '';
            chatBox.scrollTop = chatBox.scrollHeight;
        }
    </script>
</body>
</html>
