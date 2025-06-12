# 🤖 Human Follower Robot - روبوت تتبع الإنسان (Arduino)

<p align="center">
  <img src="./images/433319f6-4cfd-435d-afbe-c8104b8f43f7.jfif" width="220" alt="Human Follower Robot"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Arduino-blue" alt="Arduino">
  <img src="https://img.shields.io/badge/License-MIT-green" alt="License">
  <img src="https://img.shields.io/github/stars/Eng-Ayman-Twfaq/Human-Follower-Robot?style=social" alt="Stars">
</p>

## 📝 نظرة عامة

مشروع **روبوت تتبع الإنسان** هو نظام ذكي يعتمد على تقنيات استشعار متعددة لتتبع الأشخاص تلقائيًا. يتميز بقدرات تتبع دقيقة وسلاسة في الحركة، مما يجعله مثاليًا للمشاريع التعليمية أو التجريبية في عالم الروبوتات والذكاء الاصطناعي المدمج.

---

## ✨ المميزات الرئيسية

- 🎯 نظام تتبع ذكي باستخدام حساسات الموجات فوق الصوتية وIR
- ⚙️ تحكم كامل ودقيق في أربع محركات حركة
- 🔍 مسح محيطي بزاوية 180 درجة باستخدام محرك سيرفو
- 💰 تصميم بسيط بمكونات متوفرة وسهل التركيب

---

## 📦 قائمة المكونات

| المكون                        | الكمية | الصورة                                                                 | ملاحظات                        |
|------------------------------|--------|------------------------------------------------------------------------|--------------------------------|
| أردوينو أونو                 | 1      | ![1.jpg](./images/1.jpg)                                              | لوحة التحكم الأساسية           |
| درايفر المحركات L293D       | 1      | ![L293D](./images/AI0031.2-300x300.jpg)                               | التحكم في 4 محركات             |
| حساس الموجات فوق الصوتية     | 1      | ![HC-SR04](./images/hc-sr04-ultrasonic-wave-distance-sensor.jpg)      | لقياس المسافات                 |
| حساسات الأشعة تحت الحمراء  | 2      | ![IR](./images/ir-sensor-module-imported-500x500-1000x1000.jpg)       | لتحديد اتجاه الحركة            |
| محركات DC مع عجلات          | 4      | ![Motors](./images/336.2.jpg)                                         | قطر العجلات 6-8 سم             |
| محرك سيرفو SG90             | 1      | ![Servo](./images/R.png)                                              | لتدوير حساس الموجات            |
| بطارية 9V + حامل            | 1      | ![Battery](./images/s-l400.jpg)                                       | مصدر طاقة متنقل                |
| هيكل الروبوت                | 1      | ![Chassis](./images/4wd-smart-motor-robot-car-chasis-500x500.jpg)     | أي هيكل متوافق متاح            |

---

## 🔌 دائرة التوصيلات

<p align="center">
  <img src="./images/f738f3a3-289e-4a0e-a267-ced5d8d162fd.jfif" width="400" alt="Wiring Diagram"/>
</p>

### التوصيلات التفصيلية:

#### حساس الموجات فوق الصوتية (HC-SR04)
- VCC → 5V  
- GND → GND  
- TRIG → A1  
- ECHO → A0  

#### حساسات IR:
- **الحساس الأيمن:** OUT → A2  
- **الحساس الأيسر:** OUT → A3  

#### المحركات:
- المحرك الأمامي الأيمن → M1  
- المحرك الأمامي الأيسر → M2  
- المحرك الخلفي الأيمن → M3  
- المحرك الخلفي الأيسر → M4  

#### محرك السيرفو:
- الإشارة → D10  
- VCC → 5V  
- GND → GND  

---

## 💻 البرمجة والإعداد

### المتطلبات المسبقة
- Arduino IDE
- تثبيت المكتبات التالية:
  - `AFMotor`
  - `NewPing`
  - `Servo`

### مثال برمجي أولي:

```cpp
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
قم بتركيب المكونات وتوصيل الأسلاك.

حمّل الكود إلى لوحة Arduino باستخدام Arduino IDE.

ضع الروبوت على الأرض.

تحرك أمامه على مسافة 30-50 سم.

سيتتبعك الروبوت تلقائيًا.

للإنهاء، ابتعد عن نطاق الاستشعار.

📂 هيكل الملفات

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
الروبوت لا يتحرك	تأكد من توصيل المحركات جيدًا
الحساسات لا تستجيب	افحص أسلاك الطاقة والإشارات
حركة غير دقيقة أو عشوائية	تحقق من شحن البطارية واستخدام هيكل متوازن

👨‍💻 المطور
<p align="center"> <img src="https://img.shields.io/badge/GitHub-Eng__Ayman__Twfaq-181717?style=for-the-badge&logo=github" alt="GitHub"/> <img src="https://img.shields.io/badge/Email-ayman.tawfaq.developes%2540gmail.com-D14836?style=for-the-badge&logo=gmail" alt="Email"/> <img src="https://img.shields.io/badge/WhatsApp-%252B967%2520770%2520883%2520615-25D366?style=for-the-badge&logo=whatsapp" alt="WhatsApp"/> </p>
🌟 دعم المشروع
<p align="center"> <img src="https://img.shields.io/github/stars/Eng-Ayman-Twfaq/Human-Follower-Robot?style=social" alt="Stars"/> <img src="https://img.shields.io/github/followers/Eng-Ayman-Twfaq?style=social" alt="Followers"/> </p>
إذا أعجبك المشروع:

⭐ اضغط "Star" لدعم المشروع

👁️ تابع المطور على GitHub

📢 شارك المشروع مع زملائك المهتمين بالروبوتات

🚀 مشاريع قادمة
تابعنا على GitHub لمزيد من المشاريع المستقبلية 👇


