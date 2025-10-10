# 🚀 دليل نشر البوت على تليجرام

## ✅ البوت جاهز ويعمل!

تم اختبار البوت محلياً وهو يعمل بشكل ممتاز! ✨

---

## 📋 المعلومات الحالية

- **التوكن**: `8085016643:AAEHAO1BlQzhdo39N7MSkx3NEZK3P0d5M58`
- **المشرفين**: 
  - المعرف 1: `953696547`
  - المعرف 2: `7942066919` (tohelx)

⚠️ **تنبيه أمني**: يُنصح بتغيير التوكن لأنه تم كشفه علناً!

---

## 🎯 خيارات النشر

### الخيار 1: Render.com (موصى به) ⭐

#### المميزات:
- ✅ مجاني 100%
- ✅ سهل جداً
- ✅ يعمل 24/7
- ✅ دعم متغيرات البيئة
- ✅ نشر تلقائي من GitHub

#### الخطوات:

1. **سجل في Render**
   - اذهب إلى: https://render.com
   - سجل حساب جديد (مجاني)

2. **اربط GitHub**
   - في لوحة التحكم، اضغط "New +"
   - اختر "Web Service"
   - اختر "Connect GitHub"
   - اختر repository: `0onepro/majid`
   - اختر branch: `branch-3` (أو main)

3. **إعدادات الخدمة**
   ```
   Name: chinese-learning-bot
   Region: اختر الأقرب لك
   Branch: branch-3
   Root Directory: (اتركه فارغ)
   Runtime: Python 3
   Build Command: pip install -r requirements.txt
   Start Command: bash start.sh
   ```

4. **المتغيرات البيئية**
   اضغط "Advanced" ثم "Add Environment Variable":
   
   ```
   TELEGRAM_TOKEN = 8085016643:AAEHAO1BlQzhdo39N7MSkx3NEZK3P0d5M58
   ADMIN_USER_IDS = [953696547, 7942066919]
   PORT = 10000
   ```

5. **اختر الخطة**
   - اختر "Free" (مجاني)
   - اضغط "Create Web Service"

6. **انتظر النشر**
   - سيستغرق 2-3 دقائق
   - عند الانتهاء، سيظهر "Live" باللون الأخضر

7. **اختبر البوت**
   - افتح تليجرام
   - ابحث عن البوت
   - أرسل `/start`
   - يجب أن يرد عليك فوراً!

---

### الخيار 2: Railway.app (بديل ممتاز)

#### الخطوات:

1. سجل في https://railway.app
2. "New Project" → "Deploy from GitHub"
3. اختر `0onepro/majid`
4. أضف المتغيرات البيئية:
   ```
   TELEGRAM_TOKEN = 8085016643:AAEHAO1BlQzhdo39N7MSkx3NEZK3P0d5M58
   ADMIN_USER_IDS = [953696547, 7942066919]
   ```
5. Railway سيكتشف Python تلقائياً
6. انتظر النشر

---

### الخيار 3: Heroku (كلاسيكي)

⚠️ **ملاحظة**: Heroku لم يعد مجانياً بالكامل، لكن يمكن استخدامه

#### الخطوات:

1. سجل في https://heroku.com
2. ثبت Heroku CLI
3. في terminal:
   ```bash
   heroku login
   heroku create chinese-learning-bot
   heroku config:set TELEGRAM_TOKEN="8085016643:AAEHAO1BlQzhdo39N7MSkx3NEZK3P0d5M58"
   heroku config:set ADMIN_USER_IDS="[953696547, 7942066919]"
   git push heroku branch-3:main
   ```

---

### الخيار 4: PythonAnywhere (للمبتدئين)

1. سجل في https://www.pythonanywhere.com
2. افتح Bash console
3. استنسخ المشروع:
   ```bash
   git clone https://github.com/0onepro/majid.git
   cd majid
   pip3 install -r requirements.txt
   ```
4. أنشئ ملف `.env`:
   ```bash
   nano .env
   ```
   أضف:
   ```
   TELEGRAM_TOKEN=8085016643:AAEHAO1BlQzhdo39N7MSkx3NEZK3P0d5M58
   ADMIN_USER_IDS=[953696547, 7942066919]
   ```
5. شغّل البوت:
   ```bash
   python bot.py
   ```

⚠️ **عيب**: سيتوقف عند إغلاق المتصفح (يحتاج Always-On بـ $5/شهر)

---

### الخيار 5: VPS خاص (للمحترفين)

إذا كان لديك VPS (مثل DigitalOcean، Linode):

```bash
# على السيرفر
git clone https://github.com/0onepro/majid.git
cd majid
pip3 install -r requirements.txt

# إنشاء .env
nano .env
# أضف المتغيرات

# تشغيل دائم مع systemd
sudo nano /etc/systemd/system/chinese-bot.service
```

محتوى الملف:
```ini
[Unit]
Description=Chinese Learning Bot
After=network.target

[Service]
Type=simple
User=ubuntu
WorkingDirectory=/home/ubuntu/majid
ExecStart=/usr/bin/python3 bot.py
Restart=always

[Install]
WantedBy=multi-user.target
```

ثم:
```bash
sudo systemctl enable chinese-bot
sudo systemctl start chinese-bot
sudo systemctl status chinese-bot
```

---

## 🔍 التحقق من عمل البوت

بعد النشر، تحقق من:

1. **السجلات (Logs)**
   - في Render: اذهب إلى "Logs"
   - يجب أن ترى: `Bot is running...`

2. **اختبار على تليجرام**
   - ابحث عن البوت
   - أرسل `/start`
   - يجب أن يرد خلال ثانية

3. **اختبار الأوامر**
   - `/help` - قائمة المساعدة
   - اختر قسم من القائمة
   - جرب إضافة محتوى (للمشرفين)

---

## 🐛 حل المشاكل

### البوت لا يرد:
1. تحقق من السجلات (Logs)
2. تأكد من صحة التوكن
3. تأكد من تشغيل الخدمة

### خطأ في التوكن:
```
telegram.error.InvalidToken
```
- تحقق من المتغير البيئي `TELEGRAM_TOKEN`
- تأكد من عدم وجود مسافات زائدة

### خطأ في الأذونات:
- تأكد من `ADMIN_USER_IDS` بالصيغة الصحيحة: `[123, 456]`

### البوت يتوقف بعد فترة:
- استخدم Render أو Railway (لا يتوقفون)
- أو فعّل "Always On" في PythonAnywhere

---

## 📊 مراقبة البوت

### Render:
- الدخول إلى Dashboard
- اختر الخدمة
- اضغط "Logs" لرؤية السجلات
- اضغط "Metrics" للإحصائيات

### Railway:
- افتح المشروع
- اضغط على الخدمة
- "View Logs"

---

## 🔄 تحديث البوت

عند إضافة ميزات جديدة:

1. **ادفع التحديثات إلى GitHub**:
   ```bash
   git add .
   git commit -m "Add new features"
   git push origin branch-3
   ```

2. **في Render**:
   - سيتم النشر تلقائياً!
   - أو اضغط "Manual Deploy"

3. **في Railway**:
   - نشر تلقائي أيضاً

---

## 🎯 الخطوات التالية

بعد نشر البوت:

1. ✅ اختبر جميع الأوامر
2. ✅ أضف محتوى تعليمي
3. ✅ شارك البوت مع الأصدقاء
4. ✅ راقب الأداء
5. ✅ طبّق التطويرات المقترحة

---

## 💡 نصائح مهمة

1. **احفظ التوكن بأمان**
   - لا تشاركه علناً
   - استخدم متغيرات البيئة دائماً

2. **راقب السجلات**
   - تحقق من الأخطاء يومياً
   - استخدم الإشعارات

3. **احتفظ بنسخة احتياطية**
   - احفظ `data.json` بانتظام
   - استخدم Git للكود

4. **حدّث المكتبات**
   ```bash
   pip install --upgrade python-telegram-bot
   ```

---

## 📞 الدعم

إذا واجهت أي مشكلة:

1. راجع السجلات (Logs)
2. ابحث في [Telegram Bot API Docs](https://core.telegram.org/bots/api)
3. اسأل في [Stack Overflow](https://stackoverflow.com/questions/tagged/telegram-bot)

---

## 🎉 مبروك!

البوت الآن جاهز للعمل 24/7! 🚀

**رابط الموقع**: https://vgh0i1c19ez7.manus.space  
**البوت على تليجرام**: [أضف الرابط بعد النشر]

---

**تاريخ التحديث**: 10 أكتوبر 2025  
**الإصدار**: 2.0  
**الحالة**: ✅ جاهز للنشر
