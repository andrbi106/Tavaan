# پرامپت پیاده‌سازی موتور Tavaan-Engine-Container

> این پرامپت به‌صورت خودکار تولید شده و تمام اطلاعات لازم برای پیاده‌سازی مستقل موتور را گردآوری می‌کند.
> تاریخ تولید: **2026-11-03 09:28:10 UTC**

## ۱. آدرس مخازن مرتبط

| نوع | URL |
|-----|-----|
| مخزن اصلی (source framework) | `https://github.com/Derogaramin/Tavaan-Framework` |
| مخزن هدف (split meta-repo) | `https://github.com/andrbi106/Tavaan` |
| مخزن مستندات | `https://github.com/Derogaramin/Tavaan-Doc` |
| مخزن این موتور | `https://github.com/andrbi106/Tavaan-Engine-Container` |
| سند موتور | [`docs/03-engines/container.md`](https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/container.md) |
| فایل ROADMAP موتور | [`ROADMAP.md`](https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/ROADMAP.md) |
| فایل TICKET موتور | [`TICKET.md`](https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/TICKET.md) |
| فایل module.json | [`module.json`](https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/module.json) |

## ۲. زمینه و شناسه‌ها

| فیلد | مقدار |
|------|------|
| نام مخزن | `Tavaan-Engine-Container` |
| Engine ID | `tavaan.engine.container` |
| DOC-ID | `DOC-031` |
| Namespace | `Tavaan\Engine\Container` |
| اولویت | P0 |
| فاز | M1 |
| Facade | `—` (accessor: `—`) |
| تخمین LOC | 1200 |
| وابستگی‌های سخت (depends_on) | — |
| وابستگی‌های نرم (soft_depends_on) | — |

## ۳. درخواست

برای مخزن `Tavaan-Engine-Container` یک پیاده‌سازی کامل، خودبسنده و سازگار با مستندات از موتور **Container** بساز.

این موتور در فریمورک Tavaan نقش زیر را بر عهده دارد:

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

فایل [`ROADMAP.md`](https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/ROADMAP.md) این موتور قبلاً با تحلیل شکاف بین مستندات و پیاده‌سازی فعلی تولید شده است.
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

فایل [`TICKET.md`](https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/TICKET.md) حاوی تیکت‌های توسعهٔ تیکت‌محور موتور است. این فایل شامل:

- شناسه موتور (مثلاً `tavaan.engine.cache`)
- نسخه، namespace
- آمار واقعی: تعداد فایل‌ها و خطوط کد فعلی
- تیکت‌های مرتبط (مثلاً `TVN-0060`) با فاز، اولویت، وضعیت، پیش‌نیازها و برآورد LOC

### ۴.۳ مستندات کامل موتور

سند کامل: [`docs/03-engines/container.md`](https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/container.md)

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

### کلاس `Container`

```php
namespace Tavaan\Engine\Container;

class Container
{
    public function bind(/* ... */): mixed { /* ... */ }
    public function singleton(/* ... */): mixed { /* ... */ }
    public function scoped(/* ... */): mixed { /* ... */ }
    public function factory(/* ... */): mixed { /* ... */ }
    public function instance(/* ... */): mixed { /* ... */ }
    public function alias(/* ... */): mixed { /* ... */ }
    public function tag(/* ... */): mixed { /* ... */ }
    public function tagged(/* ... */): mixed { /* ... */ }
    public function when(/* ... */): mixed { /* ... */ }
    public function extend(/* ... */): mixed { /* ... */ }
    public function make(/* ... */): mixed { /* ... */ }
    public function get(/* ... */): mixed { /* ... */ }
    public function has(/* ... */): mixed { /* ... */ }
    public function call(/* ... */): mixed { /* ... */ }
    public function lazy(/* ... */): mixed { /* ... */ }
    public function flush(/* ... */): mixed { /* ... */ }
    public function flushScoped(/* ... */): mixed { /* ... */ }
    public function forgetInstance(/* ... */): mixed { /* ... */ }
    public function bindings(/* ... */): mixed { /* ... */ }
    public function dependencyGraph(/* ... */): mixed { /* ... */ }
    public function stats(/* ... */): mixed { /* ... */ }
}
```

متدهای مورد انتظار (21 مورد):

`bind()`, `singleton()`, `scoped()`, `factory()`, `instance()`, `alias()`, `tag()`, `tagged()`, `when()`, `extend()`, `make()`, `get()`, `has()`, `call()`, `lazy()`, `flush()`, `flushScoped()`, `forgetInstance()`, `bindings()`, `dependencyGraph()`, `stats()`

## ۶. سناریوهای تست مورد انتظار

| ID | سناریو |
|----|--------|
| `T-01` | Singleton دو بار make → یک نمونه |
| `T-02` | Transient دو بار → دو نمونه |
| `T-03` | Auto-wire ۵ سطح تو‌در‌تو |
| `T-04` | چرخه A→B→A |
| `T-05` | Union `(A&B)\ |
| `T-06` | پارامتر با default و بدون type + `strict.allow_untyped=false` |
| `T-07` | Contextual برای دو مصرف‌کننده |
| `T-08` | `tagged()` lazy (بدون make تا iterate) |
| `T-09` | `extend()` دو بار → زنجیرهٔ decorator |
| `T-10` | `flushScoped()` → singleton باقی، scoped حذف |
| `T-11` | Variadic parameter |
| `T-12` | Promoted readonly property |
| `T-13` | Enum injection با default |
| `T-14` | `call()` روی static method |
| `T-15` | Reflection Cache dump/load → نتیجه یکسان |

هر سناریو باید به یک متد `test<Scenario>` در `tests/Feature/<Engine>Test.php` تبدیل شود.

## ۷. معیارهای پذیرش (Acceptance Criteria)

- `AC-CON-01`
- `AC-CON-02`
- `AC-CON-03`
- `AC-CON-04`
- `AC-CON-05`
- `AC-CON-06`

پیاده‌سازی تا زمان برآورده شدن همهٔ معیارهای پذیرش بالا کامل نشده است.

## ۱۰. فایل پیکربندی

فایل پیکربندی باید در `engines/container/config/container.php` ساخته شود و تمام کلیدهای مستندشده در سند را شامل شود.

## ۱۱. الزامات امنیتی 🔒

| تهدید | کنترل |
| تزریق کلاس دلخواه از ورودی کاربر به `make()` | 🔒 `make()` با abstract از ورودی کاربر ممنوع → `assertSafeAbstract()` |
| DoS با چرخهٔ عمیق | CycleDetector + `max_depth = 32` |
| Memory Exhaust با Singletonهای بزرگ | `stats()` + هشدار در Debug Bar |
| نشت سرویس Request در Resident | `flushScoped()` در terminate |
```php
private function assertSafeAbstract(string $abstract): void
{
    if (!\class_exists($abstract) && !\interface_exists($abstract) && !$this->bound($abstract)) {
        throw BindingResolutionException::notFound($abstract);
    }
    if (\str_contains($abstract, "\0") || \strlen($abstract) > 300) {
        throw BindingResolutionException::unsafe($abstract);
    }
}
```
🔒 هرگز `$container->make($_GET['class'])` — در `security-policy` هم ممنوع است.
---

🔒 هر گزینه امنیتی با علامت 🔒 در مستندات، یک الزام سخت پیاده‌سازی است و نباید نادیده گرفته شود.

## ۱۲. اهداف کارایی

| عملیات | هدف |
| `make()` singleton (کش‌شده) | ≤ ۱µs |
| `make()` transient بدون وابستگی | ≤ ۲µs |
| `make()` با ۵ وابستگی (Reflection Cache) | ≤ ۲۰µs |
| `make()` اولین بار (Reflection کامل) | ≤ ۳۰۰µs |
| `call()` با ۳ پارامتر | ≤ ۲۵µs |
| ۱۰۰۰ `make` متوالی | ≤ ۱ms |
| حافظه با ۲۰۰ binding | ≤ ۱٫۵MB |
| Compiled Container → بهبود | ≥ ۸۰٪ |

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

namespace Tavaan\Engine\Container;

use Tavaan\Core\Contracts\Container\ContainerInterface;
use Tavaan\Core\Provider\ServiceProvider;

class ContainerServiceProvider extends ServiceProvider
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

### ۱۳٫۴ فایل پیکربندی

یک فایل `config/container.php` با تمام کلیدهای مستندشده بسازید. مثال ساختار:

```php
<?php
declare(strict_types=1);

return [
    'default' => env('CONTAINER_DEFAULT', 'file'),
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

namespace Tavaan\Engine\Container\Tests\Feature;

use PHPUnit\Framework\TestCase;
use Tavaan\Engine\Container\<Manager>;

class ContainerTest extends TestCase
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

- مستندات: https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/container.md
- ROADMAP موتور: https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/ROADMAP.md
- TICKET موتور: https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/TICKET.md
- module.json: https://github.com/andrbi106/Tavaan-Engine-Container/blob/main/module.json
- مخزن موتور: https://github.com/andrbi106/Tavaan-Engine-Container
- مخزن اصلی فریمورک: https://github.com/Derogaramin/Tavaan-Framework
- مخزن مستندات: https://github.com/Derogaramin/Tavaan-Doc
- مخزن تفکیک (meta): https://github.com/andrbi106/Tavaan
- رجیستری موتورها: https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/README.md

---
*این پرامپت توسط Tavaan Engine Prompt Generator در 2026-11-03 09:28:10 UTC تولید شده است.*