روبوت تتبع الإنسان - مشروع أردوينو 🤖
images/433319f6-4cfd-435d-afbe-c8104b8f43f7.jfif

📝 نظرة عامة
روبوت ذكي قادر على تتبع الأشخاص تلقائياً باستخدام تقنيات الاستشعار عن بعد. يتميز هذا المشروع بدقة الحركة وسهولة التصنيع، مما يجعله مثالياً لمشاريع الروبوتات التعليمية.

✨ المميزات الرئيسية
نظام تتبع ذكي باستخدام حساسات متعددة

تحكم دقيق في الحركة بأربع محركات

مسح محيطي بزاوية 180 درجة

تصميم متوافق مع مكونات متوفرة بسهولة

📦 قائمة المكونات
المكون	الكمية	الصورة	ملاحظات
أردوينو أونو	1	images/1.jpg	لوحة التحكم الأساسية
درايفر المحركات L293D	1	images/AI0031.2-300x300.jpg	لتحكم في 4 محركات
حساس المسافة HC-SR04	1	images/hc-sr04-ultrasonic-wave-distance-sensor.jpg	لقياس المسافات
حساسات الأشعة تحت الحمراء	2	images/ir-sensor-module-imported-500x500-1000x1000.jpg	لكشف الاتجاهات
محركات DC مع عجلات	4	images/336.2.jpg	قطر العجلات 6-8 سم
محرك سيرفو SG90	1	images/R.png	لتحريك الحساس
بطارية 9V	1	images/s-l400.jpg	مع حامل بطارية
هيكل الروبوت	1	images/4wd-smart-motor-robot-car-chasis-500x500.jpg	يمكن استخدام أي هيكل متوفر
🔌 دائرة التوصيلات
images/f738f3a3-289e-4a0e-a267-ced5d8d162fd.jfif

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
تثبيت Arduino IDE

تنزيل المكتبات المطلوبة:

AFMotor Library

NewPing Library

Servo Library

خطوات التنفيذ
قم بتنزيل ملف المشروع من GitHub

افتح ملف Human_Follower_Robot.ino في Arduino IDE

قم برفع الكود على لوحة الأردوينو

تأكد من أن جميع التوصيلات صحيحة

شغل الروبوت باستخدام البطارية

arduino
// نموذج من الكود الأساسي
#include <AFMotor.h>
#include <NewPing.h>
#include <Servo.h>

// تعريف الثوابت والمتغيرات
#define TRIGGER_PIN A1
#define ECHO_PIN A0
#define MAX_DISTANCE 100

NewPing sonar(TRIGGER_PIN, ECHO_PIN, MAX_DISTANCE);
Servo myservo;
// ... باقي الكود
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
│   ├── arduino_uno.jpg
│   ├── hc-sr04.jpg
│   ├── ir_sensor.jpg
│   ├── l293d.jpg
│   ├── robot_chassis.jpg
│   ├── robot_final.jpg
│   ├── wiring_diagram.jpg
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
📞 الدعم والاتصال
لأي استفسارات أو مساعدة تقنية:

📧 البريد الإلكتروني: ayman.tawfaq.developes@gmail.com
📞 الهاتف: +967 770 883 615
🕒 ساعات الدعم: 9 صباحاً - 5 مساءً (بتوقيت اليمن)


## **👨💻 حقوق البرمجة والتطوير**
تم تطوير وبرمجة هذا المشروع بواسطة:

[![GitHub Profile](https://img.shields.io/badge/GitHub-Eng__Ayman__Twfaq-181717?style=for-the-badge&logo=github)](https://github.com/Eng-Ayman-Twfaq)  
[![Email](https://img.shields.io/badge/Email-ayman.tawfaq.developes@gmail.com-D14836?style=for-the-badge&logo=gmail)](mailto:ayman.tawfaq.developes@gmail.com)  
[![WhatsApp](https://img.shields.io/badge/WhatsApp-%2B967%20770%20883%20615-25D366?style=for-the-badge&logo=whatsapp)](https://wa.me/967770883615)

---

## **🌟 دعم المشروع**
إذا أعجبك المشروع، يمكنك دعمنا بـ:
1. ⭐ **ضغط زر Star** في أعلى الصفحة على GitHub
2. 👁️ **متابعة حسابنا** لمشاريع جديدة
3. 💬 **مشاركة المشروع** مع الأصدقاء

[![GitHub Stars](https://img.shields.io/github/stars/Eng-Ayman-Twfaq/Human-Follower-Robot?style=social)](https://github.com/Eng-Ayman-Twfaq/Human-Follower-Robot)  
[![GitHub Followers](https://img.shields.io/github/followers/Eng-Ayman-Twfaq?style=social)](https://github.com/Eng-Ayman-Twfaq)

---

## **🚀 مشاريع قادمة**
تابعنا على GitHub لمشاهدة مشاريعنا الجديدة:

[![Visit Profile](https://img.shields.io/badge/VIEW_PROFILE-181717?style=for-the-badge&logo=github)](https://github.com/Eng-Ayman-Twfaq)