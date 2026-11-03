# Progress Report: Tavaan-Engine-Event

| Field | Value |
|-------|-------|
| Engine | `tavaan.engine.event` |
| DOC-ID | `DOC-033` |
| Repository | https://github.com/andrbi106/Tavaan-Engine-Event |
| Implementation commit | `94ebd342397927b03ede25d628b0902a8ec552e4` |
| Date | 2026-11-03 10:03:57 UTC |
| Status | ✅ completed |
| Source files | 7 |
| Test files | 1 |
| Config files | 1 |
| Lang files | 2 |
| LOC | 411 |
| Old src files (replaced) | 7 |

## Generated files

### Source (`src/`)
- `src/OutboxRelay.php`
- `src/EventDispatcherServiceProvider.php`
- `src/EventDispatcher.php`
- `src/Console/EventListCommand.php`
- `src/Console/EventOutboxRelayCommand.php`
- `src/Contracts/OutboxRelayInterface.php`
- `src/Contracts/EventDispatcherInterface.php`

### Tests (`tests/`)
- `tests/Feature/EventDispatcherTest.php`

### Config (`config/`)
- `config/event.php`

### Lang (`lang/`)
- `lang/en/event.php`
- `lang/fa/event.php`

## Public API implemented

### `EventDispatcher` (11 methods)
### `OutboxRelay` (3 methods)

## Test scenarios

15 scenarios (T-NN) from docs — each mapped to a `testTNN_*` method.

## Acceptance criteria

`AC-EVT-01`, `AC-EVT-11`, `AC-EVT-12`, `AC-EVT-13`

## Notes

- This is a scaffold implementation. Method bodies return `null` or `[]` with `// TODO` markers — they need real implementation per the doc's API section.
- All PHP files use `declare(strict_types=1);`.
- All classes are `final` (where applicable).
- Tests use PHPUnit and `markTestIncomplete` for T-NN scenarios not yet fully implemented.
- README.md provides usage examples.
- `module.json` updated: `autoload` now points to `src/`, `providers` includes the ServiceProvider.

## Next steps

1. Open the doc (`https://github.com/Derogaramin/Tavaan-Doc/blob/main/docs/03-engines/event.md`) and implement each method body per the API section.
2. Replace `markTestIncomplete` in tests with real assertions per T-NN scenarios.
3. Run `php bin/tvn test engines/event` to verify.
4. Run `php bin/tvn stan` to verify PHPStan compliance.
5. Run `php bin/tvn cs:check` to verify coding standard.
