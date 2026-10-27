<div align="center">

# 💬 پیامرسان کوچک من — My Mini Messenger (M3)

**پیام‌رسان تحت وب تک‌فایلی، خودمیزبان (Self-Hosted)، بدون وابستگی خارجی و مبتنی بر معماری بدون لاگ (Zero-Log)**  
**Single-File, Zero-Dependency, Self-Hosted & Privacy-First Web Messenger in Pure PHP**

[![PHP 7.2+](https://img.shields.io/badge/PHP-7.2%2B%20%7C%208.x-777BB4?logo=php&logoColor=white)](#)
[![Database](https://img.shields.io/badge/Database-SQLite%20%7C%20MySQL%20%2F%20MariaDB-009687)](#)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero%20%28Single%20index.php%29-10b981)](#)
[![Offline & LAN Ready](https://img.shields.io/badge/Network-Internet%20%26%20Isolated%20LAN-0ea5e9)](#)

[**🇮🇷 مستندات فارسی**](#-معرفی-پیامرسان-کوچک-من-m3) • [**🇬🇧 English Documentation**](#-english-documentation) • [**📦 مخزن گیت‌هاب / GitHub**](https://github.com/mehdisayyadnahed/my-mini-messenger)

  <img src="/images/Screenshot_1.png" alt="Universal File Server Screenshot 1" width="340" />
  <img src="/images/Screenshot_2.png" alt="Universal File Server Screenshot 2" width="680" />

</div>

---

<div dir="rtl">

## 🇮🇷 معرفی پیامرسان کوچک من (M3)

**پیامرسان کوچک من (`My Mini Messenger` یا به‌اختصار `M3`)** یک سکوی ارتباطی کامل، سبک، امن و کاملاً مستقل است که تمام بخش‌های سمت سرور، رابط کاربری، استایل‌ها، آیکون‌ها، فونت فارسی (`Vazirmatn`)، تولید بارکد دوبعدی، سرویس‌ورکر (`PWA`) و موتور تماس و رمزنگاری آن در **تنها یک فایل (`index.php`)** تجمیع شده است.

این نرم‌افزار به گونه‌ای طراحی شده است که بدون نیاز به `Composer`، `Node.js`، `Docker` یا هرگونه CDN و سرویس اینترنتی بیرونی، ظرف چند ثانیه روی ساده‌ترین هاست‌های اشتراکی، سرورهای شخصی یا حتی **شبکه‌های محلی کاملاً ایزوله و بدون اینترنت (Air-Gapped LAN)** راه‌اندازی شود.

> 🤖 **توضیح درباره روند توسعه:** این نرم‌افزار با ایده‌پردازی، هدایت و نظارت **مهدی صیادناهد** و **با کمک هوش مصنوعی (AI-Assisted Development)** طراحی، پیاده‌سازی و بهینه‌سازی شده است.

---

## ✨ امکانات و ویژگی‌های کلیدی

### ۱. گفتگوها، گروه‌ها و کانال‌ها
- **گفتگوهای خصوصی (DM) و فضای «پیام‌های ذخیره‌شده» (`Saved Messages`)** برای یادداشت‌ها و فایل‌های شخصی.
- **گفتگوهای محرمانه سرتاسری (`Secret Chats`):** رمزنگاری سرتاسری در سمت مرورگر با کلیدهای `ECDH P-256` و الگوریتم `AES-256-GCM`، همراه با تایید اثر انگشت امنیتی (`Safety Fingerprint`) و عدم ذخیره متن خام روی سرور.
- **گروه‌ها و کانال‌ها (عمومی و خصوصی):** پشتیبانی از شناسه عمومی (`@handle`)، لینک دعوت اختصاصی، مدیریت دقیق دسترسی‌های مدیران، حالت ارسال آهسته (`Slow Mode`)، بی‌صدا کردن کل گروه و سنجاق چندگانه پیام‌ها (`Multi-Pin`).
- **کانال رسمی «اعلان‌های سیستم»:** گفتگوی یک‌طرفه سیستمی برای دریافت هشدارهای امنیتی نشست و اطلاعیه‌های مهم.
- **ابزارهای کامل پیام‌رسانی:** پاسخ (`Reply`)، ویرایش پیام (همراه با تاریخچه ویرایش و سیاست پنج‌سطحی نمایش/مخفی‌سازی نشان ویرایش)، بازارسال با نام یا بدون نام فرستنده، واکنش‌ها (`Reactions`)، نظرسنجی (`Polls`)، تقسیم خودکار پیام‌های بلند هنگام ارسال، همگام‌سازی پیش‌نویس‌ها (`Draft Sync`) و جستجوی سراسری با قابلیت «نمایش در گفتگو».
- **نشانگر زنده «در حال نوشتن...» (`Typing Indicator`):** نمایش آنی در گفتگوهای خصوصی، محرمانه و گروه‌ها (تا ۳ نام به‌همراه شمارش سایرین) با کنترل پنج‌سطحی حریم خصوصی.

### ۲. رسانه، اشتراک فایل و تماس زنده
- **بارگذاری قطعه‌ای (`Chunked Upload`):** ارسال پایدار فایل‌های حجیم بدون برخورد با محدودیت حجم تک‌درخواست وب‌سرور.
- **پخش‌کننده اختصاصی صوت و ویدیو:** مجهز به بافر اشتراکی هوشمند، نوار جابه‌جایی روان بدون تداخل با ژست‌های لمسی موبایل، و توقف/ادامه خودکار هنگام خروج از دید صفحه.
- **ضبط درجا برای پیام صوتی و ویدیونوت دایره‌ای (`Voice & Circular Video Note`)** مستقیماً در نوار نوشتن پیام.
- **رسانه پوشش‌دار دوکلیکی (`Covered / Spoiler Media`):** امکان ارسال تصاویر و ویدیوهای محوشده و کنترل بارگذاری خودکار رسانه‌ها توسط کاربر.
- **مدیریت «فایل‌های بارگذاری‌شده من»:** مشاهده سهمیه مصرفی و حذف مستقیم فایل‌های قبلی برای آزادسازی فضا.
- **تماس صوتی و تصویری زنده:** تماس تک‌به‌تک و گروهی/کانالی مبتنی بر `WebRTC` محلی (بدون نیاز به سرورهای STUN اینترنتی) به‌همراه رله پشتیبان داخلی و سیاست‌های کنترلی کیفیت صدا و تصویر.

### ۳. امنیت، حریم خصوصی و معماری بدون لاگ (`Zero-Log`)
- **سیاست سخت‌گیرانه بدون لاگ (`Zero-Log Policy`):** عدم ایجاد هرگونه فایل `.log` و عدم ذخیره‌سازی آدرس IP یا مشخصات مرورگر کاربران در نشست‌ها (تنها زمان ورود ثبت می‌شود).
- **سپر امنیتی و فایروال بدون لاگ:** مجهز به تله ضدربات به سبک `WP-Armour` (توکن پویا + فیلد مخفی یکتا برای هر نصب)، کپچای جمع عددی سبک، سپر بررسی ساختار ورودی و محدودکننده نرخ درخواست (`Rate Limiter`) به همراه چالش `Proof-of-Work (SHA-256)`.
- **تایید دومرحله‌ای (`2FA TOTP`) و کد بازیابی یک‌بارمصرف:** تولید کاملاً آفلاین بارکد دوبعدی (`QR Code`) برای نرم‌افزارهای Authenticator و ارائه کد بازیابی ۱۲ کاراکتری.
- **قفل صفحه پیام‌رسان (`Lock Screen`):** رمز مجزای قفل صفحه با قفل خودکار در صورت عدم فعالیت و مسدودسازی دسترسی به API و فایل‌ها در زمان قفل بودن نشست.
- **پیام‌های خودحذف‌شونده (`TTL / Self-Destruct`):** زمان‌سنج حذف خودکار «پس از ارسال» یا «پس از خوانده شدن» در سطح تک‌پیام، پیش‌فرض کاربر، گفتگو یا کل سامانه (همراه با جلوگیری از ذخیره و بازارسال).
- **رمزهای اضطراری (`Duress & Panic Mode`):**
  - **رمز جعلی تخریب حساب (`Account Duress Password`):** پاکسازی آنی حساب کاربری در شرایط اضطراری با وارد کردن رمز جایگزین در صفحه ورود یا قفل صفحه (بدون مطالبه کد دومرحله‌ای).
  - **رمز جعلی تخریب کل پیام‌رسان (`Panic Duress Password`):** پاکسازی کامل پایگاه داده و تمام فایل‌های پیام‌رسان توسط مدیر کل در شرایط بحرانی.
- **حالت روح (`Ghost Mode`) و حریم خصوصی پیشرفته:** مشاهده نامحسوس گروه‌ها/کانال‌ها توسط مدیر کل بدون ثبت در فهرست بازدیدکنندگان، مخفی‌سازی آخرین بازدید و وضعیت آنلاین، و امکان فعالیت بدون یوزرنیم عمومی.

### ۴. پنل مدیریت کل، پشتیبان‌گیری و حالت خودمختار
- **مدیریت جامع ظرفیت و سهمیه‌ها:** تعیین سقف کل کاربران، سقف تعداد گروه و کانال قابل ساخت توسط هر کاربر، ظرفیت اعضا، محدودیت کاراکترهای مجاز برای **نام نمایشی** و **یوزرنیم (`@username`)**، سهمیه فضای ذخیره‌سازی و سهمیه ترافیک دوره‌ای.
- **زمان استراحت (`Quiet / Idle Hours`) و منطقه زمانی:** تعطیلی موقت خودکار یا دستی ارسال پیام در ساعات مشخص شبانه‌روز (سراسری یا اختصاصی هر گروه) و تنظیم منطقه زمانی و ساعت سفارشی سامانه.
- **پشتیبان‌گیری استاندارد `.m3b` و پشتیبان شخصی `ZIP`:** تهیه نسخه پشتیبان کامل یا تفکیکی (پایگاه داده / فایل‌ها / کامل) با فرمت `.m3b` توسط مدیر کل و دریافت خروجی `ZIP` گفتگوهای مجاز توسط کاربر بدون ایجاد فایل موقت روی دیسک سرور.
- **حالت خودمختار دائمی (`Autonomous Mode`):** امکان واگذاری غیرقابل‌بازگشت نقش ادمین کل به سامانه، به‌گونه‌ای که پیام‌رسان بدون وجود مدیر کل به‌صورت خودکار به کار خود ادامه دهد.

---

## ⚙️ پیش‌نیازهای سرور

- **PHP نسخه `7.2` یا بالاتر** (کاملاً سازگار با PHP `7.4`، `8.0`، `8.2`، `8.3` و `8.4`).
- یکی از دو افزونه پایگاه داده در PHP:
  - `pdo_sqlite` (پیشنهادی برای راه‌اندازی سریع و بدون نیاز به ساخت پایگاه داده مجزا)، **یا**
  - `pdo_mysql` (برای اتصال به `MySQL` یا `MariaDB`).
- افزونه‌های استاندارد PHP: `json`، `mbstring` و `openssl` (در اکثر قریب‌به‌اتفاق نصب‌های استاندارد PHP و XAMPP به‌طور پیش‌فرض فعال هستند).
- دسترسی نوشتن (`Write Permission`) در پوشه کنار فایل `index.php` جهت ساخت خودکار پوشه `chat_data/`.

---

## 🚀 راهنمای نصب و راه‌اندازی

### روش اول: نصب روی هاست لینوکسی یا سرور وب (Apache / Nginx / LiteSpeed)
1. تنها فایل `index.php` را در پوشه دلخواه هاست خود (مثلاً `public_html/` یا یک زیرپوشه مانند `public_html/chat/`) بارگذاری کنید.
2. آدرس سایت را در مرورگر باز کنید؛ **نصب‌کننده گرافیکی هوشمند** به‌صورت خودکار نمایش داده می‌شود.
3. نوع پایگاه داده (`SQLite` یا `MySQL / MariaDB`)، نام فارسی و انگلیسی پیام‌رسان، و مشخصات حساب **ادمین کل** را وارد کرده و دکمه نصب را بزنید.
4. کد بازیابی نمایش‌داده‌شده در پایان نصب را در جای امنی یادداشت کنید و وارد پیام‌رسان شوید.

### روش دوم: راه‌اندازی در شبکه محلی ایزوله (بدون اینترنت) با XAMPP
این برنامه هیچ فایل یا ارتباط اینترنتی خارجی نیاز ندارد و برای شبکه‌های داخلی سازمان‌ها، کارگاه‌ها و محیط‌های آفلاین ایده‌آل است:
1. برنامه **XAMPP** را نصب کرده و سرویس **Apache** (و در صورت تمایل به استفاده از MySQL، سرویس **MySQL**) را `Start` کنید.
2. فایل `index.php` را در مسیر `C:\xampp\htdocs\m3\index.php` قرار دهید.
3. در مرورگر آدرس `http://localhost/m3/` (یا از سایر سیستم‌های شبکه آدرس IP سرور مانند `https://192.168.1.10/m3/`) را باز کرده و مراحل نصب یک‌کلیکی را تکمیل کنید:
   - در XAMPP پیش‌فرض، گزینه **MySQL** از همان ابتدا آماده است (میزبان: `127.0.0.1`، کاربر: `root`، گذرواژه: خالی؛ خود برنامه پایگاه داده را خودکار می‌سازد).
   - برای استفاده از **SQLite** در XAMPP، کافی است در فایل `php.ini` خط `extension=pdo_sqlite` فعال (بدون `;` در ابتدای خط) باشد.
4. **نکته مهم مرورگرها در شبکه محلی (`HTTPS`):**
   - بخش‌های متنی، ارسال فایل/تصویر/ویدیو، گروه‌ها، کانال‌ها و پنل مدیریت روی `http://IP` عادی در شبکه محلی کار می‌کنند.
   - اما مرورگرهای مدرن اجازه دسترسی به **میکروفون، دوربین** (برای تماس صوتی/تصویری، پیام صوتی و ویدیونوت) و موتور **`WebCrypto`** (برای گفتگوی محرمانه `Secret Chat`) را روی IP شبکه تنها در بستر **`https://`** صادر می‌کنند. از آنجا که XAMPP به‌طور پیش‌فرض ماژول SSL آپاچی (پورت `443` با گواهی Self-Signed آفلاین) را دارد، کافی است کاربران شبکه آدرس را با **`https://192.168.x.x/m3/`** باز کنند.

### روش سوم: اجرای سریع با وب‌سرور داخلی PHP (مناسب تست و توسعه)
</div>

```bash
PHP_CLI_SERVER_WORKERS=6 php -S 0.0.0.0:8080 index.php
```

<div dir="rtl">

> توجه: تنظیم متغیر محیطی `PHP_CLI_SERVER_WORKERS=6` برای وب‌سرور داخلی PHP ضروری است تا هم‌زمان با ارتباط `Long-Polling`، سایر درخواست‌های موازی بدون انتظار پردازش شوند.

---

## 🛡️ نکات مهم امنیتی و نگهداری

1. **محافظت از پوشه `chat_data/`:**
   - برنامه هنگام اجرا، فایل‌های حفاظتی `.htaccess` (برای Apache / LiteSpeed)، `web.config` (برای IIS) و نام تصادفی غیرقابل‌حدس برای فایل پایگاه داده SQLite را به‌طور خودکار در پوشه `chat_data/` ایجاد می‌کند.
   - **اگر از وب‌سرور Nginx استفاده می‌کنید** (که فایل `.htaccess` را نمی‌خواند)، حتماً بلوک زیر را در تنظیمات `server` مربوط به Nginx قرار دهید تا دسترسی مستقیم وب به پوشه `chat_data/` مسدود باشد:

</div>

```nginx
location ^~ /chat_data/ {
    deny all;
    return 403;
}
```

<div dir="rtl">

2. **تنظیمات پیشنهادی `php.ini` برای فایل‌های حجیم:**
   - هرچند بارگذاری فایل‌ها در M3 به‌صورت قطعه‌ای (`Chunked`) انجام می‌شود، داشتن مقادیر معقول مانند `post_max_size = 32M`، `upload_max_filesize = 32M` و `memory_limit = 256M` در `php.ini` عملکرد بهینه‌تری در پردازش فایل‌ها و پشتیبان‌گیری فراهم می‌کند.
3. **پشتیبان‌گیری منظم (`.m3b`):**
   - از طریق **پنل مدیریت ⟵ پشتیبان‌گیری** می‌توانید فایل پشتیبان یکپارچه با پسوند `.m3b` تهیه و در صورت انتقال سرور، مستقیماً از همان بخش بازیابی نمایید.
4. **نگهداری کد بازیابی و گذرواژه‌های اضطراری:**
   - به دلیل معماری رمزنگاری‌شده گذرواژه‌ها و نبود وابستگی به ایمیل یا پیامک اینترنتی، کد بازیابی یک‌بارمصرف ارائه‌شده هنگام ثبت‌نام را نزد خود نگه دارید. همچنین در صورت تعریف «رمز جعلی تخریب» (`Duress Password`)، دقت کنید که وارد کردن آن بلافاصله عملیات پاکسازی اضطراری را اجرا می‌کند.

---

## 👨‍💻 توسعه‌دهنده و مشارکت

- **توسعه و پشتیبانی:** [مهدی صیادناهد](https://mehdisayyadnahed.ir)
- **توسعه‌یافته با کمک هوش مصنوعی (AI-Assisted)**
- **ارسال دیدگاه، گزارش اشکال و پیشنهاد بهبود:** از بخش Issues و Pull Requests در مخزن گیت‌هاب استقبال می‌شود:  
  🔗 [https://github.com/mehdisayyadnahed/my-mini-messenger](https://github.com/mehdisayyadnahed/my-mini-messenger)

</div>

---
---

# 🇬🇧 English Documentation

## Overview

**My Mini Messenger (`M3`)** is a complete, lightweight, privacy-first, self-hosted web messenger packed entirely into **a single PHP file (`index.php`)**. Everything—backend API, database schema & migrations, responsive RTL/LTR UI, embedded `Vazirmatn` font, inline SVG icons, offline 2FA QR generator, WebAudio sound synthesizer, PWA manifest/Service Worker, and LAN-ready WebRTC + E2EE cryptography—lives inside that one file with **zero external dependencies**.

Whether you want to deploy a private family/team messenger on shared hosting in 30 seconds or run a completely offline communication hub on an **isolated, air-gapped local network (LAN)** using XAMPP, `M3` works out of the box without `Composer`, `Node.js`, `Docker`, or internet access.

> 🤖 **AI-Assisted Development Note:** This project was conceived, directed, and curated by **Mehdi Sayyadnahed**, and **developed with the assistance of Artificial Intelligence (AI)**.

---

## ✨ Key Features

### 1. Rich Messaging, Groups & Channels
- **Direct Messages (DMs) & Personal "Saved Messages"** cloud space.
- **End-to-End Encrypted Secret Chats (`ECDH P-256` + `AES-256-GCM`):** Client-side key generation and encryption with verifiable safety fingerprints—plaintext never touches the server.
- **Public & Private Groups and Channels:** Public `@handle` discovery, private invite links, granular admin role permissions, Slow Mode, group mute, and multi-message pinning.
- **Official System Notices Chat:** Dedicated one-way system channel for login notifications and administrative notices.
- **Modern Chat Capabilities:** Replies, message editing (with edit history and a 5-tier silent-edit badge governance model), normal & anonymous forwarding, emoji reactions, interactive polls, automatic long-message splitting, cross-session draft syncing (excluded on Secret Chats for privacy), global search with *"Show in Chat"*, and a 5-tier live **Typing Indicator** (`DM`, `Secret Chat`, and up to 3 active names in `Groups`).

### 2. Media, Chunked Files & Live Voice/Video Calls
- **Resilient Chunked File Uploads:** Smoothly upload large files across restrictive reverse proxies or shared hosts.
- **Custom Audio & Video Players:** Shared media buffer management, touch-friendly horizontal scrubbing without gesture conflicts, and automatic viewport pause/resume.
- **In-Place Voice Messages & Circular Video Notes** recorded directly from the composer bar.
- **Two-Click Covered (Spoiler) Media** and per-user auto-download preferences, plus a **"My Uploaded Files"** manager to inspect and free personal storage quota.
- **LAN-Ready Voice & Video Calls:** 1-on-1 and Group/Channel live calls powered by `WebRTC` (`iceServers: []`—zero external STUN dependency) with an integrated encrypted fallback relay and admin quality/duration governance.

### 3. Security, Privacy & Strict Zero-Log Architecture
- **Strict Zero-Log Policy:** Zero `.log` files on disk, zero IP/User-Agent session tracking (sessions record login timestamp only).
- **Zero-Log Firewall & Anti-Bot Shield:** Built-in `WP-Armour`–style dynamic JS token + unique per-installation honeypot trap, lightweight single-line sum captcha, payload shield, rate limiting, and `SHA-256` Proof-of-Work (including a pure-JS `SHA-256` fallback for non-HTTPS LAN environments).
- **Offline `2FA (TOTP)` & One-Time Recovery Codes:** Built-in SVG QR code generator for authenticator apps and 12-character recovery codes.
- **Top-Layer Messenger Lock Screen:** Optional lock password with inactivity auto-lock and server-enforced `HTTP 423` API/file protection while locked.
- **Self-Destructing Messages (`TTL`):** *Expire After Send* or *Burn After Read* timers at the message, user, chat, and global levels, with copy/save/forward protection.
- **Emergency Duress & Panic Modes:**
  - **Account Duress Password:** Entering a secondary duress password at login or unlock (bypassing 2FA prompts) immediately wipes the account.
  - **Messenger Panic Duress Password:** Allows the Super-Admin to trigger an instant, zero-trace wipe of the entire messenger database and uploaded files in emergencies.
- **Ghost Mode & Identity Privacy:** Invisible Super-Admin inspection (excluded from read/viewer lists), global or personal last-seen hiding, and optional `@username`-free accounts.

### 4. Super-Admin Panel, `.m3b` Backups & Autonomous Mode
- **Granular Quotas & Limits:** Configure total user caps, per-user created group/channel quotas, member limits, **allowed character length ranges for Display Names & `@Usernames`**, storage quotas, and rolling periodic bandwidth quotas.
- **Global & Per-Chat Quiet/Idle Hours**, custom messenger timezone, and custom server clock offset.
- **Multi-Mode `.m3b` Backups & Zero-Temp-Disk User `ZIP` Exports:** Full/Database/Files system backups (`.m3b`) and streaming PKZIP personal data exports.
- **Permanent Autonomous Mode:** Optional irreversible handover where the Super-Admin relinquishes privileges so the messenger operates autonomously under its configured rules.
- **Full Localization & PWA:** Instant `Persian (Jalali)` / `English (Gregorian)` switching, Dark/Light/Auto themes, mobile back-stack navigation, and installable PWA support.

---

## ⚙️ Server Requirements

- **PHP `7.2` or newer** (tested up to PHP `8.4`).
- **Database Extension:** `pdo_sqlite` (recommended for instant zero-config setup) **or** `pdo_mysql` (`MySQL` / `MariaDB`).
- **Standard PHP Extensions:** `json`, `mbstring`, `openssl`.
- Write permission on the directory containing `index.php` (to create and manage `chat_data/`).

---

## 🚀 Quick Start & Installation

### Option 1: Shared Hosting or Linux Server (Apache / Nginx / LiteSpeed)
1. Upload **`index.php`** to your web root or a subdirectory (e.g., `/var/www/html/chat/index.php`).
2. Visit the URL in your browser to launch the **Built-in Visual Installer**.
3. Choose **SQLite** or **MySQL/MariaDB**, set your Persian/English site titles, create the **Super-Admin** account, and save your 12-character recovery code.

### Option 2: Isolated / Offline LAN with XAMPP
`M3` requires **zero internet access** and runs cleanly on air-gapped local networks:
1. Install **XAMPP** and start **Apache** (and **MySQL** if using MariaDB/MySQL).
2. Copy `index.php` into `C:\xampp\htdocs\m3\index.php`.
3. Open `http://localhost/m3/` (or `https://<LAN-IP>/m3/` from other devices on the LAN) and complete the 1-step installer:
   - **MySQL** works out of the box in XAMPP (`Host: 127.0.0.1`, `User: root`, empty password—the installer creates the database automatically).
   - **SQLite** works as soon as `extension=pdo_sqlite` is enabled in XAMPP's `php.ini`.
4. **Browser `HTTPS` Note on LAN IPs:**
   - Standard messaging, groups, channels, file uploads, and admin tools work over plain `http://<LAN-IP>`.
   - Modern browsers restrict **microphone/camera access** (voice notes, video notes, live calls) and **`WebCrypto`** (`Secret Chats`) on non-localhost IPs to **`https://`**. XAMPP includes Apache SSL (port `443` with an offline self-signed certificate) out of the box—simply open **`https://<LAN-IP>/m3/`** on LAN clients (no internet required).

### Option 3: PHP Built-in Server (Quick Local Testing)
```bash
PHP_CLI_SERVER_WORKERS=6 php -S 0.0.0.0:8080 index.php
```

---

## 🛡️ Security & Deployment Tips

- **Protect `chat_data/` on Nginx:** `M3` automatically generates `.htaccess` (Apache/LiteSpeed), `web.config` (IIS), and a randomized unguessable SQLite filename inside `chat_data/`. Because Nginx ignores `.htaccess`, add this rule to your Nginx `server` block:
  ```nginx
  location ^~ /chat_data/ {
      deny all;
      return 403;
  }
  ```
- **Backups:** Regularly export a full `.m3b` archive from **Admin Panel → Backup & Restore**.
- **Recovery Codes:** Since `M3` does not rely on external email/SMS gateways, store your one-time recovery code safely upon registration.

---

## 👨‍💻 Author & Contributing

- **Developed & Maintained by:** [Mehdi Sayyadnahed](https://mehdisayyadnahed.ir)
- **Developed with the assistance of Artificial Intelligence (AI)**
- **Contributions, Issues & Feature Requests:** Welcome at [github.com/mehdisayyadnahed/my-mini-messenger](https://github.com/mehdisayyadnahed/my-mini-messenger)
