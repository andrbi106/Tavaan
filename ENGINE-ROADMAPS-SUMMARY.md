# خلاصهٔ نقشه‌های راه موتورها (Engine Roadmaps Summary)

> این سند به‌صورت خودکار پس از تحلیل تطابق ۵۲ موتور با مستندات `Derogaramin/Tavaan-Doc` تولید شد.
> تاریخ تولید: **2026-11-03 05:42:12 UTC**

## ۱. خلاصهٔ اجرایی

- **موتورهای بررسی‌شده:** 52 موتور
- **موتورهای کاملاً منطبق با مستندات:** 27 موتور (✅)
- **موتورهای دارای شکاف:** 25 موتور
- **موتورهای بدون پیاده‌سازی (فقط config):** 6 موتور
- **مجموع شکاف‌ها:** 79 مورد
  - 🔴 بالا (high): 35 مورد
  - 🟡 متوسط (medium): 42 مورد
  - 🟢 پایین (low): 2 مورد

## ۲. جدول کامل موتورها

| # | موتور | DOC-ID | اولویت | src | کلاس | تست | شکاف | 🔴/🟡/🟢 | ROADMAP |
|---|-------|--------|--------|-----|------|-----|------|---------|---------|
| 1 | [`Tavaan-Engine-API`](https://github.com/andrbi106/Tavaan-Engine-API) | DOC-044 | **P1** — فاز M6 | 17 | 17 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-API/blob/main/ROADMAP.md) |
| 2 | [`Tavaan-Engine-Admin`](https://github.com/andrbi106/Tavaan-Engine-Admin) | DOC-078 | **P2** — فاز M8 | 15 | 15 | 3 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Admin/blob/main/ROADMAP.md) |
| 3 | [`Tavaan-Engine-Audit`](https://github.com/andrbi106/Tavaan-Engine-Audit) | DOC-058 | **P1** — فاز M4 | 10 | 10 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Audit/blob/main/ROADMAP.md) |
| 4 | [`Tavaan-Engine-Auth`](https://github.com/andrbi106/Tavaan-Engine-Auth) | DOC-056 | **P0** — فاز M4 | 25 | 25 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Auth/blob/main/ROADMAP.md) |
| 5 | [`Tavaan-Engine-Backup`](https://github.com/andrbi106/Tavaan-Engine-Backup) | DOC-068 | **P2** — فاز M5 | 13 | 13 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Backup/blob/main/ROADMAP.md) |
| 6 | [`Tavaan-Engine-CORS`](https://github.com/andrbi106/Tavaan-Engine-CORS) | DOC-046 | **P0** — فاز M2 | 0 | 0 | 0 | 2 🔴 | 2/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-CORS/blob/main/ROADMAP.md) |
| 7 | [`Tavaan-Engine-Cache`](https://github.com/andrbi106/Tavaan-Engine-Cache) | DOC-060 | **P0** — فاز M4 | 13 | 13 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Cache/blob/main/ROADMAP.md) |
| 8 | [`Tavaan-Engine-Compat`](https://github.com/andrbi106/Tavaan-Engine-Compat) | DOC-083E | **P0** — فاز M1 (زیرساخت همهٔ موتورها) | 7 | 7 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Compat/blob/main/ROADMAP.md) |
| 9 | [`Tavaan-Engine-Config`](https://github.com/andrbi106/Tavaan-Engine-Config) | DOC-032 | **P0** — فاز M1 | 13 | 13 | 3 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Config/blob/main/ROADMAP.md) |
| 10 | [`Tavaan-Engine-Console`](https://github.com/andrbi106/Tavaan-Engine-Console) | DOC-076 | **P1** — فاز M5 | 31 | 31 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Console/blob/main/ROADMAP.md) |
| 11 | [`Tavaan-Engine-Container`](https://github.com/andrbi106/Tavaan-Engine-Container) | DOC-031 | **P0** — فاز M1 (اولین موتور) | 14 | 14 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/ROADMAP.md) |
| 12 | [`Tavaan-Engine-Cookie`](https://github.com/andrbi106/Tavaan-Engine-Cookie) | DOC-042 | **P0** — فاز M2 | 0 | 0 | 0 | 2 🔴 | 2/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Cookie/blob/main/ROADMAP.md) |
| 13 | [`Tavaan-Engine-Crypt`](https://github.com/andrbi106/Tavaan-Engine-Crypt) | DOC-054 | **P0** — فاز M4 | 7 | 7 | 1 | 3 🔴 | 3/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Crypt/blob/main/ROADMAP.md) |
| 14 | [`Tavaan-Engine-Database`](https://github.com/andrbi106/Tavaan-Engine-Database) | DOC-047 | **P0** — فاز M3 | 82 | 82 | 3 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/ROADMAP.md) |
| 15 | [`Tavaan-Engine-Error`](https://github.com/andrbi106/Tavaan-Engine-Error) | DOC-035 | **P0** — فاز M1 | 10 | 10 | 2 | 1 🔴 | 1/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Error/blob/main/ROADMAP.md) |
| 16 | [`Tavaan-Engine-Event`](https://github.com/andrbi106/Tavaan-Engine-Event) | DOC-033 | **P0** — فاز M1 | 12 | 12 | 2 | 1 🔴 | 1/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Event/blob/main/ROADMAP.md) |
| 17 | [`Tavaan-Engine-Feature-Flag`](https://github.com/andrbi106/Tavaan-Engine-Feature-Flag) | DOC-075 | **P2** — فاز M6 | 5 | 5 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Feature-Flag/blob/main/ROADMAP.md) |
| 18 | [`Tavaan-Engine-Filesystem`](https://github.com/andrbi106/Tavaan-Engine-Filesystem) | DOC-063 | **P1** — فاز M5 | 13 | 13 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Filesystem/blob/main/ROADMAP.md) |
| 19 | [`Tavaan-Engine-Hash`](https://github.com/andrbi106/Tavaan-Engine-Hash) | DOC-055 | **P0** — فاز M4 | 4 | 4 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Hash/blob/main/ROADMAP.md) |
| 20 | [`Tavaan-Engine-Http`](https://github.com/andrbi106/Tavaan-Engine-Http) | DOC-039 | **P0** — فاز M2 | 47 | 47 | 4 | 3 🟡 | 0/3/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Http/blob/main/ROADMAP.md) |
| 21 | [`Tavaan-Engine-Http-Client`](https://github.com/andrbi106/Tavaan-Engine-Http-Client) | DOC-064 | **P1** — فاز M5 | 19 | 19 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Http-Client/blob/main/ROADMAP.md) |
| 22 | [`Tavaan-Engine-I18n`](https://github.com/andrbi106/Tavaan-Engine-I18n) | DOC-069 | **P0** — فاز M2 | 7 | 7 | 2 | 3 🟡 | 0/3/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-I18n/blob/main/ROADMAP.md) |
| 23 | [`Tavaan-Engine-Jalali`](https://github.com/andrbi106/Tavaan-Engine-Jalali) | DOC-070 | **P0** — فاز M2 | 0 | 0 | 0 | 5 🔴 | 5/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Jalali/blob/main/ROADMAP.md) |
| 24 | [`Tavaan-Engine-Log`](https://github.com/andrbi106/Tavaan-Engine-Log) | DOC-036 | **P0** — فاز M1 | 20 | 20 | 1 | 2 🔴 | 1/1/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Log/blob/main/ROADMAP.md) |
| 25 | [`Tavaan-Engine-Mail`](https://github.com/andrbi106/Tavaan-Engine-Mail) | DOC-065 | **P1** — فاز M5 | 18 | 18 | 2 | 4 🟡 | 0/4/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Mail/blob/main/ROADMAP.md) |
| 26 | [`Tavaan-Engine-Media`](https://github.com/andrbi106/Tavaan-Engine-Media) | DOC-074 | **P1** — فاز M5 | 8 | 8 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Media/blob/main/ROADMAP.md) |
| 27 | [`Tavaan-Engine-Migration`](https://github.com/andrbi106/Tavaan-Engine-Migration) | DOC-049 | **P0** — فاز M3 | 6 | 6 | 5 | 4 🔴 | 3/0/1 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Migration/blob/main/ROADMAP.md) |
| 28 | [`Tavaan-Engine-Module`](https://github.com/andrbi106/Tavaan-Engine-Module) | DOC-038 | **P0** — فاز M1 | 14 | 14 | 2 | 5 🔴 | 2/3/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Module/blob/main/ROADMAP.md) |
| 29 | [`Tavaan-Engine-Notification`](https://github.com/andrbi106/Tavaan-Engine-Notification) | DOC-066 | **P1** — فاز M5 | 33 | 33 | 5 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Notification/blob/main/ROADMAP.md) |
| 30 | [`Tavaan-Engine-ORM`](https://github.com/andrbi106/Tavaan-Engine-ORM) | DOC-050 | **P0** — فاز M3 | 0 | 0 | 3 | 1 🔴 | 1/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-ORM/blob/main/ROADMAP.md) |
| 31 | [`Tavaan-Engine-Observability`](https://github.com/andrbi106/Tavaan-Engine-Observability) | DOC-067 | **P1** — فاز M6 | 27 | 27 | 2 | 2 🔴 | 2/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Observability/blob/main/ROADMAP.md) |
| 32 | [`Tavaan-Engine-Optimizer`](https://github.com/andrbi106/Tavaan-Engine-Optimizer) | DOC-037 | **P1** — فاز M1 | 6 | 6 | 0 | 3 🔴 | 2/0/1 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Optimizer/blob/main/ROADMAP.md) |
| 33 | [`Tavaan-Engine-Payment`](https://github.com/andrbi106/Tavaan-Engine-Payment) | DOC-073 | **P2** — فاز M7 | 34 | 34 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Payment/blob/main/ROADMAP.md) |
| 34 | [`Tavaan-Engine-Pipeline`](https://github.com/andrbi106/Tavaan-Engine-Pipeline) | DOC-034 | **P0** — فاز M1 | 5 | 5 | 1 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Pipeline/blob/main/ROADMAP.md) |
| 35 | [`Tavaan-Engine-Plugin`](https://github.com/andrbi106/Tavaan-Engine-Plugin) | DOC-079 | **P1** — فاز M8 | 20 | 20 | 5 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Plugin/blob/main/ROADMAP.md) |
| 36 | [`Tavaan-Engine-Queue`](https://github.com/andrbi106/Tavaan-Engine-Queue) | DOC-061 | **P1** — فاز M5 | 48 | 48 | 14 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Queue/blob/main/ROADMAP.md) |
| 37 | [`Tavaan-Engine-RBAC`](https://github.com/andrbi106/Tavaan-Engine-RBAC) | DOC-057 | **P0** — فاز M4 | 12 | 12 | 1 | 2 🟡 | 0/2/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-RBAC/blob/main/ROADMAP.md) |
| 38 | [`Tavaan-Engine-Realtime`](https://github.com/andrbi106/Tavaan-Engine-Realtime) | DOC-045 | **P2** — فاز M6 | 15 | 15 | 2 | 2 🔴 | 1/1/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Realtime/blob/main/ROADMAP.md) |
| 39 | [`Tavaan-Engine-Report`](https://github.com/andrbi106/Tavaan-Engine-Report) | DOC-072 | **P2** — فاز M7 | 20 | 20 | 2 | 5 🟡 | 0/5/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Report/blob/main/ROADMAP.md) |
| 40 | [`Tavaan-Engine-Router`](https://github.com/andrbi106/Tavaan-Engine-Router) | DOC-040 | **P0** — فاز M2 | 0 | 0 | 0 | 3 🔴 | 3/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Router/blob/main/ROADMAP.md) |
| 41 | [`Tavaan-Engine-Scaffold`](https://github.com/andrbi106/Tavaan-Engine-Scaffold) | DOC-077 | **P1** — فاز M8 | 40 | 40 | 2 | 1 🔴 | 1/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Scaffold/blob/main/ROADMAP.md) |
| 42 | [`Tavaan-Engine-Schedule`](https://github.com/andrbi106/Tavaan-Engine-Schedule) | DOC-062 | **P1** — فاز M5 | 7 | 7 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Schedule/blob/main/ROADMAP.md) |
| 43 | [`Tavaan-Engine-Schema`](https://github.com/andrbi106/Tavaan-Engine-Schema) | DOC-048 | **P0** — فاز M3 | 0 | 0 | 2 | 3 🔴 | 3/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Schema/blob/main/ROADMAP.md) |
| 44 | [`Tavaan-Engine-Search`](https://github.com/andrbi106/Tavaan-Engine-Search) | DOC-052 | **P1** — فاز M6 | 15 | 15 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Search/blob/main/ROADMAP.md) |
| 45 | [`Tavaan-Engine-Security`](https://github.com/andrbi106/Tavaan-Engine-Security) | DOC-059 | **P0** — فاز M4 | 11 | 11 | 1 | 1 🔴 | 1/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Security/blob/main/ROADMAP.md) |
| 46 | [`Tavaan-Engine-Session`](https://github.com/andrbi106/Tavaan-Engine-Session) | DOC-041 | **P0** — فاز M2 | 12 | 12 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Session/blob/main/ROADMAP.md) |
| 47 | [`Tavaan-Engine-Tenancy`](https://github.com/andrbi106/Tavaan-Engine-Tenancy) | DOC-082E | **P1** — فاز M6 | 40 | 40 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Tenancy/blob/main/ROADMAP.md) |
| 48 | [`Tavaan-Engine-Test`](https://github.com/andrbi106/Tavaan-Engine-Test) | DOC-084E | **P0** — فاز M8 (اما از M1 استفاده می‌شود) | 22 | 22 | 8 | 9 🔴 | 1/8/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Test/blob/main/ROADMAP.md) |
| 49 | [`Tavaan-Engine-Upgrade`](https://github.com/andrbi106/Tavaan-Engine-Upgrade) | DOC-081E | **P2** — فاز M8 | 16 | 16 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Upgrade/blob/main/ROADMAP.md) |
| 50 | [`Tavaan-Engine-Validation`](https://github.com/andrbi106/Tavaan-Engine-Validation) | DOC-051 | **P0** — فاز M3 | 25 | 25 | 3 | 3 🟡 | 0/3/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Validation/blob/main/ROADMAP.md) |
| 51 | [`Tavaan-Engine-View`](https://github.com/andrbi106/Tavaan-Engine-View) | DOC-043 | **P0** — فاز M2 | 12 | 12 | 1 | 9 🟡 | 0/9/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-View/blob/main/ROADMAP.md) |
| 52 | [`Tavaan-Engine-Workflow`](https://github.com/andrbi106/Tavaan-Engine-Workflow) | DOC-071 | **P2** — فاز M7 | 31 | 31 | 2 | 0 ✅ | 0/0/0 | [ROADMAP](https://github.com/andrbi106/Tavaan-Engine-Workflow/blob/main/ROADMAP.md) |

## ۳. موتورهای دارای شکاف بالا (پیش‌نیاز فوری)

| موتور | شکاف‌های بالا | شرح |
|------|--------------|------|
| [`Tavaan-Engine-Jalali`](https://github.com/andrbi106/Tavaan-Engine-Jalali) | 5 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Crypt`](https://github.com/andrbi106/Tavaan-Engine-Crypt) | 3 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Migration`](https://github.com/andrbi106/Tavaan-Engine-Migration) | 3 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Router`](https://github.com/andrbi106/Tavaan-Engine-Router) | 3 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Schema`](https://github.com/andrbi106/Tavaan-Engine-Schema) | 3 | (شرح در ROADMAP) |
| [`Tavaan-Engine-CORS`](https://github.com/andrbi106/Tavaan-Engine-CORS) | 2 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Cookie`](https://github.com/andrbi106/Tavaan-Engine-Cookie) | 2 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Module`](https://github.com/andrbi106/Tavaan-Engine-Module) | 2 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Observability`](https://github.com/andrbi106/Tavaan-Engine-Observability) | 2 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Optimizer`](https://github.com/andrbi106/Tavaan-Engine-Optimizer) | 2 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Error`](https://github.com/andrbi106/Tavaan-Engine-Error) | 1 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Event`](https://github.com/andrbi106/Tavaan-Engine-Event) | 1 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Log`](https://github.com/andrbi106/Tavaan-Engine-Log) | 1 | (شرح در ROADMAP) |
| [`Tavaan-Engine-ORM`](https://github.com/andrbi106/Tavaan-Engine-ORM) | 1 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Realtime`](https://github.com/andrbi106/Tavaan-Engine-Realtime) | 1 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Scaffold`](https://github.com/andrbi106/Tavaan-Engine-Scaffold) | 1 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Security`](https://github.com/andrbi106/Tavaan-Engine-Security) | 1 | (شرح در ROADMAP) |
| [`Tavaan-Engine-Test`](https://github.com/andrbi106/Tavaan-Engine-Test) | 1 | (شرح در ROADMAP) |

## ۴. موتورهای بدون پیاده‌سازی src (فقط config/manifest)

| موتور | DOC-ID | علت |
|------|--------|------|
| [`Tavaan-Engine-CORS`](https://github.com/andrbi106/Tavaan-Engine-CORS) | DOC-046 | پیاده‌سازی به موتور همسایه منتقل شده (e.g. Router → Http) یا هنوز توسعه نیافته |
| [`Tavaan-Engine-Cookie`](https://github.com/andrbi106/Tavaan-Engine-Cookie) | DOC-042 | پیاده‌سازی به موتور همسایه منتقل شده (e.g. Router → Http) یا هنوز توسعه نیافته |
| [`Tavaan-Engine-Jalali`](https://github.com/andrbi106/Tavaan-Engine-Jalali) | DOC-070 | پیاده‌سازی به موتور همسایه منتقل شده (e.g. Router → Http) یا هنوز توسعه نیافته |
| [`Tavaan-Engine-ORM`](https://github.com/andrbi106/Tavaan-Engine-ORM) | DOC-050 | پیاده‌سازی به موتور همسایه منتقل شده (e.g. Router → Http) یا هنوز توسعه نیافته |
| [`Tavaan-Engine-Router`](https://github.com/andrbi106/Tavaan-Engine-Router) | DOC-040 | پیاده‌سازی به موتور همسایه منتقل شده (e.g. Router → Http) یا هنوز توسعه نیافته |
| [`Tavaan-Engine-Schema`](https://github.com/andrbi106/Tavaan-Engine-Schema) | DOC-048 | پیاده‌سازی به موتور همسایه منتقل شده (e.g. Router → Http) یا هنوز توسعه نیافته |

## ۵. توصیه‌های کلی

1. **اولویت ۱ — موتورهای بدون src:** برای موتورهای `Tavaan-Engine-Router`، `Tavaan-Engine-CORS`، `Tavaan-Engine-Cookie`، `Tavaan-Engine-Jalali`، `Tavaan-Engine-ORM`، `Tavaan-Engine-Schema` که فایل `src/` خالی دارند، بررسی کنید که آیا پیاده‌سازی در موتور همسایه (مثل Http) قرار گرفته یا واقعاً ناقص است. در صورت انتقال، رفرنس‌های `module.json` را به‌روز کنید.

2. **اولویت ۲ — تست‌های ناقص:** موتورهایی که سناریوهای تست زیادی در مستندات دارند ولی تست کمی موجود است (مثل `Tavaan-Engine-Test` با ۹ شکاف، `Tavaan-Engine-View` با ۹ شکاف)، نیاز به افزایش پوشش تست دارند.

3. **اولویت ۳ — کلاس‌های ناقص:** موتورهایی که شکاف method دارند (مثل `Http`، `I18n`، `Validation`، `Mail`)، باید API عمومی مستندات را کامل‌تر پیاده‌سازی کنند.

4. **پایداری:** هر تغییری در API عمومی موتور باید با به‌روزرسانی بلوک YAML `public_api` در مستندات همراه باشد تا در ران بعدی این تحلیل، شکاف‌ها به‌روز شوند.

## ۶. روش تولید

این نقشه‌های راه توسط اسکریپت `scripts/compare_engines.py` تولید شده‌اند که:

1. بلوک YAML ماشین‌خوان (`# machine-readable`) هر سند موتور را parse می‌کند و `public_api`, `tables`, `drivers`, `acceptance_criteria` را استخراج می‌کند.
2. سناریوهای تست (T-NN) و معیارهای پذیرش (AC-XXX-NN) را از بدنهٔ سند استخراج می‌کند.
3. فایل‌های `src/**/*.php`، `tests/**/*.php`، `config/` و `migrations/` موتور را اسکن می‌کند و کلاس‌ها و متدهای عمومی واقعی را شناسایی می‌کند.
4. چهار نوع شکاف را شناسایی می‌کند:
   - `missing_class` (🔴 بالا) — کلاس در `public_api` مستندات هست ولی پیاده‌سازی ندارد.
   - `missing_method` (🟡 متوسط) — متد در کلاس موجود نیست.
   - `missing_migrations` (🔴 بالا) — جدول در مستندات هست ولی migration ندارد.
   - `missing_tests` (🔴 بالا) — سناریو تست در مستندات هست ولی فایل تستی وجود ندارد.
   - `partial_tests` (🟡 متوسط) — پوشش تست ناکافی.
   - `loc_underestimate` (🟢 پایین) — LOC واقعی به‌طور قابل‌توجهی کمتر از تخمین است.
5. برای هر شکاف، وظیفه (`TASK-NN`) با گام‌های مشخص در `ROADMAP.md` تولید می‌شود.

## ۷. منابع

- مخزن مستندات: [Derogaramin/Tavaan-Doc](https://github.com/Derogaramin/Tavaan-Doc)
- رجیستری موتورها: [DOC-030](https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/README.md)
- مخزن مرجع تفکیک: [andrbi106/Tavaan](https://github.com/andrbi106/Tavaan)

---
*این سند توسط Tavaan Doc-Comparator در 2026-11-03 05:42:12 UTC تولید شده است.*