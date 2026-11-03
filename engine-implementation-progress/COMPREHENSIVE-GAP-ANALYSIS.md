# تحلیل جامع نقص ۵۲ موتور — Comprehensive Gap Analysis

> تاریخ تولید: **2026-11-03 13:43:39 UTC**

## ۱. خلاصهٔ اجرایی

- **موتورهای بررسی‌شده:** 52
- **موتورهای کامل (✅):** 4
- **موتورهای ناقص متوسط (🟡):** 11
- **موتورهای ناقص بالا (🔴):** 37
- **مجموع نقص‌ها:** 263 (🔴 67 / 🟡 169 / 🟢 27)

## ۲. جدول کامل ۵۲ موتور

| # | موتور | DOC-ID | اولویت | LOC هدف | LOC واقعی | فایل‌های src | تست | config | نقص | 🔴 | 🟡 | 🟢 | وضعیت |
|---|-------|--------|--------|---------|----------|-------------|------|--------|------|-----|-----|-----|--------|
| 1 | api | DOC-044 | **P1** — فاز M6 | 1200 | 76 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |
| 2 | admin | DOC-078 | **P2** — فاز M8 | 2500 | 52 | 1 | 0 | 1 | 8 | 3 | 4 | 1 | 🔴 |
| 3 | audit | DOC-058 | **P1** — فاز M4 | 700 | 222 | 1 | 15 | 1 | 1 | 1 | 0 | 0 | 🔴 |
| 4 | auth | DOC-056 | **P0** — فاز M4 | 2000 | 108 | 1 | 0 | 1 | 10 | 1 | 8 | 1 | 🔴 |
| 5 | backup | DOC-068 | **P2** — فاز M5 | 700 | 67 | 1 | 0 | 1 | 3 | 2 | 0 | 1 | 🔴 |
| 6 | cors | DOC-046 | **P0** — فاز M2 | 350 | 140 | 1 | 12 | 1 | 0 | 0 | 0 | 0 | ✅ |
| 7 | cache | DOC-060 | **P0** — فاز M4 | 1400 | 597 | 8 | 34 | 1 | 5 | 0 | 5 | 0 | 🟡 |
| 8 | compat | DOC-083E | **P0** — فاز M1 (زیر | 400 | 923 | 11 | 23 | 1 | 0 | 0 | 0 | 0 | ✅ |
| 9 | config | DOC-032 | **P0** — فاز M1 | 600 | 789 | 10 | 54 | 1 | 2 | 0 | 2 | 0 | 🟡 |
| 10 | console | DOC-076 | **P1** — فاز M5 | 1600 | 511 | 6 | 33 | 1 | 2 | 1 | 1 | 0 | 🔴 |
| 11 | container | DOC-031 | **P0** — فاز M1 (اول | 1200 | 802 | 9 | 35 | 1 | 6 | 0 | 6 | 0 | 🟡 |
| 12 | cookie | DOC-042 | **P0** — فاز M2 | 400 | 94 | 1 | 3 | 1 | 2 | 1 | 0 | 1 | 🔴 |
| 13 | crypt | DOC-054 | **P0** — فاز M4 | 600 | 456 | 6 | 30 | 1 | 2 | 2 | 0 | 0 | 🔴 |
| 14 | database | DOC-047 | **P0** — فاز M3 | 3200 | 606 | 5 | 47 | 1 | 37 | 0 | 36 | 1 | 🟡 |
| 15 | error | DOC-035 | **P0** — فاز M1 | 800 | 534 | 9 | 37 | 1 | 4 | 1 | 3 | 0 | 🔴 |
| 16 | event | DOC-033 | **P0** — فاز M1 | 900 | 463 | 4 | 35 | 1 | 3 | 1 | 2 | 0 | 🔴 |
| 17 | feature-flag | DOC-075 | **P2** — فاز M6 | 600 | 37 | 1 | 0 | 1 | 3 | 2 | 0 | 1 | 🔴 |
| 18 | filesystem | DOC-063 | **P1** — فاز M5 | 1200 | 725 | 6 | 41 | 1 | 2 | 0 | 2 | 0 | 🟡 |
| 19 | hash | DOC-055 | **P0** — فاز M4 | 350 | 278 | 5 | 24 | 1 | 1 | 0 | 1 | 0 | 🟡 |
| 20 | http | DOC-039 | **P0** — فاز M2 | 2800 | 588 | 3 | 52 | 1 | 14 | 1 | 12 | 1 | 🔴 |
| 21 | http-client | DOC-064 | **P1** — فاز M5 | 1300 | 524 | 6 | 31 | 1 | 1 | 1 | 0 | 0 | 🔴 |
| 22 | i18n | DOC-069 | **P0** — فاز M2 | 900 | 407 | 5 | 30 | 1 | 2 | 1 | 1 | 0 | 🔴 |
| 23 | jalali | DOC-070 | **P0** — فاز M2 | 800 | 252 | 3 | 26 | 1 | 12 | 1 | 11 | 0 | 🔴 |
| 24 | log | DOC-036 | **P0** — فاز M1 | 900 | 732 | 12 | 29 | 1 | 5 | 1 | 4 | 0 | 🔴 |
| 25 | mail | DOC-065 | **P1** — فاز M5 | 1400 | 468 | 6 | 18 | 1 | 5 | 1 | 4 | 0 | 🔴 |
| 26 | media | DOC-074 | **P1** — فاز M5 | 1500 | 485 | 6 | 26 | 1 | 1 | 1 | 0 | 0 | 🔴 |
| 27 | migration | DOC-049 | **P0** — فاز M3 | 800 | 79 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |
| 28 | module | DOC-038 | **P0** — فاز M1 | 900 | 382 | 6 | 27 | 1 | 2 | 2 | 0 | 0 | 🔴 |
| 29 | notification | DOC-066 | **P1** — فاز M5 | 900 | 232 | 4 | 11 | 1 | 6 | 1 | 4 | 1 | 🔴 |
| 30 | orm | DOC-050 | **P0** — فاز M3 | 4000 | 569 | 4 | 46 | 1 | 17 | 0 | 16 | 1 | 🟡 |
| 31 | observability | DOC-067 | **P1** — فاز M6 | 1400 | 422 | 4 | 27 | 1 | 2 | 2 | 0 | 0 | 🔴 |
| 32 | optimizer | DOC-037 | **P1** — فاز M1 | 800 | 278 | 1 | 19 | 1 | 0 | 0 | 0 | 0 | ✅ |
| 33 | payment | DOC-073 | **P2** — فاز M7 | 1800 | 84 | 1 | 0 | 1 | 3 | 2 | 0 | 1 | 🔴 |
| 34 | pipeline | DOC-034 | **P0** — فاز M1 | 250 | 249 | 3 | 22 | 1 | 0 | 0 | 0 | 0 | ✅ |
| 35 | plugin | DOC-079 | **P1** — فاز M8 | 900 | 57 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |
| 36 | queue | DOC-061 | **P1** — فاز M5 | 2200 | 82 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |
| 37 | rbac | DOC-057 | **P0** — فاز M4 | 1600 | 54 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |
| 38 | realtime | DOC-045 | **P2** — فاز M6 | 1200 | 67 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |
| 39 | report | DOC-072 | **P2** — فاز M7 | 1600 | 75 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |
| 40 | router | DOC-040 | **P0** — فاز M2 | 1400 | 220 | 1 | 3 | 1 | 3 | 1 | 1 | 1 | 🔴 |
| 41 | scaffold | DOC-077 | **P1** — فاز M8 | 1200 | 66 | 1 | 0 | 1 | 3 | 2 | 0 | 1 | 🔴 |
| 42 | schedule | DOC-062 | **P1** — فاز M5 | 700 | 77 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |
| 43 | schema | DOC-048 | **P0** — فاز M3 | 1100 | 618 | 5 | 39 | 1 | 7 | 0 | 7 | 0 | 🟡 |
| 44 | search | DOC-052 | **P1** — فاز M6 | 1500 | 290 | 4 | 28 | 1 | 6 | 0 | 5 | 1 | 🟡 |
| 45 | security | DOC-059 | **P0** — فاز M4 | 1500 | 93 | 1 | 0 | 1 | 5 | 4 | 0 | 1 | 🔴 |
| 46 | session | DOC-041 | **P0** — فاز M2 | 900 | 43 | 1 | 0 | 1 | 12 | 1 | 10 | 1 | 🔴 |
| 47 | tenancy | DOC-082E | **P1** — فاز M6 | 1000 | 500 | 10 | 30 | 1 | 1 | 0 | 1 | 0 | 🟡 |
| 48 | test | DOC-084E | **P0** — فاز M8 (اما | 2500 | 703 | 11 | 49 | 1 | 9 | 1 | 7 | 1 | 🔴 |
| 49 | upgrade | DOC-081E | **P2** — فاز M8 | 600 | 228 | 1 | 20 | 1 | 1 | 1 | 0 | 0 | 🔴 |
| 50 | validation | DOC-051 | **P0** — فاز M3 | 2200 | 537 | 5 | 42 | 1 | 6 | 1 | 4 | 1 | 🔴 |
| 51 | view | DOC-043 | **P0** — فاز M2 | 1800 | 327 | 6 | 32 | 1 | 13 | 0 | 12 | 1 | 🟡 |
| 52 | workflow | DOC-071 | **P2** — فاز M7 | 2000 | 112 | 1 | 0 | 1 | 4 | 3 | 0 | 1 | 🔴 |

## ۳. موتورهای با نقص اولویت بالا 🔴

| # | موتور | DOC-ID | اولویت | نقص‌های 🔴 | شرح |
|---|-------|--------|--------|------------|------|
| 1 | `api` | DOC-044 | **P1** — فاز M6 | 3 | missing_class; missing_class; missing_tests |
| 2 | `admin` | DOC-078 | **P2** — فاز M8 | 3 | missing_class; missing_class; missing_tests |
| 3 | `audit` | DOC-058 | **P1** — فاز M4 | 1 | missing_class |
| 4 | `auth` | DOC-056 | **P0** — فاز M4 | 1 | missing_tests |
| 5 | `backup` | DOC-068 | **P2** — فاز M5 | 2 | missing_class; missing_tests |
| 6 | `console` | DOC-076 | **P1** — فاز M5 | 1 | missing_class |
| 7 | `cookie` | DOC-042 | **P0** — فاز M2 | 1 | missing_class |
| 8 | `crypt` | DOC-054 | **P0** — فاز M4 | 2 | missing_class; missing_class |
| 9 | `error` | DOC-035 | **P0** — فاز M1 | 1 | missing_class |
| 10 | `event` | DOC-033 | **P0** — فاز M1 | 1 | missing_class |
| 11 | `feature-flag` | DOC-075 | **P2** — فاز M6 | 2 | missing_class; missing_tests |
| 12 | `http` | DOC-039 | **P0** — فاز M2 | 1 | missing_class |
| 13 | `http-client` | DOC-064 | **P1** — فاز M5 | 1 | missing_class |
| 14 | `i18n` | DOC-069 | **P0** — فاز M2 | 1 | missing_class |
| 15 | `jalali` | DOC-070 | **P0** — فاز M2 | 1 | missing_class |
| 16 | `log` | DOC-036 | **P0** — فاز M1 | 1 | missing_migrations |
| 17 | `mail` | DOC-065 | **P1** — فاز M5 | 1 | missing_class |
| 18 | `media` | DOC-074 | **P1** — فاز M5 | 1 | missing_class |
| 19 | `migration` | DOC-049 | **P0** — فاز M3 | 3 | missing_class; missing_migrations; missing_tests |
| 20 | `module` | DOC-038 | **P0** — فاز M1 | 2 | missing_class; missing_class |
| 21 | `notification` | DOC-066 | **P1** — فاز M5 | 1 | missing_class |
| 22 | `observability` | DOC-067 | **P1** — فاز M6 | 2 | missing_class; missing_class |
| 23 | `payment` | DOC-073 | **P2** — فاز M7 | 2 | missing_class; missing_tests |
| 24 | `plugin` | DOC-079 | **P1** — فاز M8 | 3 | missing_class; missing_class; missing_tests |
| 25 | `queue` | DOC-061 | **P1** — فاز M5 | 3 | missing_class; missing_class; missing_tests |
| 26 | `rbac` | DOC-057 | **P0** — فاز M4 | 3 | missing_class; missing_class; missing_tests |
| 27 | `realtime` | DOC-045 | **P2** — فاز M6 | 3 | missing_class; missing_class; missing_tests |
| 28 | `report` | DOC-072 | **P2** — فاز M7 | 3 | missing_class; missing_class; missing_tests |
| 29 | `router` | DOC-040 | **P0** — فاز M2 | 1 | missing_class |
| 30 | `scaffold` | DOC-077 | **P1** — فاز M8 | 2 | missing_class; missing_tests |
| 31 | `schedule` | DOC-062 | **P1** — فاز M5 | 3 | missing_class; missing_class; missing_tests |
| 32 | `security` | DOC-059 | **P0** — فاز M4 | 4 | missing_class; missing_class; missing_class |
| 33 | `session` | DOC-041 | **P0** — فاز M2 | 1 | missing_tests |
| 34 | `test` | DOC-084E | **P0** — فاز M8 | 1 | missing_class |
| 35 | `upgrade` | DOC-081E | **P2** — فاز M8 | 1 | missing_class |
| 36 | `validation` | DOC-051 | **P0** — فاز M3 | 1 | missing_class |
| 37 | `workflow` | DOC-071 | **P2** — فاز M7 | 3 | missing_class; missing_class; missing_tests |

## ۴. جزئیات نقص هر موتور

### api (`DOC-044`)

- **Repository:** `Tavaan-Engine-API`
- **اولویت:** **P1** — فاز M6
- **LOC:** هدف 1200 | واقعی 76
- **فایل‌های src:** 1
- **تست:** 0 متد / 7 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `JsonResource` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `OpenApiGenerator` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |
| 3 | missing_tests | 🔴 | مستندات 7 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (76) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1200) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `JsonResource` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند.
   - ایجاد `src/JsonResource.php`
   - پیاده‌سازی متدها: make, collection, toArray, when, whenLoaded, whenCounted, mergeWhen, response
1. 🔴 **missing_class** — کلاس `OpenApiGenerator` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/OpenApiGenerator.php`
   - پیاده‌سازی متدها: generate, toYaml, toJson
1. 🔴 **missing_tests** — مستندات 7 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (76) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1200) است.

### admin (`DOC-078`)

- **Repository:** `Tavaan-Engine-Admin`
- **اولویت:** **P2** — فاز M8
- **LOC:** هدف 2500 | واقعی 52
- **فایل‌های src:** 1
- **تست:** 0 متد / 8 سناریو
- **نقص‌ها:** 8 (🔴 3 / 🟡 4 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `resource()` در کلاس `AdminManager` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `menu()` در کلاس `AdminManager` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `dashboard()` در کلاس `AdminManager` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `widget()` در کلاس `AdminManager` پیاده‌سازی نشده. |
| 5 | missing_class | 🔴 | کلاس `Resource` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند. |
| 6 | missing_class | 🔴 | کلاس `Form` در پیاده‌سازی یافت نشد. مستندات 10 متد عمومی تعریف می‌کند. |
| 7 | missing_tests | 🔴 | مستندات 8 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 8 | loc_shortfall | 🟢 | LOC پیاده‌سازی (52) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2500) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Resource` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند.
   - ایجاد `src/Resource.php`
   - پیاده‌سازی متدها: title, columns, searchable, filterable, sortable, form, actions, show
1. 🔴 **missing_class** — کلاس `Form` در پیاده‌سازی یافت نشد. مستندات 10 متد عمومی تعریف می‌کند.
   - ایجاد `src/Form.php`
   - پیاده‌سازی متدها: text, textarea, number, money, select, relation, media, richtext, jalaliDate, repeater
1. 🔴 **missing_tests** — مستندات 8 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟡 **missing_method** — متد `resource()` در کلاس `AdminManager` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `menu()` در کلاس `AdminManager` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `dashboard()` در کلاس `AdminManager` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `widget()` در کلاس `AdminManager` پیاده‌سازی نشده.
8. 🟢 **loc_shortfall** — LOC پیاده‌سازی (52) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2500) است.

### audit (`DOC-058`)

- **Repository:** `Tavaan-Engine-Audit`
- **اولویت:** **P1** — فاز M4
- **LOC:** هدف 700 | واقعی 222
- **فایل‌های src:** 1
- **تست:** 15 متد / 6 سناریو
- **نقص‌ها:** 1 (🔴 1 / 🟡 0 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Auditor` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Auditor` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند.
   - ایجاد `src/Auditor.php`
   - پیاده‌سازی متدها: record, verify, export, prune, lastHash

### auth (`DOC-056`)

- **Repository:** `Tavaan-Engine-Auth`
- **اولویت:** **P0** — فاز M4
- **LOC:** هدف 2000 | واقعی 108
- **فایل‌های src:** 1
- **تست:** 0 متد / 12 سناریو
- **نقص‌ها:** 10 (🔴 1 / 🟡 8 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `once()` در کلاس `AuthManager` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `validate()` در کلاس `AuthManager` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `token()` در کلاس `AuthManager` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `otp()` در کلاس `AuthManager` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `twoFactor()` در کلاس `AuthManager` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `devices()` در کلاس `AuthManager` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `sendPasswordResetLink()` در کلاس `AuthManager` پیاده‌سازی نشده. |
| 8 | missing_method | 🟡 | متد `resetPassword()` در کلاس `AuthManager` پیاده‌سازی نشده. |
| 9 | missing_tests | 🔴 | مستندات 12 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 10 | loc_shortfall | 🟢 | LOC پیاده‌سازی (108) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2000) است. |

**وظایف تکمیل:**

1. 🔴 **missing_tests** — مستندات 12 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
2. 🟡 **missing_method** — متد `once()` در کلاس `AuthManager` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `validate()` در کلاس `AuthManager` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `token()` در کلاس `AuthManager` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `otp()` در کلاس `AuthManager` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `twoFactor()` در کلاس `AuthManager` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `devices()` در کلاس `AuthManager` پیاده‌سازی نشده.
8. 🟡 **missing_method** — متد `sendPasswordResetLink()` در کلاس `AuthManager` پیاده‌سازی نشده.
9. 🟡 **missing_method** — متد `resetPassword()` در کلاس `AuthManager` پیاده‌سازی نشده.
10. 🟢 **loc_shortfall** — LOC پیاده‌سازی (108) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2000) است.

### backup (`DOC-068`)

- **Repository:** `Tavaan-Engine-Backup`
- **اولویت:** **P2** — فاز M5
- **LOC:** هدف 700 | واقعی 67
- **فایل‌های src:** 1
- **تست:** 0 متد / 7 سناریو
- **نقص‌ها:** 3 (🔴 2 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `BackupManager` در پیاده‌سازی یافت نشد. مستندات 7 متد عمومی تعریف می‌کند. |
| 2 | missing_tests | 🔴 | مستندات 7 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 3 | loc_shortfall | 🟢 | LOC پیاده‌سازی (67) به‌طور قابل‌توجهی کمتر از تخمین مستندات (700) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `BackupManager` در پیاده‌سازی یافت نشد. مستندات 7 متد عمومی تعریف می‌کند.
   - ایجاد `src/BackupManager.php`
   - پیاده‌سازی متدها: run, database, files, restore, list, verify, prune
1. 🔴 **missing_tests** — مستندات 7 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
3. 🟢 **loc_shortfall** — LOC پیاده‌سازی (67) به‌طور قابل‌توجهی کمتر از تخمین مستندات (700) است.

### cache (`DOC-060`)

- **Repository:** `Tavaan-Engine-Cache`
- **اولویت:** **P0** — فاز M4
- **LOC:** هدف 1400 | واقعی 597
- **فایل‌های src:** 8
- **تست:** 34 متد / 9 سناریو
- **نقص‌ها:** 5 (🔴 0 / 🟡 5 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `driver()` در کلاس `CacheManager` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `extend()` در کلاس `CacheManager` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `tags()` در کلاس `CacheManager` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `getDefaultDriver()` در کلاس `CacheManager` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `lock()` در کلاس `CacheRepository` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `driver()` در کلاس `CacheManager` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `extend()` در کلاس `CacheManager` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `tags()` در کلاس `CacheManager` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `getDefaultDriver()` در کلاس `CacheManager` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `lock()` در کلاس `CacheRepository` پیاده‌سازی نشده.

### config (`DOC-032`)

- **Repository:** `Tavaan-Engine-Config`
- **اولویت:** **P0** — فاز M1
- **LOC:** هدف 600 | واقعی 789
- **فایل‌های src:** 10
- **تست:** 54 متد / 12 سناریو
- **نقص‌ها:** 2 (🔴 0 / 🟡 2 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `masked()` در کلاس `Repository` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `has()` در کلاس `EnvRepository` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `masked()` در کلاس `Repository` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `has()` در کلاس `EnvRepository` پیاده‌سازی نشده.

### console (`DOC-076`)

- **Repository:** `Tavaan-Engine-Console`
- **اولویت:** **P1** — فاز M5
- **LOC:** هدف 1600 | واقعی 511
- **فایل‌های src:** 6
- **تست:** 33 متد / 7 سناریو
- **نقص‌ها:** 2 (🔴 1 / 🟡 1 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `progressStart()` در کلاس `Command` پیاده‌سازی نشده. |
| 2 | missing_class | 🔴 | کلاس `ConsoleKernel` در پیاده‌سازی یافت نشد. مستندات 4 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `ConsoleKernel` در پیاده‌سازی یافت نشد. مستندات 4 متد عمومی تعریف می‌کند.
   - ایجاد `src/ConsoleKernel.php`
   - پیاده‌سازی متدها: handle, call, register, commands
2. 🟡 **missing_method** — متد `progressStart()` در کلاس `Command` پیاده‌سازی نشده.

### container (`DOC-031`)

- **Repository:** `Tavaan-Engine-Container`
- **اولویت:** **P0** — فاز M1 (اولین موتور)
- **LOC:** هدف 1200 | واقعی 802
- **فایل‌های src:** 9
- **تست:** 35 متد / 15 سناریو
- **نقص‌ها:** 6 (🔴 0 / 🟡 6 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `has()` در کلاس `Container` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `lazy()` در کلاس `Container` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `flushScoped()` در کلاس `Container` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `forgetInstance()` در کلاس `Container` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `dependencyGraph()` در کلاس `Container` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `stats()` در کلاس `Container` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `has()` در کلاس `Container` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `lazy()` در کلاس `Container` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `flushScoped()` در کلاس `Container` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `forgetInstance()` در کلاس `Container` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `dependencyGraph()` در کلاس `Container` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `stats()` در کلاس `Container` پیاده‌سازی نشده.

### cookie (`DOC-042`)

- **Repository:** `Tavaan-Engine-Cookie`
- **اولویت:** **P0** — فاز M2
- **LOC:** هدف 400 | واقعی 94
- **فایل‌های src:** 1
- **تست:** 3 متد / 6 سناریو
- **نقص‌ها:** 2 (🔴 1 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `CookieJar` در پیاده‌سازی یافت نشد. مستندات 7 متد عمومی تعریف می‌کند. |
| 2 | loc_shortfall | 🟢 | LOC پیاده‌سازی (94) به‌طور قابل‌توجهی کمتر از تخمین مستندات (400) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `CookieJar` در پیاده‌سازی یافت نشد. مستندات 7 متد عمومی تعریف می‌کند.
   - ایجاد `src/CookieJar.php`
   - پیاده‌سازی متدها: make, forever, queue, get, forget, hasQueued, queued
2. 🟢 **loc_shortfall** — LOC پیاده‌سازی (94) به‌طور قابل‌توجهی کمتر از تخمین مستندات (400) است.

### crypt (`DOC-054`)

- **Repository:** `Tavaan-Engine-Crypt`
- **اولویت:** **P0** — فاز M4
- **LOC:** هدف 600 | واقعی 456
- **فایل‌های src:** 6
- **تست:** 30 متد / 9 سناریو
- **نقص‌ها:** 2 (🔴 2 / 🟡 0 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Signer` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `BlindIndex` در پیاده‌سازی یافت نشد. مستندات 2 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Signer` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/Signer.php`
   - پیاده‌سازی متدها: sign, verify, generateKeyPair
1. 🔴 **missing_class** — کلاس `BlindIndex` در پیاده‌سازی یافت نشد. مستندات 2 متد عمومی تعریف می‌کند.
   - ایجاد `src/BlindIndex.php`
   - پیاده‌سازی متدها: compute, verify

### database (`DOC-047`)

- **Repository:** `Tavaan-Engine-Database`
- **اولویت:** **P0** — فاز M3
- **LOC:** هدف 3200 | واقعی 606
- **فایل‌های src:** 5
- **تست:** 47 متد / 15 سناریو
- **نقص‌ها:** 37 (🔴 0 / 🟡 36 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `selectRaw()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `rightJoin()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `crossJoin()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `whereBetween()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `whereExists()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `whereRaw()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `groupBy()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 8 | missing_method | 🟡 | متد `having()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 9 | missing_method | 🟡 | متد `forUpdate()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 10 | missing_method | 🟡 | متد `sharedLock()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 11 | missing_method | 🟡 | متد `union()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 12 | missing_method | 🟡 | متد `withCte()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 13 | missing_method | 🟡 | متد `getBindings()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 14 | missing_method | 🟡 | متد `cursor()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 15 | missing_method | 🟡 | متد `find()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 16 | missing_method | 🟡 | متد `value()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 17 | missing_method | 🟡 | متد `pluck()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 18 | missing_method | 🟡 | متد `sum()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 19 | missing_method | 🟡 | متد `avg()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 20 | missing_method | 🟡 | متد `min()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 21 | missing_method | 🟡 | متد `max()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 22 | missing_method | 🟡 | متد `insertGetId()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 23 | missing_method | 🟡 | متد `insertOrIgnore()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 24 | missing_method | 🟡 | متد `upsert()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 25 | missing_method | 🟡 | متد `increment()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 26 | missing_method | 🟡 | متد `decrement()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 27 | missing_method | 🟡 | متد `truncate()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 28 | missing_method | 🟡 | متد `paginate()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 29 | missing_method | 🟡 | متد `chunk()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 30 | missing_method | 🟡 | متد `lazy()` در کلاس `QueryBuilder` پیاده‌سازی نشده. |
| 31 | missing_method | 🟡 | متد `cursor()` در کلاس `Connection` پیاده‌سازی نشده. |
| 32 | missing_method | 🟡 | متد `affectingStatement()` در کلاس `Connection` پیاده‌سازی نشده. |
| 33 | missing_method | 🟡 | متد `lastInsertId()` در کلاس `Connection` پیاده‌سازی نشده. |
| 34 | missing_method | 🟡 | متد `transactionLevel()` در کلاس `Connection` پیاده‌سازی نشده. |
| 35 | missing_method | 🟡 | متد `pdo()` در کلاس `Connection` پیاده‌سازی نشده. |
| 36 | missing_method | 🟡 | متد `queryLog()` در کلاس `Connection` پیاده‌سازی نشده. |
| 37 | loc_shortfall | 🟢 | LOC پیاده‌سازی (606) به‌طور قابل‌توجهی کمتر از تخمین مستندات (3200) است. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `selectRaw()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `rightJoin()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `crossJoin()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `whereBetween()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `whereExists()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `whereRaw()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `groupBy()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
8. 🟡 **missing_method** — متد `having()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
9. 🟡 **missing_method** — متد `forUpdate()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
10. 🟡 **missing_method** — متد `sharedLock()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
11. 🟡 **missing_method** — متد `union()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
12. 🟡 **missing_method** — متد `withCte()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
13. 🟡 **missing_method** — متد `getBindings()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
14. 🟡 **missing_method** — متد `cursor()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
15. 🟡 **missing_method** — متد `find()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
16. 🟡 **missing_method** — متد `value()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
17. 🟡 **missing_method** — متد `pluck()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
18. 🟡 **missing_method** — متد `sum()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
19. 🟡 **missing_method** — متد `avg()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
20. 🟡 **missing_method** — متد `min()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
21. 🟡 **missing_method** — متد `max()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
22. 🟡 **missing_method** — متد `insertGetId()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
23. 🟡 **missing_method** — متد `insertOrIgnore()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
24. 🟡 **missing_method** — متد `upsert()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
25. 🟡 **missing_method** — متد `increment()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
26. 🟡 **missing_method** — متد `decrement()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
27. 🟡 **missing_method** — متد `truncate()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
28. 🟡 **missing_method** — متد `paginate()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
29. 🟡 **missing_method** — متد `chunk()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
30. 🟡 **missing_method** — متد `lazy()` در کلاس `QueryBuilder` پیاده‌سازی نشده.
31. 🟡 **missing_method** — متد `cursor()` در کلاس `Connection` پیاده‌سازی نشده.
32. 🟡 **missing_method** — متد `affectingStatement()` در کلاس `Connection` پیاده‌سازی نشده.
33. 🟡 **missing_method** — متد `lastInsertId()` در کلاس `Connection` پیاده‌سازی نشده.
34. 🟡 **missing_method** — متد `transactionLevel()` در کلاس `Connection` پیاده‌سازی نشده.
35. 🟡 **missing_method** — متد `pdo()` در کلاس `Connection` پیاده‌سازی نشده.
36. 🟡 **missing_method** — متد `queryLog()` در کلاس `Connection` پیاده‌سازی نشده.
37. 🟢 **loc_shortfall** — LOC پیاده‌سازی (606) به‌طور قابل‌توجهی کمتر از تخمین مستندات (3200) است.

### error (`DOC-035`)

- **Repository:** `Tavaan-Engine-Error`
- **اولویت:** **P0** — فاز M1
- **LOC:** هدف 800 | واقعی 534
- **فایل‌های src:** 9
- **تست:** 37 متد / 0 سناریو
- **نقص‌ها:** 4 (🔴 1 / 🟡 3 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `ExceptionHandler` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند. |
| 2 | missing_method | 🟡 | متد `maskString()` در کلاس `LogMasker` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `addKeys()` در کلاس `LogMasker` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `addPatterns()` در کلاس `LogMasker` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `ExceptionHandler` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند.
   - ایجاد `src/ExceptionHandler.php`
   - پیاده‌سازی متدها: report, render, map, renderable, reportable, dontReport, level, context
2. 🟡 **missing_method** — متد `maskString()` در کلاس `LogMasker` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `addKeys()` در کلاس `LogMasker` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `addPatterns()` در کلاس `LogMasker` پیاده‌سازی نشده.

### event (`DOC-033`)

- **Repository:** `Tavaan-Engine-Event`
- **اولویت:** **P0** — فاز M1
- **LOC:** هدف 900 | واقعی 463
- **فایل‌های src:** 4
- **تست:** 35 متد / 15 سناریو
- **نقص‌ها:** 3 (🔴 1 / 🟡 2 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `push()` در کلاس `EventDispatcher` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `extend()` در کلاس `EventDispatcher` پیاده‌سازی نشده. |
| 3 | missing_class | 🔴 | کلاس `OutboxRelay` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `OutboxRelay` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/OutboxRelay.php`
   - پیاده‌سازی متدها: relay, retryDead, purge
2. 🟡 **missing_method** — متد `push()` در کلاس `EventDispatcher` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `extend()` در کلاس `EventDispatcher` پیاده‌سازی نشده.

### feature-flag (`DOC-075`)

- **Repository:** `Tavaan-Engine-Feature-Flag`
- **اولویت:** **P2** — فاز M6
- **LOC:** هدف 600 | واقعی 37
- **فایل‌های src:** 1
- **تست:** 0 متد / 6 سناریو
- **نقص‌ها:** 3 (🔴 2 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `FeatureManager` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند. |
| 2 | missing_tests | 🔴 | مستندات 6 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 3 | loc_shortfall | 🟢 | LOC پیاده‌سازی (37) به‌طور قابل‌توجهی کمتر از تخمین مستندات (600) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `FeatureManager` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند.
   - ایجاد `src/FeatureManager.php`
   - پیاده‌سازی متدها: enabled, for, value, define, kill, revive, experiment, percentage
1. 🔴 **missing_tests** — مستندات 6 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
3. 🟢 **loc_shortfall** — LOC پیاده‌سازی (37) به‌طور قابل‌توجهی کمتر از تخمین مستندات (600) است.

### filesystem (`DOC-063`)

- **Repository:** `Tavaan-Engine-Filesystem`
- **اولویت:** **P1** — فاز M5
- **LOC:** هدف 1200 | واقعی 725
- **فایل‌های src:** 6
- **تست:** 41 متد / 8 سناریو
- **نقص‌ها:** 2 (🔴 0 / 🟡 2 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `url()` در کلاس `FilesystemManager` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `temporaryUrl()` در کلاس `FilesystemManager` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `url()` در کلاس `FilesystemManager` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `temporaryUrl()` در کلاس `FilesystemManager` پیاده‌سازی نشده.

### hash (`DOC-055`)

- **Repository:** `Tavaan-Engine-Hash`
- **اولویت:** **P0** — فاز M4
- **LOC:** هدف 350 | واقعی 278
- **فایل‌های src:** 5
- **تست:** 24 متد / 5 سناریو
- **نقص‌ها:** 1 (🔴 0 / 🟡 1 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `driver()` در کلاس `HashManager` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `driver()` در کلاس `HashManager` پیاده‌سازی نشده.

### http (`DOC-039`)

- **Repository:** `Tavaan-Engine-Http`
- **اولویت:** **P0** — فاز M2
- **LOC:** هدف 2800 | واقعی 588
- **فایل‌های src:** 3
- **تست:** 52 متد / 18 سناریو
- **نقص‌ها:** 14 (🔴 1 / 🟡 12 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `sendAndTerminate()` در کلاس `HttpKernel` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `handleSubRequest()` در کلاس `HttpKernel` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `statusCode()` در کلاس `Response` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `withStatus()` در کلاس `Response` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `header()` در کلاس `Response` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `withHeader()` در کلاس `Response` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `withHeaders()` در کلاس `Response` پیاده‌سازی نشده. |
| 8 | missing_method | 🟡 | متد `body()` در کلاس `Response` پیاده‌سازی نشده. |
| 9 | missing_method | 🟡 | متد `withBody()` در کلاس `Response` پیاده‌سازی نشده. |
| 10 | missing_method | 🟡 | متد `withJson()` در کلاس `Response` پیاده‌سازی نشده. |
| 11 | missing_method | 🟡 | متد `cookie()` در کلاس `Response` پیاده‌سازی نشده. |
| 12 | missing_method | 🟡 | متد `isRedirect()` در کلاس `Response` پیاده‌سازی نشده. |
| 13 | missing_class | 🔴 | کلاس `ResponseFactory` در پیاده‌سازی یافت نشد. مستندات 11 متد عمومی تعریف می‌کند. |
| 14 | loc_shortfall | 🟢 | LOC پیاده‌سازی (588) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2800) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `ResponseFactory` در پیاده‌سازی یافت نشد. مستندات 11 متد عمومی تعریف می‌کند.
   - ایجاد `src/ResponseFactory.php`
   - پیاده‌سازی متدها: json, view, file, download, stream, streamDownload, noContent, make, redirectToRoute, redirectToUrl, problem
2. 🟡 **missing_method** — متد `sendAndTerminate()` در کلاس `HttpKernel` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `handleSubRequest()` در کلاس `HttpKernel` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `statusCode()` در کلاس `Response` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `withStatus()` در کلاس `Response` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `header()` در کلاس `Response` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `withHeader()` در کلاس `Response` پیاده‌سازی نشده.
8. 🟡 **missing_method** — متد `withHeaders()` در کلاس `Response` پیاده‌سازی نشده.
9. 🟡 **missing_method** — متد `body()` در کلاس `Response` پیاده‌سازی نشده.
10. 🟡 **missing_method** — متد `withBody()` در کلاس `Response` پیاده‌سازی نشده.
11. 🟡 **missing_method** — متد `withJson()` در کلاس `Response` پیاده‌سازی نشده.
12. 🟡 **missing_method** — متد `cookie()` در کلاس `Response` پیاده‌سازی نشده.
13. 🟡 **missing_method** — متد `isRedirect()` در کلاس `Response` پیاده‌سازی نشده.
14. 🟢 **loc_shortfall** — LOC پیاده‌سازی (588) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2800) است.

### http-client (`DOC-064`)

- **Repository:** `Tavaan-Engine-Http-Client`
- **اولویت:** **P1** — فاز M5
- **LOC:** هدف 1300 | واقعی 524
- **فایل‌های src:** 6
- **تست:** 31 متد / 9 سناریو
- **نقص‌ها:** 1 (🔴 1 / 🟡 0 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Factory` در پیاده‌سازی یافت نشد. مستندات 16 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Factory` در پیاده‌سازی یافت نشد. مستندات 16 متد عمومی تعریف می‌کند.
   - ایجاد `src/Factory.php`
   - پیاده‌سازی متدها: get, post, put, patch, delete, withHeaders, withToken, asJson, asForm, timeout, retry, pool, fake, assertSent, withQueryParameters, attach

### i18n (`DOC-069`)

- **Repository:** `Tavaan-Engine-I18n`
- **اولویت:** **P0** — فاز M2
- **LOC:** هدف 900 | واقعی 407
- **فایل‌های src:** 5
- **تست:** 30 متد / 9 سناریو
- **نقص‌ها:** 2 (🔴 1 / 🟡 1 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `namespace()` در کلاس `Translator` پیاده‌سازی نشده. |
| 2 | missing_class | 🔴 | کلاس `PersianFormatter` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `PersianFormatter` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند.
   - ایجاد `src/PersianFormatter.php`
   - پیاده‌سازی متدها: digits, number, currency, date, toLatinDigits
2. 🟡 **missing_method** — متد `namespace()` در کلاس `Translator` پیاده‌سازی نشده.

### jalali (`DOC-070`)

- **Repository:** `Tavaan-Engine-Jalali`
- **اولویت:** **P0** — فاز M2
- **LOC:** هدف 800 | واقعی 252
- **فایل‌های src:** 3
- **تست:** 26 متد / 10 سناریو
- **نقص‌ها:** 12 (🔴 1 / 🟡 11 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `now()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `fromGregorian()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `parse()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `toGregorian()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `addDays()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `subMonths()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `diffInDays()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 8 | missing_method | 🟡 | متد `isLeap()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 9 | missing_method | 🟡 | متد `dayName()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 10 | missing_method | 🟡 | متد `startOfMonth()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 11 | missing_method | 🟡 | متد `endOfMonth()` در کلاس `JalaliDate` پیاده‌سازی نشده. |
| 12 | missing_class | 🔴 | کلاس `Clock` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Clock` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/Clock.php`
   - پیاده‌سازی متدها: utcNow, now, jalaliNow
2. 🟡 **missing_method** — متد `now()` در کلاس `JalaliDate` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `fromGregorian()` در کلاس `JalaliDate` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `parse()` در کلاس `JalaliDate` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `toGregorian()` در کلاس `JalaliDate` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `addDays()` در کلاس `JalaliDate` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `subMonths()` در کلاس `JalaliDate` پیاده‌سازی نشده.
8. 🟡 **missing_method** — متد `diffInDays()` در کلاس `JalaliDate` پیاده‌سازی نشده.
9. 🟡 **missing_method** — متد `isLeap()` در کلاس `JalaliDate` پیاده‌سازی نشده.
10. 🟡 **missing_method** — متد `dayName()` در کلاس `JalaliDate` پیاده‌سازی نشده.
11. 🟡 **missing_method** — متد `startOfMonth()` در کلاس `JalaliDate` پیاده‌سازی نشده.
12. 🟡 **missing_method** — متد `endOfMonth()` در کلاس `JalaliDate` پیاده‌سازی نشده.

### log (`DOC-036`)

- **Repository:** `Tavaan-Engine-Log`
- **اولویت:** **P0** — فاز M1
- **LOC:** هدف 900 | واقعی 732
- **فایل‌های src:** 12
- **تست:** 29 متد / 13 سناریو
- **نقص‌ها:** 5 (🔴 1 / 🟡 4 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `stack()` در کلاس `LogManager` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `driver()` در کلاس `LogManager` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `extend()` در کلاس `LogManager` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `getChannels()` در کلاس `LogManager` پیاده‌سازی نشده. |
| 5 | missing_migrations | 🔴 | مستندات 1 جدول تعریف می‌کند اما migration موجود نیست. |

**وظایف تکمیل:**

1. 🔴 **missing_migrations** — مستندات 1 جدول تعریف می‌کند اما migration موجود نیست.
2. 🟡 **missing_method** — متد `stack()` در کلاس `LogManager` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `driver()` در کلاس `LogManager` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `extend()` در کلاس `LogManager` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `getChannels()` در کلاس `LogManager` پیاده‌سازی نشده.

### mail (`DOC-065`)

- **Repository:** `Tavaan-Engine-Mail`
- **اولویت:** **P1** — فاز M5
- **LOC:** هدف 1400 | واقعی 468
- **فایل‌های src:** 6
- **تست:** 18 متد / 7 سناریو
- **نقص‌ها:** 5 (🔴 1 / 🟡 4 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Mailer` در پیاده‌سازی یافت نشد. مستندات 9 متد عمومی تعریف می‌کند. |
| 2 | missing_method | 🟡 | متد `with()` در کلاس `Mailable` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `replyTo()` در کلاس `Mailable` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `send()` در کلاس `Mailable` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `queue()` در کلاس `Mailable` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Mailer` در پیاده‌سازی یافت نشد. مستندات 9 متد عمومی تعریف می‌کند.
   - ایجاد `src/Mailer.php`
   - پیاده‌سازی متدها: to, cc, bcc, send, queue, later, raw, fake, assertSent
2. 🟡 **missing_method** — متد `with()` در کلاس `Mailable` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `replyTo()` در کلاس `Mailable` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `send()` در کلاس `Mailable` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `queue()` در کلاس `Mailable` پیاده‌سازی نشده.

### media (`DOC-074`)

- **Repository:** `Tavaan-Engine-Media`
- **اولویت:** **P1** — فاز M5
- **LOC:** هدف 1500 | واقعی 485
- **فایل‌های src:** 6
- **تست:** 26 متد / 10 سناریو
- **نقص‌ها:** 1 (🔴 1 / 🟡 0 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `MediaManager` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `MediaManager` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/MediaManager.php`
   - پیاده‌سازی متدها: upload, fromPath, variants

### migration (`DOC-049`)

- **Repository:** `Tavaan-Engine-Migration`
- **اولویت:** **P0** — فاز M3
- **LOC:** هدف 800 | واقعی 79
- **فایل‌های src:** 1
- **تست:** 0 متد / 7 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Migrator` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند. |
| 2 | missing_migrations | 🔴 | مستندات 1 جدول تعریف می‌کند اما migration موجود نیست. |
| 3 | missing_tests | 🔴 | مستندات 7 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (79) به‌طور قابل‌توجهی کمتر از تخمین مستندات (800) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Migrator` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند.
   - ایجاد `src/Migrator.php`
   - پیاده‌سازی متدها: run, rollback, refresh, fresh, status, install
1. 🔴 **missing_migrations** — مستندات 1 جدول تعریف می‌کند اما migration موجود نیست.
1. 🔴 **missing_tests** — مستندات 7 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (79) به‌طور قابل‌توجهی کمتر از تخمین مستندات (800) است.

### module (`DOC-038`)

- **Repository:** `Tavaan-Engine-Module`
- **اولویت:** **P0** — فاز M1
- **LOC:** هدف 900 | واقعی 382
- **فایل‌های src:** 6
- **تست:** 27 متد / 7 سناریو
- **نقص‌ها:** 2 (🔴 2 / 🟡 0 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `ModuleManager` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `ModuleRunner` در پیاده‌سازی یافت نشد. مستندات 1 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `ModuleManager` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند.
   - ایجاد `src/ModuleManager.php`
   - پیاده‌سازی متدها: install, uninstall, enable, disable, update, validate
1. 🔴 **missing_class** — کلاس `ModuleRunner` در پیاده‌سازی یافت نشد. مستندات 1 متد عمومی تعریف می‌کند.
   - ایجاد `src/ModuleRunner.php`
   - پیاده‌سازی متدها: run

### notification (`DOC-066`)

- **Repository:** `Tavaan-Engine-Notification`
- **اولویت:** **P1** — فاز M5
- **LOC:** هدف 900 | واقعی 232
- **فایل‌های src:** 4
- **تست:** 11 متد / 7 سناریو
- **نقص‌ها:** 6 (🔴 1 / 🟡 4 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `NotificationSender` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |
| 2 | missing_method | 🟡 | متد `toMail()` در کلاس `Notification` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `toSms()` در کلاس `Notification` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `toDatabase()` در کلاس `Notification` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `toTelegram()` در کلاس `Notification` پیاده‌سازی نشده. |
| 6 | loc_shortfall | 🟢 | LOC پیاده‌سازی (232) به‌طور قابل‌توجهی کمتر از تخمین مستندات (900) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `NotificationSender` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/NotificationSender.php`
   - پیاده‌سازی متدها: send, sendNow, route
2. 🟡 **missing_method** — متد `toMail()` در کلاس `Notification` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `toSms()` در کلاس `Notification` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `toDatabase()` در کلاس `Notification` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `toTelegram()` در کلاس `Notification` پیاده‌سازی نشده.
6. 🟢 **loc_shortfall** — LOC پیاده‌سازی (232) به‌طور قابل‌توجهی کمتر از تخمین مستندات (900) است.

### orm (`DOC-050`)

- **Repository:** `Tavaan-Engine-ORM`
- **اولویت:** **P0** — فاز M3
- **LOC:** هدف 4000 | واقعی 569
- **فایل‌های src:** 4
- **تست:** 46 متد / 14 سناریو
- **نقص‌ها:** 17 (🔴 0 / 🟡 16 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `findOrFail()` در کلاس `Model` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `query()` در کلاس `Model` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `updateOrCreate()` در کلاس `Model` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `firstOrCreate()` در کلاس `Model` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `restore()` در کلاس `Model` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `update()` در کلاس `Model` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `refresh()` در کلاس `Model` پیاده‌سازی نشده. |
| 8 | missing_method | 🟡 | متد `toJson()` در کلاس `Model` پیاده‌سازی نشده. |
| 9 | missing_method | 🟡 | متد `with()` در کلاس `Model` پیاده‌سازی نشده. |
| 10 | missing_method | 🟡 | متد `withCount()` در کلاس `Model` پیاده‌سازی نشده. |
| 11 | missing_method | 🟡 | متد `load()` در کلاس `Model` پیاده‌سازی نشده. |
| 12 | missing_method | 🟡 | متد `observe()` در کلاس `Model` پیاده‌سازی نشده. |
| 13 | missing_method | 🟡 | متد `addGlobalScope()` در کلاس `Model` پیاده‌سازی نشده. |
| 14 | missing_method | 🟡 | متد `chunk()` در کلاس `Model` پیاده‌سازی نشده. |
| 15 | missing_method | 🟡 | متد `lazy()` در کلاس `Model` پیاده‌سازی نشده. |
| 16 | missing_method | 🟡 | متد `paginate()` در کلاس `Model` پیاده‌سازی نشده. |
| 17 | loc_shortfall | 🟢 | LOC پیاده‌سازی (569) به‌طور قابل‌توجهی کمتر از تخمین مستندات (4000) است. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `findOrFail()` در کلاس `Model` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `query()` در کلاس `Model` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `updateOrCreate()` در کلاس `Model` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `firstOrCreate()` در کلاس `Model` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `restore()` در کلاس `Model` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `update()` در کلاس `Model` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `refresh()` در کلاس `Model` پیاده‌سازی نشده.
8. 🟡 **missing_method** — متد `toJson()` در کلاس `Model` پیاده‌سازی نشده.
9. 🟡 **missing_method** — متد `with()` در کلاس `Model` پیاده‌سازی نشده.
10. 🟡 **missing_method** — متد `withCount()` در کلاس `Model` پیاده‌سازی نشده.
11. 🟡 **missing_method** — متد `load()` در کلاس `Model` پیاده‌سازی نشده.
12. 🟡 **missing_method** — متد `observe()` در کلاس `Model` پیاده‌سازی نشده.
13. 🟡 **missing_method** — متد `addGlobalScope()` در کلاس `Model` پیاده‌سازی نشده.
14. 🟡 **missing_method** — متد `chunk()` در کلاس `Model` پیاده‌سازی نشده.
15. 🟡 **missing_method** — متد `lazy()` در کلاس `Model` پیاده‌سازی نشده.
16. 🟡 **missing_method** — متد `paginate()` در کلاس `Model` پیاده‌سازی نشده.
17. 🟢 **loc_shortfall** — LOC پیاده‌سازی (569) به‌طور قابل‌توجهی کمتر از تخمین مستندات (4000) است.

### observability (`DOC-067`)

- **Repository:** `Tavaan-Engine-Observability`
- **اولویت:** **P1** — فاز M6
- **LOC:** هدف 1400 | واقعی 422
- **فایل‌های src:** 4
- **تست:** 27 متد / 7 سناریو
- **نقص‌ها:** 2 (🔴 2 / 🟡 0 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Tracer` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `Health` در پیاده‌سازی یافت نشد. مستندات 4 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Tracer` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/Tracer.php`
   - پیاده‌سازی متدها: startSpan, currentSpan, withSpan
1. 🔴 **missing_class** — کلاس `Health` در پیاده‌سازی یافت نشد. مستندات 4 متد عمومی تعریف می‌کند.
   - ایجاد `src/Health.php`
   - پیاده‌سازی متدها: add, check, live, ready

### payment (`DOC-073`)

- **Repository:** `Tavaan-Engine-Payment`
- **اولویت:** **P2** — فاز M7
- **LOC:** هدف 1800 | واقعی 84
- **فایل‌های src:** 1
- **تست:** 0 متد / 9 سناریو
- **نقص‌ها:** 3 (🔴 2 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `PaymentManager` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند. |
| 2 | missing_tests | 🔴 | مستندات 9 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 3 | loc_shortfall | 🟢 | LOC پیاده‌سازی (84) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1800) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `PaymentManager` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند.
   - ایجاد `src/PaymentManager.php`
   - پیاده‌سازی متدها: purchase, verify, refund, inquire, gateway
1. 🔴 **missing_tests** — مستندات 9 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
3. 🟢 **loc_shortfall** — LOC پیاده‌سازی (84) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1800) است.

### plugin (`DOC-079`)

- **Repository:** `Tavaan-Engine-Plugin`
- **اولویت:** **P1** — فاز M8
- **LOC:** هدف 900 | واقعی 57
- **فایل‌های src:** 1
- **تست:** 0 متد / 8 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `PluginManager` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `Hook` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |
| 3 | missing_tests | 🔴 | مستندات 8 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (57) به‌طور قابل‌توجهی کمتر از تخمین مستندات (900) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `PluginManager` در پیاده‌سازی یافت نشد. مستندات 8 متد عمومی تعریف می‌کند.
   - ایجاد `src/PluginManager.php`
   - پیاده‌سازی متدها: install, uninstall, enable, disable, update, list, verify, scan
1. 🔴 **missing_class** — کلاس `Hook` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/Hook.php`
   - پیاده‌سازی متدها: listen, fire, has
1. 🔴 **missing_tests** — مستندات 8 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (57) به‌طور قابل‌توجهی کمتر از تخمین مستندات (900) است.

### queue (`DOC-061`)

- **Repository:** `Tavaan-Engine-Queue`
- **اولویت:** **P1** — فاز M5
- **LOC:** هدف 2200 | واقعی 82
- **فایل‌های src:** 1
- **تست:** 0 متد / 12 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `QueueManager` در پیاده‌سازی یافت نشد. مستندات 7 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `Worker` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |
| 3 | missing_tests | 🔴 | مستندات 12 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (82) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2200) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `QueueManager` در پیاده‌سازی یافت نشد. مستندات 7 متد عمومی تعریف می‌کند.
   - ایجاد `src/QueueManager.php`
   - پیاده‌سازی متدها: push, later, pushOn, batch, chain, size, connection
1. 🔴 **missing_class** — کلاس `Worker` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/Worker.php`
   - پیاده‌سازی متدها: run, stop, daemon
1. 🔴 **missing_tests** — مستندات 12 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (82) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2200) است.

### rbac (`DOC-057`)

- **Repository:** `Tavaan-Engine-RBAC`
- **اولویت:** **P0** — فاز M4
- **LOC:** هدف 1600 | واقعی 54
- **فایل‌های src:** 1
- **تست:** 0 متد / 11 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Gate` در پیاده‌سازی یافت نشد. مستندات 11 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `RoleManager` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند. |
| 3 | missing_tests | 🔴 | مستندات 11 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (54) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1600) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Gate` در پیاده‌سازی یافت نشد. مستندات 11 متد عمومی تعریف می‌کند.
   - ایجاد `src/Gate.php`
   - پیاده‌سازی متدها: define, policy, before, after, allows, denies, check, any, authorize, forUser, abilities
1. 🔴 **missing_class** — کلاس `RoleManager` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند.
   - ایجاد `src/RoleManager.php`
   - پیاده‌سازی متدها: create, assign, remove, hierarchy, syncFromModules
1. 🔴 **missing_tests** — مستندات 11 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (54) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1600) است.

### realtime (`DOC-045`)

- **Repository:** `Tavaan-Engine-Realtime`
- **اولویت:** **P2** — فاز M6
- **LOC:** هدف 1200 | واقعی 67
- **فایل‌های src:** 1
- **تست:** 0 متد / 8 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `RealtimeManager` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `Broadcast` در پیاده‌سازی یافت نشد. مستندات 2 متد عمومی تعریف می‌کند. |
| 3 | missing_tests | 🔴 | مستندات 8 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (67) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1200) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `RealtimeManager` در پیاده‌سازی یافت نشد. مستندات 3 متد عمومی تعریف می‌کند.
   - ایجاد `src/RealtimeManager.php`
   - پیاده‌سازی متدها: broadcast, presence, publish
1. 🔴 **missing_class** — کلاس `Broadcast` در پیاده‌سازی یافت نشد. مستندات 2 متد عمومی تعریف می‌کند.
   - ایجاد `src/Broadcast.php`
   - پیاده‌سازی متدها: channel, connection
1. 🔴 **missing_tests** — مستندات 8 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (67) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1200) است.

### report (`DOC-072`)

- **Repository:** `Tavaan-Engine-Report`
- **اولویت:** **P2** — فاز M7
- **LOC:** هدف 1600 | واقعی 75
- **فایل‌های src:** 1
- **تست:** 0 متد / 9 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `ReportBuilder` در پیاده‌سازی یافت نشد. مستندات 7 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `ReportExporter` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند. |
| 3 | missing_tests | 🔴 | مستندات 9 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (75) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1600) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `ReportBuilder` در پیاده‌سازی یافت نشد. مستندات 7 متد عمومی تعریف می‌کند.
   - ایجاد `src/ReportBuilder.php`
   - پیاده‌سازی متدها: dataset, addField, addFilter, groupBy, pivot, orderBy, run
1. 🔴 **missing_class** — کلاس `ReportExporter` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند.
   - ایجاد `src/ReportExporter.php`
   - پیاده‌سازی متدها: csv, xlsx, html, json, pdf, stream
1. 🔴 **missing_tests** — مستندات 9 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (75) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1600) است.

### router (`DOC-040`)

- **Repository:** `Tavaan-Engine-Router`
- **اولویت:** **P0** — فاز M2
- **LOC:** هدف 1400 | واقعی 220
- **فایل‌های src:** 1
- **تست:** 3 متد / 18 سناریو
- **نقص‌ها:** 3 (🔴 1 / 🟡 1 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `UrlGenerator` در پیاده‌سازی یافت نشد. مستندات 11 متد عمومی تعریف می‌کند. |
| 2 | insufficient_tests | 🟡 | پوشش تست ناکافی: مستندات 18 سناریو، پیاده‌سازی 3 متد تست. |
| 3 | loc_shortfall | 🟢 | LOC پیاده‌سازی (220) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1400) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `UrlGenerator` در پیاده‌سازی یافت نشد. مستندات 11 متد عمومی تعریف می‌کند.
   - ایجاد `src/UrlGenerator.php`
   - پیاده‌سازی متدها: route, action, url, asset, current, previous, full, signed, temporarySignedRoute, isValidSignature, to
2. 🟡 **insufficient_tests** — پوشش تست ناکافی: مستندات 18 سناریو، پیاده‌سازی 3 متد تست.
3. 🟢 **loc_shortfall** — LOC پیاده‌سازی (220) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1400) است.

### scaffold (`DOC-077`)

- **Repository:** `Tavaan-Engine-Scaffold`
- **اولویت:** **P1** — فاز M8
- **LOC:** هدف 1200 | واقعی 66
- **فایل‌های src:** 1
- **تست:** 0 متد / 6 سناریو
- **نقص‌ها:** 3 (🔴 2 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `GeneratorManager` در پیاده‌سازی یافت نشد. مستندات 2 متد عمومی تعریف می‌کند. |
| 2 | missing_tests | 🔴 | مستندات 6 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 3 | loc_shortfall | 🟢 | LOC پیاده‌سازی (66) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1200) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `GeneratorManager` در پیاده‌سازی یافت نشد. مستندات 2 متد عمومی تعریف می‌کند.
   - ایجاد `src/GeneratorManager.php`
   - پیاده‌سازی متدها: generate, register
1. 🔴 **missing_tests** — مستندات 6 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
3. 🟢 **loc_shortfall** — LOC پیاده‌سازی (66) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1200) است.

### schedule (`DOC-062`)

- **Repository:** `Tavaan-Engine-Schedule`
- **اولویت:** **P1** — فاز M5
- **LOC:** هدف 700 | واقعی 77
- **فایل‌های src:** 1
- **تست:** 0 متد / 7 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `ScheduleManager` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `CronExpression` در پیاده‌سازی یافت نشد. مستندات 2 متد عمومی تعریف می‌کند. |
| 3 | missing_tests | 🔴 | مستندات 7 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (77) به‌طور قابل‌توجهی کمتر از تخمین مستندات (700) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `ScheduleManager` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند.
   - ایجاد `src/ScheduleManager.php`
   - پیاده‌سازی متدها: command, job, call, exec, events
1. 🔴 **missing_class** — کلاس `CronExpression` در پیاده‌سازی یافت نشد. مستندات 2 متد عمومی تعریف می‌کند.
   - ایجاد `src/CronExpression.php`
   - پیاده‌سازی متدها: isDue, nextRunDates
1. 🔴 **missing_tests** — مستندات 7 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (77) به‌طور قابل‌توجهی کمتر از تخمین مستندات (700) است.

### schema (`DOC-048`)

- **Repository:** `Tavaan-Engine-Schema`
- **اولویت:** **P0** — فاز M3
- **LOC:** هدف 1100 | واقعی 618
- **فایل‌های src:** 5
- **تست:** 39 متد / 6 سناریو
- **نقص‌ها:** 7 (🔴 0 / 🟡 7 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `introspect()` در کلاس `SchemaBuilder` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `all()` در کلاس `Blueprint` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `column()` در کلاس `Blueprint` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `types()` در کلاس `Blueprint` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `primary()` در کلاس `Blueprint` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `foreign()` در کلاس `Blueprint` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `fullText()` در کلاس `Blueprint` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `introspect()` در کلاس `SchemaBuilder` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `all()` در کلاس `Blueprint` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `column()` در کلاس `Blueprint` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `types()` در کلاس `Blueprint` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `primary()` در کلاس `Blueprint` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `foreign()` در کلاس `Blueprint` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `fullText()` در کلاس `Blueprint` پیاده‌سازی نشده.

### search (`DOC-052`)

- **Repository:** `Tavaan-Engine-Search`
- **اولویت:** **P1** — فاز M6
- **LOC:** هدف 1500 | واقعی 290
- **فایل‌های src:** 4
- **تست:** 28 متد / 8 سناریو
- **نقص‌ها:** 6 (🔴 0 / 🟡 5 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `delete()` در کلاس `SearchManager` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `indexMany()` در کلاس `SearchManager` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `createIndex()` در کلاس `SearchManager` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `dropIndex()` در کلاس `SearchManager` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `flush()` در کلاس `SearchManager` پیاده‌سازی نشده. |
| 6 | loc_shortfall | 🟢 | LOC پیاده‌سازی (290) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1500) است. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `delete()` در کلاس `SearchManager` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `indexMany()` در کلاس `SearchManager` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `createIndex()` در کلاس `SearchManager` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `dropIndex()` در کلاس `SearchManager` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `flush()` در کلاس `SearchManager` پیاده‌سازی نشده.
6. 🟢 **loc_shortfall** — LOC پیاده‌سازی (290) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1500) است.

### security (`DOC-059`)

- **Repository:** `Tavaan-Engine-Security`
- **اولویت:** **P0** — فاز M4
- **LOC:** هدف 1500 | واقعی 93
- **فایل‌های src:** 1
- **تست:** 0 متد / 10 سناریو
- **نقص‌ها:** 5 (🔴 4 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Security` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `RateLimiter` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند. |
| 3 | missing_class | 🔴 | کلاس `Csrf` در پیاده‌سازی یافت نشد. مستندات 4 متد عمومی تعریف می‌کند. |
| 4 | missing_tests | 🔴 | مستندات 10 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 5 | loc_shortfall | 🟢 | LOC پیاده‌سازی (93) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1500) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Security` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند.
   - ایجاد `src/Security.php`
   - پیاده‌سازی متدها: sanitize, sign, validateSignature, normalize, ssrfCheck
1. 🔴 **missing_class** — کلاس `RateLimiter` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند.
   - ایجاد `src/RateLimiter.php`
   - پیاده‌سازی متدها: attempt, tooManyAttempts, hit, remaining, clear, availableIn
1. 🔴 **missing_class** — کلاس `Csrf` در پیاده‌سازی یافت نشد. مستندات 4 متد عمومی تعریف می‌کند.
   - ایجاد `src/Csrf.php`
   - پیاده‌سازی متدها: token, field, rotate, verify
1. 🔴 **missing_tests** — مستندات 10 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
5. 🟢 **loc_shortfall** — LOC پیاده‌سازی (93) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1500) است.

### session (`DOC-041`)

- **Repository:** `Tavaan-Engine-Session`
- **اولویت:** **P0** — فاز M2
- **LOC:** هدف 900 | واقعی 43
- **فایل‌های src:** 1
- **تست:** 0 متد / 10 سناریو
- **نقص‌ها:** 12 (🔴 1 / 🟡 10 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `put()` در کلاس `Session` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `exists()` در کلاس `Session` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `pull()` در کلاس `Session` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `forget()` در کلاس `Session` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `push()` در کلاس `Session` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `increment()` در کلاس `Session` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `keep()` در کلاس `Session` پیاده‌سازی نشده. |
| 8 | missing_method | 🟡 | متد `migrate()` در کلاس `Session` پیاده‌سازی نشده. |
| 9 | missing_method | 🟡 | متد `invalidate()` در کلاس `Session` پیاده‌سازی نشده. |
| 10 | missing_method | 🟡 | متد `id()` در کلاس `Session` پیاده‌سازی نشده. |
| 11 | missing_tests | 🔴 | مستندات 10 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 12 | loc_shortfall | 🟢 | LOC پیاده‌سازی (43) به‌طور قابل‌توجهی کمتر از تخمین مستندات (900) است. |

**وظایف تکمیل:**

1. 🔴 **missing_tests** — مستندات 10 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
2. 🟡 **missing_method** — متد `put()` در کلاس `Session` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `exists()` در کلاس `Session` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `pull()` در کلاس `Session` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `forget()` در کلاس `Session` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `push()` در کلاس `Session` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `increment()` در کلاس `Session` پیاده‌سازی نشده.
8. 🟡 **missing_method** — متد `keep()` در کلاس `Session` پیاده‌سازی نشده.
9. 🟡 **missing_method** — متد `migrate()` در کلاس `Session` پیاده‌سازی نشده.
10. 🟡 **missing_method** — متد `invalidate()` در کلاس `Session` پیاده‌سازی نشده.
11. 🟡 **missing_method** — متد `id()` در کلاس `Session` پیاده‌سازی نشده.
12. 🟢 **loc_shortfall** — LOC پیاده‌سازی (43) به‌طور قابل‌توجهی کمتر از تخمین مستندات (900) است.

### tenancy (`DOC-082E`)

- **Repository:** `Tavaan-Engine-Tenancy`
- **اولویت:** **P1** — فاز M6
- **LOC:** هدف 1000 | واقعی 500
- **فایل‌های src:** 10
- **تست:** 30 متد / 7 سناریو
- **نقص‌ها:** 1 (🔴 0 / 🟡 1 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `withoutCurrentScope()` در کلاس `TenantManager` پیاده‌سازی نشده. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `withoutCurrentScope()` در کلاس `TenantManager` پیاده‌سازی نشده.

### test (`DOC-084E`)

- **Repository:** `Tavaan-Engine-Test`
- **اولویت:** **P0** — فاز M8 (اما از M1 استفاده می‌شود)
- **LOC:** هدف 2500 | واقعی 703
- **فایل‌های src:** 11
- **تست:** 49 متد / 0 سناریو
- **نقص‌ها:** 9 (🔴 1 / 🟡 7 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `get()` در کلاس `TestCase` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `post()` در کلاس `TestCase` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `postJson()` در کلاس `TestCase` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `actingAs()` در کلاس `TestCase` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `...()` در کلاس `TestCase` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `suite()` در کلاس `TestRunner` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `result()` در کلاس `TestRunner` پیاده‌سازی نشده. |
| 8 | missing_class | 🔴 | کلاس `Factory` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند. |
| 9 | loc_shortfall | 🟢 | LOC پیاده‌سازی (703) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2500) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Factory` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند.
   - ایجاد `src/Factory.php`
   - پیاده‌سازی متدها: definition, create, make, count, state
2. 🟡 **missing_method** — متد `get()` در کلاس `TestCase` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `post()` در کلاس `TestCase` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `postJson()` در کلاس `TestCase` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `actingAs()` در کلاس `TestCase` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `...()` در کلاس `TestCase` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `suite()` در کلاس `TestRunner` پیاده‌سازی نشده.
8. 🟡 **missing_method** — متد `result()` در کلاس `TestRunner` پیاده‌سازی نشده.
9. 🟢 **loc_shortfall** — LOC پیاده‌سازی (703) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2500) است.

### upgrade (`DOC-081E`)

- **Repository:** `Tavaan-Engine-Upgrade`
- **اولویت:** **P2** — فاز M8
- **LOC:** هدف 600 | واقعی 228
- **فایل‌های src:** 1
- **تست:** 20 متد / 6 سناریو
- **نقص‌ها:** 1 (🔴 1 / 🟡 0 / 🟢 0)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `Upgrader` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `Upgrader` در پیاده‌سازی یافت نشد. مستندات 5 متد عمومی تعریف می‌کند.
   - ایجاد `src/Upgrader.php`
   - پیاده‌سازی متدها: upgrade, check, rollback, status, patches

### validation (`DOC-051`)

- **Repository:** `Tavaan-Engine-Validation`
- **اولویت:** **P0** — فاز M3
- **LOC:** هدف 2200 | واقعی 537
- **فایل‌های src:** 5
- **تست:** 42 متد / 12 سناریو
- **نقص‌ها:** 6 (🔴 1 / 🟡 4 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `extend()` در کلاس `Validator` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `replacer()` در کلاس `Validator` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `forDto()` در کلاس `Validator` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `sometimes()` در کلاس `Validator` پیاده‌سازی نشده. |
| 5 | missing_class | 🔴 | کلاس `FormRequest` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند. |
| 6 | loc_shortfall | 🟢 | LOC پیاده‌سازی (537) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2200) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `FormRequest` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند.
   - ایجاد `src/FormRequest.php`
   - پیاده‌سازی متدها: authorize, rules, messages, attributes, validated, validateResolved
2. 🟡 **missing_method** — متد `extend()` در کلاس `Validator` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `replacer()` در کلاس `Validator` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `forDto()` در کلاس `Validator` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `sometimes()` در کلاس `Validator` پیاده‌سازی نشده.
6. 🟢 **loc_shortfall** — LOC پیاده‌سازی (537) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2200) است.

### view (`DOC-043`)

- **Repository:** `Tavaan-Engine-View`
- **اولویت:** **P0** — فاز M2
- **LOC:** هدف 1800 | واقعی 327
- **فایل‌های src:** 6
- **تست:** 32 متد / 18 سناریو
- **نقص‌ها:** 13 (🔴 0 / 🟡 12 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_method | 🟡 | متد `addNamespace()` در کلاس `ViewFactory` پیاده‌سازی نشده. |
| 2 | missing_method | 🟡 | متد `addLocation()` در کلاس `ViewFactory` پیاده‌سازی نشده. |
| 3 | missing_method | 🟡 | متد `directive()` در کلاس `ViewFactory` پیاده‌سازی نشده. |
| 4 | missing_method | 🟡 | متد `composer()` در کلاس `ViewFactory` پیاده‌سازی نشده. |
| 5 | missing_method | 🟡 | متد `component()` در کلاس `ViewFactory` پیاده‌سازی نشده. |
| 6 | missing_method | 🟡 | متد `renderEach()` در کلاس `ViewFactory` پیاده‌سازی نشده. |
| 7 | missing_method | 🟡 | متد `file()` در کلاس `ViewFactory` پیاده‌سازی نشده. |
| 8 | missing_method | 🟡 | متد `first()` در کلاس `ViewFactory` پیاده‌سازی نشده. |
| 9 | missing_method | 🟡 | متد `nest()` در کلاس `View` پیاده‌سازی نشده. |
| 10 | missing_method | 🟡 | متد `extends()` در کلاس `View` پیاده‌سازی نشده. |
| 11 | missing_method | 🟡 | متد `section()` در کلاس `View` پیاده‌سازی نشده. |
| 12 | missing_method | 🟡 | متد `css()` در کلاس `Escaper` پیاده‌سازی نشده. |
| 13 | loc_shortfall | 🟢 | LOC پیاده‌سازی (327) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1800) است. |

**وظایف تکمیل:**

1. 🟡 **missing_method** — متد `addNamespace()` در کلاس `ViewFactory` پیاده‌سازی نشده.
2. 🟡 **missing_method** — متد `addLocation()` در کلاس `ViewFactory` پیاده‌سازی نشده.
3. 🟡 **missing_method** — متد `directive()` در کلاس `ViewFactory` پیاده‌سازی نشده.
4. 🟡 **missing_method** — متد `composer()` در کلاس `ViewFactory` پیاده‌سازی نشده.
5. 🟡 **missing_method** — متد `component()` در کلاس `ViewFactory` پیاده‌سازی نشده.
6. 🟡 **missing_method** — متد `renderEach()` در کلاس `ViewFactory` پیاده‌سازی نشده.
7. 🟡 **missing_method** — متد `file()` در کلاس `ViewFactory` پیاده‌سازی نشده.
8. 🟡 **missing_method** — متد `first()` در کلاس `ViewFactory` پیاده‌سازی نشده.
9. 🟡 **missing_method** — متد `nest()` در کلاس `View` پیاده‌سازی نشده.
10. 🟡 **missing_method** — متد `extends()` در کلاس `View` پیاده‌سازی نشده.
11. 🟡 **missing_method** — متد `section()` در کلاس `View` پیاده‌سازی نشده.
12. 🟡 **missing_method** — متد `css()` در کلاس `Escaper` پیاده‌سازی نشده.
13. 🟢 **loc_shortfall** — LOC پیاده‌سازی (327) به‌طور قابل‌توجهی کمتر از تخمین مستندات (1800) است.

### workflow (`DOC-071`)

- **Repository:** `Tavaan-Engine-Workflow`
- **اولویت:** **P2** — فاز M7
- **LOC:** هدف 2000 | واقعی 112
- **فایل‌های src:** 1
- **تست:** 0 متد / 10 سناریو
- **نقص‌ها:** 4 (🔴 3 / 🟡 0 / 🟢 1)

| # | نوع | شدت | شرح |
|---|------|------|------|
| 1 | missing_class | 🔴 | کلاس `WorkflowManager` در پیاده‌سازی یافت نشد. مستندات 4 متد عمومی تعریف می‌کند. |
| 2 | missing_class | 🔴 | کلاس `ProcessInstance` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند. |
| 3 | missing_tests | 🔴 | مستندات 10 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست. |
| 4 | loc_shortfall | 🟢 | LOC پیاده‌سازی (112) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2000) است. |

**وظایف تکمیل:**

1. 🔴 **missing_class** — کلاس `WorkflowManager` در پیاده‌سازی یافت نشد. مستندات 4 متد عمومی تعریف می‌کند.
   - ایجاد `src/WorkflowManager.php`
   - پیاده‌سازی متدها: define, start, instance, definitions
1. 🔴 **missing_class** — کلاس `ProcessInstance` در پیاده‌سازی یافت نشد. مستندات 6 متد عمومی تعریف می‌کند.
   - ایجاد `src/ProcessInstance.php`
   - پیاده‌سازی متدها: fire, currentState, can, variables, complete, cancel
1. 🔴 **missing_tests** — مستندات 10 سناریوی تست تعریف می‌کند اما هیچ فایل تستی موجود نیست.
4. 🟢 **loc_shortfall** — LOC پیاده‌سازی (112) به‌طور قابل‌توجهی کمتر از تخمین مستندات (2000) است.

## ۵. نقشه راه تکمیل

برای تکمیل موتورهای ناقص، این اولویت‌بندی توصیه می‌شود:

### موتورهای P0 ناقص (25)

| # | موتور | نقص‌های 🔴 | نقص‌های 🟡 | گام اول |
|---|-------|------------|------------|---------|
| 1 | `auth` | 1 | 8 | missing_method |
| 2 | `cache` | 0 | 5 | missing_method |
| 3 | `config` | 0 | 2 | missing_method |
| 4 | `container` | 0 | 6 | missing_method |
| 5 | `cookie` | 1 | 0 | missing_class |
| 6 | `crypt` | 2 | 0 | missing_class |
| 7 | `database` | 0 | 36 | missing_method |
| 8 | `error` | 1 | 3 | missing_class |
| 9 | `event` | 1 | 2 | missing_method |
| 10 | `hash` | 0 | 1 | missing_method |
| 11 | `http` | 1 | 12 | missing_method |
| 12 | `i18n` | 1 | 1 | missing_method |
| 13 | `jalali` | 1 | 11 | missing_method |
| 14 | `log` | 1 | 4 | missing_method |
| 15 | `migration` | 3 | 0 | missing_class |
| 16 | `module` | 2 | 0 | missing_class |
| 17 | `orm` | 0 | 16 | missing_method |
| 18 | `rbac` | 3 | 0 | missing_class |
| 19 | `router` | 1 | 1 | missing_class |
| 20 | `schema` | 0 | 7 | missing_method |
| 21 | `security` | 4 | 0 | missing_class |
| 22 | `session` | 1 | 10 | missing_method |
| 23 | `test` | 1 | 7 | missing_method |
| 24 | `validation` | 1 | 4 | missing_method |
| 25 | `view` | 0 | 12 | missing_method |

### موتورهای P1 ناقص (15)

| # | موتور | نقص‌های 🔴 | نقص‌های 🟡 | گام اول |
|---|-------|------------|------------|---------|
| 1 | `api` | 3 | 0 | missing_class |
| 2 | `audit` | 1 | 0 | missing_class |
| 3 | `console` | 1 | 1 | missing_method |
| 4 | `filesystem` | 0 | 2 | missing_method |
| 5 | `http-client` | 1 | 0 | missing_class |
| 6 | `mail` | 1 | 4 | missing_class |
| 7 | `media` | 1 | 0 | missing_class |
| 8 | `notification` | 1 | 4 | missing_class |
| 9 | `observability` | 2 | 0 | missing_class |
| 10 | `plugin` | 3 | 0 | missing_class |
| 11 | `queue` | 3 | 0 | missing_class |
| 12 | `scaffold` | 2 | 0 | missing_class |
| 13 | `schedule` | 3 | 0 | missing_class |
| 14 | `search` | 0 | 5 | missing_method |
| 15 | `tenancy` | 0 | 1 | missing_method |

### موتورهای P2 ناقص (8)

| # | موتور | نقص‌های 🔴 | نقص‌های 🟡 | گام اول |
|---|-------|------------|------------|---------|
| 1 | `admin` | 3 | 4 | missing_method |
| 2 | `backup` | 2 | 0 | missing_class |
| 3 | `feature-flag` | 2 | 0 | missing_class |
| 4 | `payment` | 2 | 0 | missing_class |
| 5 | `realtime` | 3 | 0 | missing_class |
| 6 | `report` | 3 | 0 | missing_class |
| 7 | `upgrade` | 1 | 0 | missing_class |
| 8 | `workflow` | 3 | 0 | missing_class |

## ۶. آمار کیفیت

- **مجموع LOC (src/):** 17380
- **مجموع متدهای تست:** 1030
- **مجموع سناریوهای تست مستندات:** 469
- **پوشش تست (تقریبی):** 219.6%
- **مجموع کلاس‌های API مستندات:** 98
- **مجموع معیارهای پذیرش:** 146

## ۷. درصد تکمیل

- ✅ **کامل:** 4 / 52 (7.7%)
- 🟡 **ناقص متوسط:** 11 / 52 (21.2%)
- 🔴 **ناقص بالا:** 37 / 52 (71.2%)

---
*Generated by Tavaan Comprehensive Gap Analyzer on 2026-11-03 13:43:39 UTC*