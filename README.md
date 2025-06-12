<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>روبوت تتبع الإنسان - مشروع أردوينو</title>
    <style>
        :root {
            --primary: #2b3137;
            --secondary: #586069;
            --accent: #0366d6;
            --bg: #ffffff;
            --card-bg: #f6f8fa;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--primary);
            background-color: var(--bg);
            max-width: 900px;
            margin: 0 auto;
            padding: 20px;
        }
        
        h1, h2, h3 {
            color: var(--primary);
            margin-top: 24px;
            margin-bottom: 16px;
        }
        
        h1 {
            font-size: 2em;
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
        }
        
        h2 {
            font-size: 1.5em;
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
        }
        
        img {
            max-width: 100%;
            border-radius: 6px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }
        
        .header {
            text-align: center;
            margin-bottom: 30px;
        }
        
        .header img {
            max-height: 300px;
            object-fit: cover;
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .feature-card {
            background: var(--card-bg);
            padding: 20px;
            border-radius: 6px;
            border: 1px solid #e1e4e8;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        
        table, th, td {
            border: 1px solid #dfe2e5;
        }
        
        th, td {
            padding: 12px;
            text-align: right;
        }
        
        th {
            background-color: var(--card-bg);
        }
        
        tr:nth-child(even) {
            background-color: var(--card-bg);
        }
        
        .code-block {
            background-color: #f6f8fa;
            padding: 16px;
            border-radius: 6px;
            font-family: 'Courier New', Courier, monospace;
            overflow-x: auto;
        }
        
        .badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 20px 0;
        }
        
        .badge {
            display: inline-block;
            padding: 5px 10px;
            background-color: var(--primary);
            color: white;
            border-radius: 20px;
            font-size: 0.8em;
            text-decoration: none;
        }
        
        .wiring-diagram {
            text-align: center;
            margin: 30px 0;
        }
        
        .file-structure {
            background-color: var(--card-bg);
            padding: 15px;
            border-radius: 6px;
            font-family: 'Courier New', Courier, monospace;
        }
        
        .troubleshooting {
            width: 100%;
        }
        
        .footer {
            margin-top: 40px;
            text-align: center;
            padding: 20px;
            border-top: 1px solid #eaecef;
        }
        
        @media (max-width: 768px) {
            .features {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>🤖 روبوت تتبع الإنسان - مشروع أردوينو</h1>
        <img src="./images/433319f6-4cfd-435d-afbe-c8104b8f43f7.jfif" alt="روبوت تتبع الإنسان">
    </div>

    <section>
        <h2>📝 نظرة عامة</h2>
        <p>روبوت ذكي قادر على تتبع الأشخاص تلقائياً باستخدام تقنيات الاستشعار عن بعد. يتميز هذا المشروع بدقة الحركة وسهولة التصنيع، مما يجعله مثالياً لمشاريع الروبوتات التعليمية.</p>
    </section>

    <section>
        <h2>✨ المميزات الرئيسية</h2>
        <div class="features">
            <div class="feature-card">
                <h3>🎯 نظام تتبع ذكي</h3>
                <p>يستخدم حساسات متعددة لتتبع الحركة بدقة</p>
            </div>
            <div class="feature-card">
                <h3>⚙️ تحكم دقيق</h3>
                <p>أربع محركات للحركة في جميع الاتجاهات</p>
            </div>
            <div class="feature-card">
                <h3>🔍 مسح محيطي</h3>
                <p>زاوية مسح 180 درجة لتحديد الاتجاه</p>
            </div>
        </div>
    </section>

    <section>
        <h2>📦 قائمة المكونات</h2>
        <table>
            <tr>
                <th>المكون</th>
                <th>الكمية</th>
                <th>الصورة</th>
                <th>ملاحظات</th>
            </tr>
            <tr>
                <td>أردوينو أونو</td>
                <td>1</td>
                <td><img src="./images/1.jpg" alt="أردوينو أونو" style="max-height: 100px;"></td>
                <td>لوحة التحكم الأساسية</td>
            </tr>
            <tr>
                <td>درايفر المحركات L293D</td>
                <td>1</td>
                <td><img src="./images/AI0031.2-300x300.jpg" alt="درايفر المحركات" style="max-height: 100px;"></td>
                <td>لتحكم في 4 محركات</td>
            </tr>
            <!-- باقي الصفوف بنفس النمط -->
        </table>
    </section>

    <section>
        <h2>🔌 دائرة التوصيلات</h2>
        <div class="wiring-diagram">
            <img src="./images/f738f3a3-289e-4a0e-a267-ced5d8d162fd.jfif" alt="دائرة التوصيلات">
        </div>
    </section>

    <section>
        <h2>💻 البرمجة والإعداد</h2>
        <h3>المتطلبات المسبقة</h3>
        <ul>
            <li>تثبيت Arduino IDE</li>
            <li>تنزيل المكتبات المطلوبة</li>
        </ul>
        
        <h3>كود البرمجة</h3>
        <div class="code-block">
            <pre>#include &lt;AFMotor.h&gt;
#include &lt;NewPing.h&gt;
#include &lt;Servo.h&gt;

#define TRIGGER_PIN A1
#define ECHO_PIN A0
#define MAX_DISTANCE 100

NewPing sonar(TRIGGER_PIN, ECHO_PIN, MAX_DISTANCE);
Servo myservo;

void setup() {
  // كود الإعداد
}

void loop() {
  // الكود الرئيسي
}</pre>
        </div>
    </section>

    <section>
        <h2>📂 هيكل الملفات</h2>
        <div class="file-structure">
            <pre>Human-Follower-Robot/
├── Human_Follower_Robot.ino
├── README.md
├── images/
│   ├── 1.jpg
│   ├── AI0031.2-300x300.jpg
│   ├── hc-sr04-ultrasonic-wave-distance-sensor.jpg
│   └── ...
└── libraries/
    ├── AFMotor/
    ├── NewPing/
    └── Servo/</pre>
        </div>
    </section>

    <section>
        <h2>⚠️ استكشاف الأخطاء</h2>
        <table class="troubleshooting">
            <tr>
                <th>المشكلة</th>
                <th>الحل</th>
            </tr>
            <tr>
                <td>الروبوت لا يتحرك</td>
                <td>تأكد من توصيل المحركات بشكل صحيح</td>
            </tr>
            <tr>
                <td>الحساسات لا تعمل</td>
                <td>تحقق من توصيلات الطاقة والإشارة</td>
            </tr>
        </table>
    </section>

    <section>
        <h2>👨💻 حقوق البرمجة والتطوير</h2>
        <p>تم تطوير وبرمجة هذا المشروع بواسطة:</p>
        <div class="badges">
            <a href="https://github.com/Eng-Ayman-Twfaq" class="badge">GitHub: Eng-Ayman-Twfaq</a>
            <a href="mailto:ayman.tawfaq.developes@gmail.com" class="badge">Email</a>
            <a href="https://wa.me/967770883615" class="badge">WhatsApp</a>
        </div>
    </section>

    <section>
        <h2>🌟 دعم المشروع</h2>
        <p>إذا أعجبك المشروع:</p>
        <ol>
            <li>⭐ اضغط زر Star في أعلى الصفحة على GitHub</li>
            <li>👁️ متابعة حسابنا لمشاريع جديدة</li>
            <li>💬 مشاركة المشروع مع الأصدقاء</li>
        </ol>
    </section>

    <div class="footer">
        <p>🚀 تابعنا لمشاهدة مشاريعنا الجديدة</p>
        <a href="https://github.com/Eng-Ayman-Twfaq" class="badge">عرض الملف الشخصي على GitHub</a>
    </div>
</body>
</html>