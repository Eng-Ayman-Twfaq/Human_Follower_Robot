🤖 روبوت تتبع الإنسان - مشروع أردوينو
https://./images/433319f6-4cfd-435d-afbe-c8104b8f43f7.jfif

📝 نظرة عامة
روبوت ذكي قادر على تتبع الأشخاص تلقائياً باستخدام تقنيات الاستشعار عن بعد. يتميز هذا المشروع بدقة الحركة وسهولة التصنيع، مما يجعله مثالياً لمشاريع الروبوتات التعليمية.

✨ المميزات الرئيسية
🎯 نظام تتبع ذكي باستخدام حساسات متعددة

⚙️ تحكم دقيق في الحركة بأربع محركات

🔍 مسح محيطي بزاوية 180 درجة

💰 تصميم متوافق مع مكونات متوفرة بسهولة

📦 قائمة المكونات
المكون	الكمية	الصورة	ملاحظات
أردوينو أونو	1	https://./images/1.jpg	لوحة التحكم الأساسية
درايفر المحركات L293D	1	https://./images/AI0031.2-300x300.jpg	لتحكم في 4 محركات
حساس المسافة HC-SR04	1	https://./images/hc-sr04-ultrasonic-wave-distance-sensor.jpg	لقياس المسافات
حساسات الأشعة تحت الحمراء	2	https://./images/ir-sensor-module-imported-500x500-1000x1000.jpg	لكشف الاتجاهات
محركات DC مع عجلات	4	https://./images/336.2.jpg	قطر العجلات 6-8 سم
محرك سيرفو SG90	1	https://./images/R.png	لتحريك الحساس
بطارية 9V	1	https://./images/s-l400.jpg	مع حامل بطارية
هيكل الروبوت	1	https://./images/4wd-smart-motor-robot-car-chasis-500x500.jpg	يمكن استخدام أي هيكل متوفر
🔌 دائرة التوصيلات
https://./images/f738f3a3-289e-4a0e-a267-ced5d8d162fd.jfif

التوصيلات التفصيلية:
حساس الموجات فوق الصوتية (HC-SR04)

VCC → 5V

GND → GND

TRIG → A1

ECHO → A0

حساسات IR

الحساس الأيمن:

VCC → 5V

GND → GND

OUT → A2

الحساس الأيسر:

VCC → 5V

GND → GND

OUT → A3

المحركات

المحرك الأمامي الأيمن → M1

المحرك الأمامي الأيسر → M2

المحرك الخلفي الأيمن → M3

المحرك الخلفي الأيسر → M4

محرك السيرفو

الإشارة → D10

VCC → 5V

GND → GND

💻 البرمجة والإعداد
المتطلبات المسبقة
Arduino IDE

المكتبات المطلوبة:

AFMotor Library

NewPing Library

Servo Library

خطوات التنفيذ
arduino
#include <AFMotor.h>
#include <NewPing.h>
#include <Servo.h>

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
}
🎯 طريقة التشغيل
قم بتشغيل الروبوت

تحرك أمام الروبوت على مسافة 30-50 سم

سيبدأ الروبوت في تتبعك تلقائياً

لوقف الروبوت، ابتعد عن نطاق الحساسات

📂 هيكل الملفات
text
Human-Follower-Robot/
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
    └── Servo/
⚠️ استكشاف الأخطاء
المشكلة	الحل
الروبوت لا يتحرك	تأكد من توصيل المحركات بشكل صحيح
الحساسات لا تعمل	تحقق من توصيلات الطاقة والإشارة
حركة غير منتظمة	تأكد من شحن البطارية بالكامل
👨💻 حقوق البرمجة والتطوير
تم تطوير وبرمجة هذا المشروع بواسطة:

https://img.shields.io/badge/GitHub-Eng__Ayman__Twfaq-181717?style=for-the-badge&logo=github
https://img.shields.io/badge/Email-ayman.tawfaq.developes%2540gmail.com-D14836?style=for-the-badge&logo=gmail
https://img.shields.io/badge/WhatsApp-%252B967%2520770%2520883%2520615-25D366?style=for-the-badge&logo=whatsapp

🌟 دعم المشروع
https://img.shields.io/github/stars/Eng-Ayman-Twfaq/Human-Follower-Robot?style=social
https://img.shields.io/github/followers/Eng-Ayman-Twfaq?style=social

إذا أعجبك المشروع:

⭐ اضغط زر Star في أعلى الصفحة

👁️ تابع حسابنا على GitHub

💬 شارك المشروع مع الأصدقاء

🚀 مشاريع قادمة
تابعنا لمشاهدة مشاريعنا الجديدة:

https://img.shields.io/badge/VIEW_MORE_PROJECTS-181717?style=for-the-badge&logo=github