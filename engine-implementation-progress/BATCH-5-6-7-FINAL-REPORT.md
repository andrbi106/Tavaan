# Batch 5, 6, 7 — گزارش نهایی (بازبینی‌شده)

> تاریخ: 2026-11-03

## 🎉 خلاصه

| Batch | موتورها | Stub‌ها پر شد | Stub‌های مشروع | وضعیت |
|-------|---------|--------------|----------------|--------|
| Batch 5 | Auth, Event, Crypt | 13 | 2 | ✅ |
| Batch 6 | I18n, Module, Session | 15 | 1 | ✅ |
| Batch 7 | Compat, Config, Container | 5 | 5 | ✅ |
| **مجموع** | **9 موتور** | **33** | **8** | ✅ |

## موتورهای تکمیل‌شده

### Batch 5 (P0)
| # | موتور | Stub‌ها | Commit | شرح |
|---|-------|--------|--------|------|
| 1 | Auth | 8/8 ✅ | `409e93a` | devices/once/otp/resetPassword/sendPasswordResetLink/token/twoFactor/validate |
| 2 | Event | 4/4 ✅ | `453b4a5` | subscribe/until/fake + extend (2 legitimate null) |
| 3 | Crypt | 2/2 ✅ | `8548513` | BlindIndex: compute/verify with HMAC |

### Batch 6 (P0)
| # | موتور | Stub‌ها | Commit | شرح |
|---|-------|--------|--------|------|
| 4 | I18n | 5/5 ✅ | `fe58ed4` | PersianFormatter: digits/number/currency/date/toLatinDigits |
| 5 | Module | 7/7 ✅ | `a94c826` | ModuleManager: install/uninstall/enable/disable/update/list/info + ModuleRunner |
| 6 | Session | 3/3 ✅ | `2989871` | invalidate/keep/migrate |

### Batch 7 (P0)
| # | موتور | Stub‌ها | Commit | شرح |
|---|-------|--------|--------|------|
| 7 | Compat | 0 ✅ | — | 3 null returns are legitimate (missing file/stream) |
| 8 | Config | 1/1 ✅ | `aa7fa72` | Repository::masked() (2 null returns are legitimate) |
| 9 | Container | 5/5 ✅ | `1477825` | dependencyGraph/flushScoped/forgetInstance/has/lazy/stats |

## توضیح `return null;` های مشروع

برخی `return null;` در کد **رفتار صحیح** هستند نه stub:
- **Event**: `return null` وقتی در حالت fake است (نرمال) یا کلاس handler متد `handle` ندارد
- **Module**: `return null` وقتی ماژول یافت نشد (خطای 404)
- **Compat/MagicBytesDetector**: `return null` وقتی فایل/stream موجود نیست
- **Config/EnvRepository**: `return null` وقتی متغیر محیطی موجود نیست یا JSON نامعتبر است

این موارد **رفتار طراحی‌شده** هستند و نباید تغییر کنند.

---
*Generated on 2026-11-03*
