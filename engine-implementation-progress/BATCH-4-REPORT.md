# Batch 4: Error, ORM, Schema — تکمیل‌شده

> تاریخ: 2026-11-03

## موتورهای تکمیل‌شده

| # | موتور | Stub‌ها | Commit | تست Runtime |
|---|-------|--------|--------|-------------|
| 1 | Error | 11/11 ✅ | `d32f41f` | ✅ PASS |
| 2 | ORM | 13/13 ✅ | `f7422da` | ✅ PASS |
| 3 | Schema | 7/7 ✅ | `48feb62` | ✅ PASS |

## Error (DOC-035)
- **ExceptionHandler**: report/render/map/renderable/reportable/dontReport/level/context
- **LogMasker**: addKeys/addPatterns/maskString with regex masking
- تست: render=PASS, masked=PASS, pattern=PASS

## ORM (DOC-050)
- **Model**: addGlobalScope/chunk/findOrFail/firstOrCreate/lazy/load/observe/paginate/query/refresh/update/updateOrCreate
- تست: create=PASS, find=PASS, name=PASS, update=PASS, count=1, fco=PASS, upsert=PASS, paginate=1

## Schema (DOC-048)
- **SchemaBuilder**: introspect() method
- **Blueprint**: column/foreign/fullText/primary/types
- تست: hasTable=PASS, hasCol=PASS, cols=3, introspect=3, alter=PASS, drop=PASS

---
*Generated on 2026-11-03*
