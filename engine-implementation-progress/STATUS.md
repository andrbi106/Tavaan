# وضعیت پیاده‌سازی ۵۲ موتور — Status

> آخرین به‌روزرسانی: **2026-11-03**

## خلاصه کلان

| شاخص | مقدار |
|------|------|
| موتورهای با منطق واقعی | **8 / 52** |
| موتورهای با scaffold | 44 |
| **مجموع LOC** | **8280** |
| فاز فعلی | Level 2 (بخشی) |
| گام بعدی | ادامه Level 2 (Event, I18n, Module, Console, Filesystem, ...) |

## پیشرفت بر اساس سطح

| سطح | تعداد موتور | تکمیل‌شده | وضعیت |
|------|-------------|------------|--------|
| 0 | 3 | 3 | ✅ تمام شد |
| 1 | 2 | 2 | ✅ تمام شد |
| 2 | 11 | 3 | 🟡 بخشی |
| 3 | 11 | 0 | در انتظار |
| 4 | 5 | 0 | در انتظار |
| 5 | 7 | 0 | در انتظار |
| 6 | 1 | 0 | در انتظار |
| 7 | 1 | 0 | در انتظار |
| 8 | 1 | 0 | در انتظار |

## موتورهای تکمیل‌شده با منطق واقعی

### Level 0

| # | موتور | Repository | LOC | Commit |
|---|-------|------------|-----|--------|
| 1 | Compat | [`Tavaan-Engine-Compat`](https://github.com/andrbi106/Tavaan-Engine-Compat) | 1366 | `9851c92` |
| 2 | Container | [`Tavaan-Engine-Container`](https://github.com/andrbi106/Tavaan-Engine-Container) | 1385 | `be3189e` |
| 3 | Test | [`Tavaan-Engine-Test`](https://github.com/andrbi106/Tavaan-Engine-Test) | 1117 | `b43e4f9` |

### Level 1

| # | موتور | Repository | LOC | Commit |
|---|-------|------------|-----|--------|
| 1 | Config | [`Tavaan-Engine-Config`](https://github.com/andrbi106/Tavaan-Engine-Config) | 1321 | `fa418c1` |
| 2 | Pipeline | [`Tavaan-Engine-Pipeline`](https://github.com/andrbi106/Tavaan-Engine-Pipeline) | 618 | `56c3064` |

### Level 2 (بخشی)

| # | موتور | Repository | LOC | Commit |
|---|-------|------------|-----|--------|
| 1 | Hash | [`Tavaan-Engine-Hash`](https://github.com/andrbi106/Tavaan-Engine-Hash) | 432 | `8266a90` |
| 2 | Crypt | [`Tavaan-Engine-Crypt`](https://github.com/andrbi106/Tavaan-Engine-Crypt) | 834 | `6dea968` |
| 3 | Log | [`Tavaan-Engine-Log`](https://github.com/andrbi106/Tavaan-Engine-Log) | 1207 | `ff3d785` |

## گزارش‌های تفصیلی

- [Level 0 Report](./LEVEL-0-REPORT.md) — 3868 LOC
- [Level 1 Report](./LEVEL-1-REPORT.md) — 1939 LOC
- [Level 2 Partial Report](./LEVEL-2-PARTIAL-REPORT.md) — 2473 LOC

## موتورهای Level 2 باقی‌مانده (برای نشست بعدی)

| # | موتور | اولویت | وابستگی‌ها |
|---|-------|--------|------------|
| 1 | Event | P0 | `container`, `config` |
| 2 | I18n | P0 | `config` |
| 3 | Module | P0 | `container`, `config` |
| 4 | Console | P1 | `container`, `config` |
| 5 | Filesystem | P1 | `config` |
| 6 | Media | P1 | `config` |
| 7 | Search | P1 | `config` |
| 8 | Tenancy | P1 | `config` |

---
*Generated on 2026-11-03.*
