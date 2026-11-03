# گزارش نصب PHP CLI و اجرای تست‌ها

> تاریخ: 2026-11-03

## 🎉 خلاصه

PHP 8.4.27 CLI نصب شد و تمام 245 فایل PHP در 52 موتور با موفقیت تست syntax شد.

## نصب PHP CLI

| شاخص | مقدار |
|------|------|
| PHP نسخه | 8.4.27 (CLI) |
| Extensionها | Core, mbstring, PDO, SQLite3, XML, DOM, SimpleXML, OpenSSL, hash, json, session |
| روش نصب | apt-get download + dpkg-deb -x (بدون root) |
| مسیر | `/usr/local/bin/php` → `/tmp/php-extract/usr/bin/php8.4` |

## نتایج تست

### Syntax Check (php -l)

| شاخص | مقدار |
|------|------|
| فایل‌های بررسی‌شده | 245 |
| خطاهای شناسایی‌شده | 26 |
| خطاهای رفع‌شده | **26** (100%) |
| خطاهای باقی‌مانده | **0** ✅ |

### تست‌های Runtime اجراشده

| موتور | تست | نتیجه |
|-------|------|--------|
| Cache | put/get/has/increment/remember/forget | ✅ PASS |
| Hash | make/check/info/needsRehash | ✅ PASS |
| Config | get/set/has (dot-notation) | ✅ PASS |
| Pipeline | send/through/then (onion order) | ✅ PASS |
| I18n | get/addLines (ترجمه فارسی) | ✅ PASS |

### نمونه تست‌های موفق

```
=== Cache ===
Get: value1
Has: YES
Increment: 11
After: 11
Remember: computed_value
After forget: NO
All Cache tests passed! ✅

=== Hash ===
Hash: $2y$12$DObCdataw5uzd...
Check: PASS
Wrong: FAIL
All Hash tests passed! ✅

=== Config ===
Get: Tavaan
Set: 1.0.0
Has: YES
All Config tests passed! ✅

=== Pipeline ===
Pipeline: HELLO! world
All Pipeline tests passed! ✅

=== I18n ===
Translate: به توان خوش آمدید
All I18n tests passed! ✅
```

## نوع خطاهای رفع‌شده

| نوع خطا | تعداد | توضیح |
|---------|-------|------|
| `\\n` literal | 12 | Stub method generation با `\\n` به جای newline |
| `\$this` | 8 | Escape backslash در generated code |
| `callable` type | 2 | PHP 8.4 callable را در property قبول نمی‌کند |
| Empty type `?` | 2 | نوع خالی بعد از حذف callable |
| Const با chr() | 1 | Constant expression با function call |
| Non-abstract method | 1 | Method بدون body در کلاس غیر abstract |
| `const string` با array | 1 | نوع string با مقدار array |
| Template string | 1 | Newline در single-quoted string |

## Stub Methods باقی‌مانده

| شاخص | مقدار |
|------|------|
| موتورها با stub | 49 |
| مجموع stub methods | 431 |
| موتورها بدون stub | 3 (Compat, CORS, Pipeline) |

**نکته:** Stub methods متدهایی هستند که `return null;` برمی‌گردانند و باید با منطق واقعی پر شوند. این متدها syntax صحیح دارند اما پیاده‌سازی ندارند.

---
*Generated on 2026-11-03*
