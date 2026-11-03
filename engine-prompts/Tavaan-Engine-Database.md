# پرامپت پیاده‌سازی موتور Tavaan-Engine-Database

> این پرامپت به‌صورت خودکار تولید شده و تمام اطلاعات لازم برای پیاده‌سازی مستقل موتور را گردآوری می‌کند.
> تاریخ تولید: **2026-11-03 09:28:10 UTC**

## ۱. آدرس مخازن مرتبط

| نوع | URL |
|-----|-----|
| مخزن اصلی (source framework) | `https://github.com/Derogaramin/Tavaan-Framework` |
| مخزن هدف (split meta-repo) | `https://github.com/andrbi106/Tavaan` |
| مخزن مستندات | `https://github.com/Derogaramin/Tavaan-Doc` |
| مخزن این موتور | `https://github.com/andrbi106/Tavaan-Engine-Database` |
| سند موتور | [`docs/03-engines/database.md`](https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/database.md) |
| فایل ROADMAP موتور | [`ROADMAP.md`](https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/ROADMAP.md) |
| فایل TICKET موتور | [`TICKET.md`](https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/TICKET.md) |
| فایل module.json | [`module.json`](https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/module.json) |

## ۲. زمینه و شناسه‌ها

| فیلد | مقدار |
|------|------|
| نام مخزن | `Tavaan-Engine-Database` |
| Engine ID | `tavaan.engine.database` |
| DOC-ID | `DOC-047` |
| Namespace | `Tavaan\Engine\Database` |
| اولویت | P0 |
| فاز | M3 |
| Facade | `DB` (accessor: `db`) |
| تخمین LOC | 3200 |
| وابستگی‌های سخت (depends_on) | `config`, `event`, `log` |
| وابستگی‌های نرم (soft_depends_on) | — |

## ۳. درخواست

برای مخزن `Tavaan-Engine-Database` یک پیاده‌سازی کامل، خودبسنده و سازگار با مستندات از موتور **Database** بساز.

این موتور در فریمورک Tavaan نقش زیر را بر عهده دارد:

> لایهٔ دادهٔ صفر‌وابستگی: مدیریت اتصال، **Query Builder** کامل، **Grammar** مخصوص هر درایور،
> تراکنش با Savepoint، Query Log، Read/Write Splitting و Pooling برای Resident.
> - ✅ اتصال Lazy با Reconnect خودکار
> - ✅ Query Builder: Select/Join/SubQuery/Union/CTE/Aggregate/Window/Lock

### خروجی‌های مورد انتظار

پیاده‌سازی باید این هفت قلم الزامی (طبق قاعده R6 فریمورک) را داشته باشد:

1. **Provider** در `src/<Name>ServiceProvider.php`
2. **Contract** در `core/Contracts/<Area>/*Interface.php`
3. **پیاده‌سازی** در `src/**`
4. **Config** در `config/<name>.php`
5. **Lang** در `lang/{fa,en}/<name>.php`
6. **Tests** در `tests/{Unit,Feature,Benchmark}`
7. **Docs + Manifest** در مستندات + `module.json`

## ۴. مراجع حیاتی

### ۴.۱ فایل ROADMAP.md

فایل [`ROADMAP.md`](https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/ROADMAP.md) این موتور قبلاً با تحلیل شکاف بین مستندات و پیاده‌سازی فعلی تولید شده است.
این فایل شامل این بخش‌هاست:

- بخش ۱: مرجع مستندات (DOC-ID, namespace, facade, LOC target)
- بخش ۲: خلاصه وضعیت فعلی (تعداد فایل‌های src, tests, migrations)
- بخش ۳: شکاف‌های شناسایی‌شده با اولویت 🔴 بالا / 🟡 متوسط / 🟢 پایین
- بخش ۴: API عمومی مورد انتظار (لیست کلاس‌ها و متدها)
- بخش ۵: سناریوهای تست مورد انتظار (T-NN)
- بخش ۶: معیارهای پذیرش (AC-XXX-NN)
- بخش ۹: نقشه راه تکمیل با TASK-NN

**پیش از شروع کار، حتماً بخش ۳ و ۹ از ROADMAP.md را مطالعه کنید.**

### ۴.۲ فایل TICKET.md

فایل [`TICKET.md`](https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/TICKET.md) حاوی تیکت‌های توسعهٔ تیکت‌محور موتور است. این فایل شامل:

- شناسه موتور (مثلاً `tavaan.engine.cache`)
- نسخه، namespace
- آمار واقعی: تعداد فایل‌ها و خطوط کد فعلی
- تیکت‌های مرتبط (مثلاً `TVN-0060`) با فاز، اولویت، وضعیت، پیش‌نیازها و برآورد LOC

### ۴.۳ مستندات کامل موتور

سند کامل: [`docs/03-engines/database.md`](https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/database.md)

این سند شامل این بخش‌های کلیدی است که باید خط‌به‌خط پیاده‌سازی شوند:

1. هدف موتور
2. معماری (با دیاگرام)
3. API تعریف و نحوه استفاده
4. الگوریتم‌ها (در صورت وجود)
5. پیکربندی (`config/<name>.php`)
6. امنیت (🔒 — تهدیدها و کنترل‌ها)
7. کارایی (اهداف عملکردی)
8. تست (سناریوهای T-NN)
9. معیار پذیرش (AC-XXX-NN)
10. مراجع (منابع الهام و تفاوت‌ها)
11. بلوک YAML ماشین‌خوان (در انتهای سند)

## ۵. API عمومی مورد انتظار

### کلاس `QueryBuilder`

```php
namespace Tavaan\Engine\Database;

class QueryBuilder
{
    public function table(/* ... */): mixed { /* ... */ }
    public function select(/* ... */): mixed { /* ... */ }
    public function selectRaw(/* ... */): mixed { /* ... */ }
    public function from(/* ... */): mixed { /* ... */ }
    public function join(/* ... */): mixed { /* ... */ }
    public function leftJoin(/* ... */): mixed { /* ... */ }
    public function rightJoin(/* ... */): mixed { /* ... */ }
    public function crossJoin(/* ... */): mixed { /* ... */ }
    public function where(/* ... */): mixed { /* ... */ }
    public function orWhere(/* ... */): mixed { /* ... */ }
    public function whereIn(/* ... */): mixed { /* ... */ }
    public function whereNull(/* ... */): mixed { /* ... */ }
    public function whereBetween(/* ... */): mixed { /* ... */ }
    public function whereExists(/* ... */): mixed { /* ... */ }
    public function whereRaw(/* ... */): mixed { /* ... */ }
    public function groupBy(/* ... */): mixed { /* ... */ }
    public function having(/* ... */): mixed { /* ... */ }
    public function orderBy(/* ... */): mixed { /* ... */ }
    public function limit(/* ... */): mixed { /* ... */ }
    public function offset(/* ... */): mixed { /* ... */ }
    public function forUpdate(/* ... */): mixed { /* ... */ }
    public function sharedLock(/* ... */): mixed { /* ... */ }
    public function union(/* ... */): mixed { /* ... */ }
    public function withCte(/* ... */): mixed { /* ... */ }
    public function toSql(/* ... */): mixed { /* ... */ }
    public function getBindings(/* ... */): mixed { /* ... */ }
    public function get(/* ... */): mixed { /* ... */ }
    public function cursor(/* ... */): mixed { /* ... */ }
    public function first(/* ... */): mixed { /* ... */ }
    public function find(/* ... */): mixed { /* ... */ }
    public function value(/* ... */): mixed { /* ... */ }
    public function pluck(/* ... */): mixed { /* ... */ }
    public function count(/* ... */): mixed { /* ... */ }
    public function sum(/* ... */): mixed { /* ... */ }
    public function avg(/* ... */): mixed { /* ... */ }
    public function min(/* ... */): mixed { /* ... */ }
    public function max(/* ... */): mixed { /* ... */ }
    public function exists(/* ... */): mixed { /* ... */ }
    public function insert(/* ... */): mixed { /* ... */ }
    public function insertGetId(/* ... */): mixed { /* ... */ }
    public function insertOrIgnore(/* ... */): mixed { /* ... */ }
    public function upsert(/* ... */): mixed { /* ... */ }
    public function update(/* ... */): mixed { /* ... */ }
    public function increment(/* ... */): mixed { /* ... */ }
    public function decrement(/* ... */): mixed { /* ... */ }
    public function delete(/* ... */): mixed { /* ... */ }
    public function truncate(/* ... */): mixed { /* ... */ }
    public function paginate(/* ... */): mixed { /* ... */ }
    public function chunk(/* ... */): mixed { /* ... */ }
    public function lazy(/* ... */): mixed { /* ... */ }
}
```

متدهای مورد انتظار (50 مورد):

`table()`, `select()`, `selectRaw()`, `from()`, `join()`, `leftJoin()`, `rightJoin()`, `crossJoin()`, `where()`, `orWhere()`, `whereIn()`, `whereNull()`, `whereBetween()`, `whereExists()`, `whereRaw()`, `groupBy()`, `having()`, `orderBy()`, `limit()`, `offset()`, `forUpdate()`, `sharedLock()`, `union()`, `withCte()`, `toSql()`, `getBindings()`, `get()`, `cursor()`, `first()`, `find()`, `value()`, `pluck()`, `count()`, `sum()`, `avg()`, `min()`, `max()`, `exists()`, `insert()`, `insertGetId()`, `insertOrIgnore()`, `upsert()`, `update()`, `increment()`, `decrement()`, `delete()`, `truncate()`, `paginate()`, `chunk()`, `lazy()`

### کلاس `Connection`

```php
namespace Tavaan\Engine\Database;

class Connection
{
    public function select(/* ... */): mixed { /* ... */ }
    public function selectOne(/* ... */): mixed { /* ... */ }
    public function cursor(/* ... */): mixed { /* ... */ }
    public function insert(/* ... */): mixed { /* ... */ }
    public function update(/* ... */): mixed { /* ... */ }
    public function delete(/* ... */): mixed { /* ... */ }
    public function statement(/* ... */): mixed { /* ... */ }
    public function affectingStatement(/* ... */): mixed { /* ... */ }
    public function lastInsertId(/* ... */): mixed { /* ... */ }
    public function transaction(/* ... */): mixed { /* ... */ }
    public function beginTransaction(/* ... */): mixed { /* ... */ }
    public function commit(/* ... */): mixed { /* ... */ }
    public function rollBack(/* ... */): mixed { /* ... */ }
    public function transactionLevel(/* ... */): mixed { /* ... */ }
    public function pdo(/* ... */): mixed { /* ... */ }
    public function queryLog(/* ... */): mixed { /* ... */ }
}
```

متدهای مورد انتظار (16 مورد):

`select()`, `selectOne()`, `cursor()`, `insert()`, `update()`, `delete()`, `statement()`, `affectingStatement()`, `lastInsertId()`, `transaction()`, `beginTransaction()`, `commit()`, `rollBack()`, `transactionLevel()`, `pdo()`, `queryLog()`

## ۶. سناریوهای تست مورد انتظار

| ID | سناریو |
|----|--------|
| `T-01` | اتصال Lazy (PDO تا اولین کوئری ساخته نمی‌شود) |
| `T-02` | Reconnect پس از «gone away» |
| `T-03` | همهٔ Builder clauseها → SQL درست (MySQL/PG/SQLite) |
| `T-04` | Prepared binding با null/bool/int/string/DateTime |
| `T-05` | Nested transaction با Savepoint |
| `T-06` | Deadlock → retry (با Mock) |
| `T-07` | Chunk با توقف در callback |
| `T-08` | Cursor/Lazy حافظه ثابت نگه می‌دارد |
| `T-09` | Upsert در هر ۳ درایور |
| `T-10` | SQL Injection Fuzzing (۲۰۰ payload) → همه fail |
| `T-11` | `whereRaw` با binding کاربر → امن |
| `T-12` | Read/Write splitting + sticky |
| `T-13` | Query Log + Slow detection |
| `T-14` | N+1 detection |
| `T-15` | Pagination (Page/Cursor/Keyset) |

هر سناریو باید به یک متد `test<Scenario>` در `tests/Feature/<Engine>Test.php` تبدیل شود.

## ۷. معیارهای پذیرش (Acceptance Criteria)

- `AC-DB-01`
- `AC-DB-02`
- `AC-DB-03`
- `AC-DB-04`
- `AC-DB-05`

پیاده‌سازی تا زمان برآورده شدن همهٔ معیارهای پذیرش بالا کامل نشده است.

## ۱۰. فایل پیکربندی

فایل پیکربندی باید در `config/database.php` ساخته شود و تمام کلیدهای مستندشده در سند را شامل شود.

## ۱۱. الزامات امنیتی 🔒

| تهدید | کنترل |
| SQL Injection | Prepared Statement ۱۰۰٪؛ `EMULATE_PREPARES=false` |
| Injection از `whereRaw`/`orderByRaw` | فقط با binding؛ allowlist برای sort field |
| Identifier Injection | `wrap()` با escape `` ` `` و ممنوعیت ورودی کاربر |
| Mass Data Leak | `limit` پیش‌فرض در `get()` (اختیاری)، Slow query alert |
| Deadlock Storm | retry محدود + backoff |
| نشت credential | فقط از config/ENV؛ mask در لاگ |
| Second-Order Injection | داده از DB هم قبل از `whereRaw` escape شود |
```php
private function assertNoUserInputInRaw(string $sql, string $context): void
{
    // 🔒 اگر raw با متغیر request ساخته شده، باید binding داشته باشد
    if (\preg_match('/[\$](?:_GET|_POST|_REQUEST|_COOKIE)/', $sql) === 1) {
        throw new UnsafeQueryException(messageId: 'database.unsafe_raw', context: ['context' => $context]);
    }
}
```
---

🔒 هر گزینه امنیتی با علامت 🔒 در مستندات، یک الزام سخت پیاده‌سازی است و نباید نادیده گرفته شود.

## ۱۲. اهداف کارایی

| عملیات | هدف |
| ساخت Connection (اولین) | ≤ ۱۵ms (MySQL local) |
| `table()->where()->get()` با ۱۰۰ رکورد | ≤ ۵ms |
| Compile SQL (builder با ۸ جزء) | ≤ ۳۰µs |
| Prepared statement reuse | ≥ ۲۰٪ سریع‌تر از prepare هر بار |
| Chunk ۱۰۰۰ رکورد (۵۰۰‌تایی) | حافظه ≤ ۵MB |
| Cursor روی ۱۰۰٬۰۰۰ رکورد | حافظه ≤ ۲MB |
| Query Log overhead (فعال) | ≤ ۵٪ |

این اهداف باید با تست‌های Benchmark در `tests/Benchmark/` تأیید شوند.

## ۱۳. نحوه پیاده‌سازی موتور به‌صورت مستقل (بدون وابستگی به سایر موتورها)

### ۱۳٫۱ اصل استقلال

هر موتور باید **کاملاً مستقل** پیاده‌سازی شود. به این معنا که:

1. هیچ `use` از namespace موتورهای دیگر نباید در کد باشد (مثلاً `use Tavaan\Engine\Cache\CacheManager` در موتور Auth ممنوع است).
2. وابستگی‌ها فقط از طریق **Contract** (اینترفیس) در `core/Contracts/` تزریق شوند، نه از طریق کلاس‌های سخت.
3. ارتباط با سایر موتورها فقط از طریق **Service Container** و **Event** باشد.
4. کلاس‌های کمکی (مثل `ArrayStore`، `FileStore`) به‌صورت داخلی در همان موتور پیاده‌سازی شوند.

### ۱۳٫۲ الگوی Service Provider

هر موتور یک `<Name>ServiceProvider` دارد که در `module.json` تحت `providers` ثبت شده. این کلاس باید:

1. در متد `register()` سرویس‌های موتور را در Container ثبت کند.
2. در متد `boot()` Facadeها، Middlewareها و Commandهای console را ثبت کند.
3. Contractها را به پیاده‌سازی‌های مربوطه bind کند.
4. هیچ وابستگی به موتورهای دیگر را به‌صورت سخت (hard-coded) نداشته باشد.

```php
<?php
declare(strict_types=1);

namespace Tavaan\Engine\Database;

use Tavaan\Core\Contracts\Container\ContainerInterface;
use Tavaan\Core\Provider\ServiceProvider;

class DatabaseServiceProvider extends ServiceProvider
{
    public function register(): void
    {
        $this->app->singleton(/* ... */, function (ContainerInterface $app) {
            // فقط وابستگی‌های اصلی از طریق Contract
            return /* ... */;
        });
    }

    public function boot(): void
    {
        $this->registerFacade();
        $this->registerCommands();
        $this->registerMiddleware();
    }
}
```

### ۱۳٫۳ مدیریت وابستگی‌ها

**وابستگی‌های سخت (required):**

- `config`: به‌صورت Contract از Container تزریق شود.
- `event`: به‌صورت Contract از Container تزریق شود.
- `log`: به‌صورت Contract از Container تزریق شود.

الگوی preditional binding برای وابستگی نرم:

```php
if ($this->app->bound(/* Contract */)) {
    // از پیاده‌سازی موجود استفاده کن
} else {
    // fallback داخلی
}
```

### ۱۳٫۴ فایل پیکربندی

یک فایل `config/database.php` با تمام کلیدهای مستندشده بسازید. مثال ساختار:

```php
<?php
declare(strict_types=1);

return [
    'default' => env('DATABASE_DEFAULT', 'file'),
    'stores' => [
        // ...
    ],
    // سایر کلیدهای مستندشده در سند بخش ۶ (پیکربندی)
];
```

### ۱۳٫۶ تست‌ها

برای هر سناریو T-NN در مستندات، یک متد تست در `tests/Feature/<Engine>Test.php` بسازید.
الگو:

```php
<?php
declare(strict_types=1);

namespace Tavaan\Engine\Database\Tests\Feature;

use PHPUnit\Framework\TestCase;
use Tavaan\Engine\Database\<Manager>;

class DatabaseTest extends TestCase
{
    protected function setUp(): void { /* ... */ }

    public function testT01_<scenario_snake>(): void
    {
        // شرط سناریوی T-01 از مستندات
        $this->/* assertion */;
    }

    // ... سایر T-NN
}
```

### ۱۳٫۷ فایل‌های زبان

برای هر کلید ترجمهٔ مستندشده، فایل‌های `lang/fa/<engine>.php` و `lang/en/<engine>.php` بسازید.
ساختار:

```php
<?php
return [
    'error_message_key' => 'متن فارسی',
    // ...
];
```

### ۱۳٫۸ README.md اختصاصی

یک `README.md` کوتاه و واضح در ریشه موتور بنویسید که شامل:

- نام موتور و کارکرد یک‌خطی
- نمونه کد استفاده
- لیست وابستگی‌ها
- نحوه اجرای تست‌ها (`php bin/tvn test engines/<name>`)
- لینک به مستندات کامل

## ۱۴. گردش کار پیاده‌سازی پیشنهادی

1. **مطالعهٔ کامل مستندات:** تمام بخش‌های سند `docs/03-engines/{doc_key}.md` را بخوانید، به‌ویژه بخش‌های API، تست و معیار پذیرش.
2. **بررسی ROADMAP.md:** شکاف‌های شناسایی‌شده و TASK-NN را مرور کنید تا بدانید چه چیزی باید تکمیل شود.
3. **بررسی TICKET.md:** تیکت‌های مرتبط (TVN-NNNN) و پیش‌نیازها را بررسی کنید.
4. **پیاده‌سازی به ترتیب:**
   a. `module.json` را به‌روز کنید (نه `autoload` به مسیر خارجی)
   b. `config/<name>.php` را بسازید
   c. `src/Contracts/*Interface.php` را تعریف کنید
   d. `src/<Name>ServiceProvider.php` را بسازید
   e. پیاده‌سازی‌های اصلی (`src/<Manager>.php` و کلاس‌های وابسته)
   f. درایورها / Storeها / Adapterها
   g. Migrationها (در صورت وجود جدول)
   h. Commandهای Console (در صورت وجود `commands` در module.json)
   i. Middlewareها (در صورت نیاز)
   j. Facade (در صورت وجود)
5. **نوشتن تست‌ها:** برای هر T-NN یک متد `testTNN_*` در `tests/Feature/`.
6. **نوشتن README.md** اختصاصی موتور.
7. **اجرا و تأیید:** `php bin/tvn test engines/<name>` و `php bin/tvn engine:validate`.
8. **کامیت و پوش:** هر مرحله به‌صورت commit مستقل با پیام روشن (`feat(<engine>): <short desc>`).
9. **به‌روزرسانی ROADMAP.md:** پس از تکمیل، بخش ۲ و ۳ را به‌روز کنید و TASK-NN انجام‌شده را علامت بزنید.

## ۱۵. محدودیت‌ها و اصول سخت (Hard Constraints)

1. **PHP 8.2+**: فقط با قابلیت‌های PHP 8.2+ (readonly classes, enums, first-class callable syntax, ...).
2. **صفر وابستگی Composer خارجی**: هیچ `require` در `composer.json` به جز `php >= 8.2` و ابزارهای dev.
3. **PSR-4 Autoloading**: namespace در `module.json` با مسیر `src/` هماهنگ باشد.
4. **Strict types**: همهٔ فایل‌های PHP با `declare(strict_types=1);` شروع شوند.
5. **Type Hints کامل**: هر متد必须有 return type و parameter types.
6. **جنس strictly نهایی**: کلاس‌های نهایی `final`، کلاس‌های انتزاعی `abstract`.
7. **اسم متدها**: camelCase با معنای روشن، بدون مخفف.
8. **آماده بودن برای PHPStan**: کد باید با `phpstan analyse --level=max` بدون خطا عبور کند.
9. **آماده بودن برای php-cs-fixer**: با `php bin/tvn cs` هماهنگ باشد.
10. **هیچ `echo`/`var_dump`/`die` در کد نهایی**: خطایابی با `log` و exception.
11. **هر خطای قابل پیش‌بینی به‌صورت Exception خالص**: نه warning، نه notice.
12. **تست‌های واقعی**: نه mock-fest — وقتی موتور می‌تواند با In-Memory پیاده‌سازی واقعی تست شود، حتماً این کار انجام شود.

## ۱۶. چک‌لیست تأیید نهایی

پیش از اعلام اتمام، همهٔ این موارد باید برآورده شوند:

- [ ] تمام متدهای `public_api` در مستندات پیاده‌سازی شده‌اند.
- [ ] تمام سناریوهای T-NN به‌صورت متد تست با assert واقعی موجودند.
- [ ] تمام AC-XXX-NN برآورده شده‌اند.
- [ ] تمام جداول مستندشده در `migrations/` موجودند.
- [ ] فایل `config/<name>.php` تمام کلیدهای مستندشده را دارد.
- [ ] `module.json` به‌روز شده و `autoload` به `src/` محلی اشاره می‌کند.
- [ ] هیچ `use` از سایر موتورها در کد نیست.
- [ ] تمام فایل‌ها `declare(strict_types=1);` دارند.
- [ ] README.md اختصاصی موتور نوشته شده.
- [ ] `php bin/tvn test engines/<name>` بدون خطا عبور می‌کند.
- [ ] `php bin/tvn engine:validate` بدون خطا عبور می‌کند.
- [ ] `php bin/tvn stan` (PHPStan) بدون خطا.
- [ ] `php bin/tvn cs:check` بدون خطا.

## ۱۷. منابع نهایی

- مستندات: https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/database.md
- ROADMAP موتور: https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/ROADMAP.md
- TICKET موتور: https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/TICKET.md
- module.json: https://github.com/andrbi106/Tavaan-Engine-Database/blob/main/module.json
- مخزن موتور: https://github.com/andrbi106/Tavaan-Engine-Database
- مخزن اصلی فریمورک: https://github.com/Derogaramin/Tavaan-Framework
- مخزن مستندات: https://github.com/Derogaramin/Tavaan-Doc
- مخزن تفکیک (meta): https://github.com/andrbi106/Tavaan
- رجیستری موتورها: https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/README.md

---
*این پرامپت توسط Tavaan Engine Prompt Generator در 2026-11-03 09:28:10 UTC تولید شده است.*