# 🇨🇳 بوت تعلم اللغة الصينية | Chinese Learning Bot

<div align="center">

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![Telegram](https://img.shields.io/badge/Telegram-Bot-blue?style=for-the-badge&logo=telegram)
![Flask](https://img.shields.io/badge/Flask-Web-green?style=for-the-badge&logo=flask)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

**منصة تعليمية شاملة لتعلم اللغة الصينية عبر تليجرام وواجهة ويب احترافية**

[🚀 نشر سريع](#-نشر-سريع) • [✨ المميزات](#-المميزات) • [📖 الدليل](#-دليل-الاستخدام) • [🤝 المساهمة](#-المساهمة)

</div>

---

## 📋 نظرة عامة

بوت تليجرام متقدم لتعلم اللغة الصينية مع واجهة ويب تفاعلية، يحتوي على:

- 📚 جميع مستويات HSK (1-6)
- 📖 القرآن الكريم بالصينية
- 🎯 قاموس ومحادثات وقصص
- 🎮 اختبارات وبطاقات تعليمية
- 🌐 واجهة ويب عصرية
- 🤖 جاهز للذكاء الاصطناعي

---

## ✨ المميزات

### 🎓 للمتعلمين
- ✅ **18 قسم تعليمي** متنوع ومنظم
- ✅ **جميع مستويات HSK** من المبتدئ للمحترف
- ✅ **القرآن الكريم** مترجم للصينية
- ✅ **قاموس شامل** مع الأمثلة
- ✅ **محادثات يومية** عملية
- ✅ **قصص تعليمية** ممتعة
- ✅ **اختبارات تفاعلية** لقياس التقدم
- ✅ **بطاقات تعليمية** للحفظ

### 🛠️ للمشرفين
- ✅ **لوحة تحكم كاملة** سهلة الاستخدام
- ✅ **إضافة محتوى** (نص، روابط، ملفات)
- ✅ **رفع ملفات** متعددة الأنواع
- ✅ **استعراض وحذف** المحتوى
- ✅ **إحصائيات مفصلة** عن الاستخدام

### 🌐 الواجهة الويب
- ✅ **تصميم عصري** وجذاب
- ✅ **بحث متقدم** في المحتوى
- ✅ **تصفية ذكية** حسب الفئات
- ✅ **إحصائيات حية** محدثة
- ✅ **متجاوب** مع جميع الأجهزة
- ✅ **سريع** وخفيف

---

## 🚀 نشر سريع

### على Render.com (مجاني - 5 دقائق)

1. **سجل في Render**: https://render.com
2. **اختر "New Web Service"**
3. **اربط هذا المستودع**: `rain-devv/btmajid`
4. **أضف المتغيرات البيئية**:
   ```
   TELEGRAM_TOKEN = توكن_البوت_من_BotFather
   ADMIN_USER_IDS = [معرفك_الرقمي]
   PORT = 10000
   ```
5. **اضغط "Create Web Service"**
6. **انتظر 2-3 دقائق** ✅

**🎉 تم! البوت الآن يعمل 24/7 مجاناً!**

📖 [دليل النشر المفصل](QUICK_DEPLOY.md)

---

## 📦 التثبيت المحلي

### المتطلبات
- Python 3.11+
- pip
- حساب تليجرام

### الخطوات

```bash
# 1. استنسخ المشروع
git clone https://github.com/rain-devv/btmajid.git
cd btmajid

# 2. ثبت المتطلبات
pip install -r requirements.txt

# 3. أنشئ ملف .env
cat > .env << EOF
TELEGRAM_TOKEN=توكن_البوت
ADMIN_USER_IDS=[معرفك]
