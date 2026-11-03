# نقشه راه پیاده‌سازی ۵۲ موتور Tavaan

> این سند ترتیب اجرای پیاده‌سازی ۵۲ موتور را بر اساس وابستگی‌های سخت (`requires`) مشخص می‌کند.
> سافت‌دپندنسی‌ها در زمان پیاده‌سازی نادیده گرفته می‌شوند (هر موتور باید بدون آن‌ها کار کند).

## ۱. خلاصهٔ اجرایی

- **تعداد کل موتورها:** 52
- **مراحل اجرا (levels):** 9
- **موتورهای مرحلهٔ ۰ (بدون وابستگی):** 3
- **موتورهای مرحلهٔ ۱:** 2
- **موتورهای مرحلهٔ ۲:** 15
- **موتورهای مرحلهٔ ۳+:** 32

## ۲. ترتیب اجرا (Topological Sort)

موتورها به ترتیب زیر پیاده‌سازی می‌شوند. هر موتور فقط زمانی شروع می‌شود که همهٔ وابستگی‌های سخت (`requires`) آن تکمیل شده باشند.

| # | موتور | Repository | مرحله | اولویت | فاز | وابستگی‌های سخت | وابستگی‌های نرم |
|---|-------|------------|-------|--------|------|-----------------|-----------------|
| 1 | Compat | `Tavaan-Engine-Compat` | 0 | P0 | ? | — | — |
| 2 | Container | `Tavaan-Engine-Container` | 0 | P0 | ? | — | — |
| 3 | Config | `Tavaan-Engine-Config` | 1 | P0 | ? | `container` | — |
| 4 | Crypt | `Tavaan-Engine-Crypt` | 2 | P0 | ? | `config` | — |
| 5 | Event | `Tavaan-Engine-Event` | 2 | P0 | ? | `container`, `config` | `queue`, `database`, `realtime` |
| 6 | Cache | `Tavaan-Engine-Cache` | 3 | P0 | ? | `config`, `event` | `database` |
| 7 | Hash | `Tavaan-Engine-Hash` | 2 | P0 | ? | `config` | — |
| 8 | I18n | `Tavaan-Engine-I18n` | 2 | P0 | ? | `config` | — |
| 9 | Jalali | `Tavaan-Engine-Jalali` | 3 | P0 | ? | `i18n` | — |
| 10 | Log | `Tavaan-Engine-Log` | 2 | P0 | ? | `config` | `event`, `queue`, `database` |
| 11 | Database | `Tavaan-Engine-Database` | 3 | P0 | ? | `config`, `event`, `log` | — |
| 12 | Error | `Tavaan-Engine-Error` | 3 | P0 | ? | `config`, `log` | `event` |
| 13 | Module | `Tavaan-Engine-Module` | 2 | P0 | ? | `container`, `config` | — |
| 14 | ORM | `Tavaan-Engine-ORM` | 4 | P0 | ? | `database`, `event` | `i18n`, `crypt`, `hash` |
| 15 | Pipeline | `Tavaan-Engine-Pipeline` | 1 | P0 | ? | `container` | — |
| 16 | Http | `Tavaan-Engine-Http` | 4 | P0 | ? | `pipeline`, `event`, `error`, `config` | `session`, `router`, `view`, `cors`, `cookie`, `security`, `validation` |
| 17 | Cookie | `Tavaan-Engine-Cookie` | 5 | P0 | ? | `http`, `crypt` | — |
| 18 | CORS | `Tavaan-Engine-CORS` | 5 | P0 | ? | `http`, `config` | — |
| 19 | Router | `Tavaan-Engine-Router` | 5 | P0 | ? | `http`, `container`, `config` | — |
| 20 | Schema | `Tavaan-Engine-Schema` | 4 | P0 | ? | `database` | — |
| 21 | Security | `Tavaan-Engine-Security` | 5 | P0 | ? | `http`, `crypt`, `cache`, `config` | `session`, `router` |
| 22 | Session | `Tavaan-Engine-Session` | 5 | P0 | ? | `http`, `crypt`, `config` | `database`, `cache` |
| 23 | Auth | `Tavaan-Engine-Auth` | 6 | P0 | ? | `session`, `hash`, `crypt`, `event`, `database`, `cache`, `config` | `http`, `orm`, `notification` |
| 24 | RBAC | `Tavaan-Engine-RBAC` | 7 | P0 | ? | `auth`, `database`, `cache`, `event`, `config` | — |
| 25 | Test | `Tavaan-Engine-Test` | 0 | P0 | ? | — | — |
| 26 | Validation | `Tavaan-Engine-Validation` | 3 | P0 | ? | `i18n`, `config` | `database`, `http` |
| 27 | View | `Tavaan-Engine-View` | 3 | P0 | ? | `event`, `i18n`, `config` | `rbac`, `http`, `session` |
| 28 | API | `Tavaan-Engine-API` | 5 | P1 | ? | `config`, `http` | `validation`, `orm`, `cache`, `router` |
| 29 | Audit | `Tavaan-Engine-Audit` | 4 | P1 | ? | `event`, `database`, `log`, `crypt`, `config` | `orm`, `auth`, `http` |
| 30 | Console | `Tavaan-Engine-Console` | 2 | P1 | ? | `container`, `config` | `event` |
| 31 | Migration | `Tavaan-Engine-Migration` | 5 | P0 | ? | `database`, `schema`, `console` | — |
| 32 | Filesystem | `Tavaan-Engine-Filesystem` | 2 | P1 | ? | `config` | `crypt`, `http`, `compat` |
| 33 | HttpClient | `Tavaan-Engine-Http-Client` | 3 | P1 | ? | `config`, `event` | `security`, `cache`, `compat` |
| 34 | Mail | `Tavaan-Engine-Mail` | 3 | P1 | ? | `config`, `event` | `view`, `queue`, `log`, `filesystem` |
| 35 | Media | `Tavaan-Engine-Media` | 2 | P1 | ? | `config` | `filesystem`, `database`, `compat`, `http` |
| 36 | Notification | `Tavaan-Engine-Notification` | 3 | P1 | ? | `config`, `event` | `mail`, `queue`, `database`, `http-client`, `cache`, `log` |
| 37 | Observability | `Tavaan-Engine-Observability` | 3 | P1 | ? | `config`, `log` | `event`, `http`, `cache`, `database`, `queue` |
| 38 | Optimizer | `Tavaan-Engine-Optimizer` | 3 | P1 | ? | `config`, `console` | — |
| 39 | Plugin | `Tavaan-Engine-Plugin` | 3 | P1 | ? | `module`, `filesystem`, `crypt` | — |
| 40 | Queue | `Tavaan-Engine-Queue` | 3 | P1 | ? | `config`, `event` | `database`, `cache`, `log` |
| 41 | Scaffold | `Tavaan-Engine-Scaffold` | 3 | P1 | ? | `console`, `filesystem` | — |
| 42 | Schedule | `Tavaan-Engine-Schedule` | 3 | P1 | ? | `config`, `console` | `cache`, `queue`, `log` |
| 43 | Search | `Tavaan-Engine-Search` | 2 | P1 | ? | `config` | `database`, `event`, `orm` |
| 44 | Tenancy | `Tavaan-Engine-Tenancy` | 2 | P1 | ? | `config` | `database`, `cache`, `http`, `event`, `console`, `migration`, `orm`, `crypt` |
| 45 | Admin | `Tavaan-Engine-Admin` | 8 | P2 | ? | `view`, `rbac`, `orm`, `validation`, `http` | — |
| 46 | Backup | `Tavaan-Engine-Backup` | 3 | P2 | ? | `config`, `filesystem` | `database`, `crypt`, `cache`, `compat` |
| 47 | FeatureFlag | `Tavaan-Engine-Feature-Flag` | 2 | P2 | ? | `config` | `cache`, `database`, `rbac`, `tenancy` |
| 48 | Payment | `Tavaan-Engine-Payment` | 2 | P2 | ? | `config` | `http-client`, `database`, `migration`, `orm`, `event`, `crypt`, `http`, `console` |
| 49 | Realtime | `Tavaan-Engine-Realtime` | 5 | P2 | ? | `config`, `event`, `http` | `database`, `cache`, `queue`, `auth` |
| 50 | Report | `Tavaan-Engine-Report` | 2 | P2 | ? | `config` | `database`, `filesystem`, `view`, `i18n`, `compat`, `http` |
| 51 | Upgrade | `Tavaan-Engine-Upgrade` | 4 | P2 | ? | `console`, `database`, `filesystem` | — |
| 52 | Workflow | `Tavaan-Engine-Workflow` | 2 | P2 | ? | `config` | `event`, `database`, `migration`, `rbac`, `queue`, `console`, `auth` |

## ۳. گروه‌بندی بر اساس مرحله (Level)

### مرحلهٔ 0 — 3 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| Compat | `Tavaan-Engine-Compat` | P0 | ? |
| Container | `Tavaan-Engine-Container` | P0 | ? |
| Test | `Tavaan-Engine-Test` | P0 | ? |

### مرحلهٔ 1 — 2 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| Config | `Tavaan-Engine-Config` | P0 | ? |
| Pipeline | `Tavaan-Engine-Pipeline` | P0 | ? |

### مرحلهٔ 2 — 15 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| Crypt | `Tavaan-Engine-Crypt` | P0 | ? |
| Event | `Tavaan-Engine-Event` | P0 | ? |
| Hash | `Tavaan-Engine-Hash` | P0 | ? |
| I18n | `Tavaan-Engine-I18n` | P0 | ? |
| Log | `Tavaan-Engine-Log` | P0 | ? |
| Module | `Tavaan-Engine-Module` | P0 | ? |
| Console | `Tavaan-Engine-Console` | P1 | ? |
| Filesystem | `Tavaan-Engine-Filesystem` | P1 | ? |
| Media | `Tavaan-Engine-Media` | P1 | ? |
| Search | `Tavaan-Engine-Search` | P1 | ? |
| Tenancy | `Tavaan-Engine-Tenancy` | P1 | ? |
| FeatureFlag | `Tavaan-Engine-Feature-Flag` | P2 | ? |
| Payment | `Tavaan-Engine-Payment` | P2 | ? |
| Report | `Tavaan-Engine-Report` | P2 | ? |
| Workflow | `Tavaan-Engine-Workflow` | P2 | ? |

### مرحلهٔ 3 — 16 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| Cache | `Tavaan-Engine-Cache` | P0 | ? |
| Jalali | `Tavaan-Engine-Jalali` | P0 | ? |
| Database | `Tavaan-Engine-Database` | P0 | ? |
| Error | `Tavaan-Engine-Error` | P0 | ? |
| Validation | `Tavaan-Engine-Validation` | P0 | ? |
| View | `Tavaan-Engine-View` | P0 | ? |
| HttpClient | `Tavaan-Engine-Http-Client` | P1 | ? |
| Mail | `Tavaan-Engine-Mail` | P1 | ? |
| Notification | `Tavaan-Engine-Notification` | P1 | ? |
| Observability | `Tavaan-Engine-Observability` | P1 | ? |
| Optimizer | `Tavaan-Engine-Optimizer` | P1 | ? |
| Plugin | `Tavaan-Engine-Plugin` | P1 | ? |
| Queue | `Tavaan-Engine-Queue` | P1 | ? |
| Scaffold | `Tavaan-Engine-Scaffold` | P1 | ? |
| Schedule | `Tavaan-Engine-Schedule` | P1 | ? |
| Backup | `Tavaan-Engine-Backup` | P2 | ? |

### مرحلهٔ 4 — 5 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| ORM | `Tavaan-Engine-ORM` | P0 | ? |
| Http | `Tavaan-Engine-Http` | P0 | ? |
| Schema | `Tavaan-Engine-Schema` | P0 | ? |
| Audit | `Tavaan-Engine-Audit` | P1 | ? |
| Upgrade | `Tavaan-Engine-Upgrade` | P2 | ? |

### مرحلهٔ 5 — 8 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| Cookie | `Tavaan-Engine-Cookie` | P0 | ? |
| CORS | `Tavaan-Engine-CORS` | P0 | ? |
| Router | `Tavaan-Engine-Router` | P0 | ? |
| Security | `Tavaan-Engine-Security` | P0 | ? |
| Session | `Tavaan-Engine-Session` | P0 | ? |
| API | `Tavaan-Engine-API` | P1 | ? |
| Migration | `Tavaan-Engine-Migration` | P0 | ? |
| Realtime | `Tavaan-Engine-Realtime` | P2 | ? |

### مرحلهٔ 6 — 1 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| Auth | `Tavaan-Engine-Auth` | P0 | ? |

### مرحلهٔ 7 — 1 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| RBAC | `Tavaan-Engine-RBAC` | P0 | ? |

### مرحلهٔ 8 — 1 موتور

این موتورها می‌توانند همزمان (parallel) پیاده‌سازی شوند چون وابستگی مشترک ندارند.

| موتور | Repository | اولویت | فاز |
|------|------------|--------|------|
| Admin | `Tavaan-Engine-Admin` | P2 | ? |

## ۴. رویکرد پیاده‌سازی

### ۴.۱ اصول

1. **استقلال کامل**: هر موتور بدون وابستگی سخت به سایر موتورها در زمان کامپایل/اجرای تست‌ها پیاده‌سازی شود. وابستگی‌ها فقط از طریق Contract (اینترفیس) تزریق شوند.
2. **Contract-First**: ابتدا Contractها در `src/Contracts/*Interface.php` تعریف شوند، سپس پیاده‌سازی‌ها.
3. **Test-Driven**: برای هر سناریوی T-NN یک متد تست نوشته شود، سپس پیاده‌سازی حداقل لازم برای عبور تست.
4. **صفر وابستگی Composer**: هیچ `require` به کتابخانه خارجی به جز `php >= 8.2`.
5. **PHP 8.2+ only**: readonly classes, enums, first-class callable syntax, strict types.

### ۴.۲ گردش کار برای هر موتور

1. خواندن `engine-prompts/Tavaan-Engine-<Name>.md` به‌عنوان پرامپت پیاده‌سازی.
2. خواندن `ROADMAP.md` و `TICKET.md` موتور برای دیدن شکاف‌ها.
3. خواندن سند کامل موتور در `Tavaan-Doc/docs/03-engines/<key>.md`.
4. پیاده‌سازی به ترتیب:
   - `module.json` (به‌روزرسانی `autoload` به `src/`)
   - `config/<name>.php`
   - `src/Contracts/*Interface.php`
   - `src/<Name>ServiceProvider.php`
   - `src/<Manager>.php` و کلاس‌های اصلی
   - درایورها/Storeها/Adapterها
   - Migrationها
   - Commandها
   - Facade
   - `tests/Feature/<Engine>Test.php`
   - `README.md`
5. اجرای تست‌ها (در صورت امکان با PHP موجود) و اصلاح.
6. کامیت و پوش به مخزن موتور.
7. ثبت گزارش پیشرفت در `engine-implementation-progress/<EngineName>.md` و کامیت به مخزن هدف.

## ۵. گزارش پیشرفت

برای هر موتور پس از تکمیل، یک فایل در `engine-implementation-progress/` ساخته می‌شود با:

- نام موتور و تاریخ پیاده‌سازی
- تعداد فایل‌های تولیدشده (`src/`, `tests/`, `config/`, `migrations/`)
- LOC تولیدشده
- SHA کامیت در مخزن موتور
- SHA کامیت گزارش در مخزن هدف
- وضعیت (✅ تکمیل / ⚠️ ناقص / ❌ ناموفق)

جدول پیشرفت کلی در `engine-implementation-progress/STATUS.md` نگهداری می‌شود.

## ۶. محدودیت‌های شناخته‌شده

1. **GitHub rate limit**: هر مرحله ممکن است چند بار با secondary rate limit متوقف شود؛ صبر تا رفع محدودیت و ادامه.
2. **PHP runtime در سندباکس**: PHP موجود ممکن است همه extensionهای مورد نیاز (Redis, APCu, Memcached) را نداشته باشد؛ تست‌ها با fallback به in-memory انجام می‌شوند.
3. **PHPStan/CS-Fixer**: بررسی نهایی کیفیت کد در یک مرحلهٔ واحد بعد از تکمیل همهٔ موتورها اجرا می‌شود.
4. **ساختار کلاس‌های core**: کلاس‌های پایه `Tavaan\Core\*` (Container, ServiceProvider, etc.) در مخزن `Tavaan-Core` موجودند و باید با کپی محلی یا autoload صحیح در موتورها استفاده شوند.

## ۷. وضعیت فعلی

| شاخص | مقدار |
|------|------|
| موتورهای پردازش‌شده | 0 / 52 |
| موتورهای تکمیل‌شده (✅) | 0 |
| موتورهای ناقص (⚠️) | 0 |
| موتورهای ناموفق (❌) | 0 |
| LOC تولیدشده | 0 |

---
*این نقشه راه در 2026-11-03 09:53:17 UTC تولید شد.*