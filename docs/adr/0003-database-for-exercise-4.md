# 0003. Database for Exercise 4 / База данни за Упражнение 4

**Status / Статус:** Proposed

## Context / Контекст

Notes are kept in memory and are lost on restart. / Бележките са в паметта и се губят при рестарт.

## Options / Варианти

- PostgreSQL: the app already supports it (`DATABASE_URL`). Minus: one more service to run. / Приложението вече го поддържа (`DATABASE_URL`). Минус: още една услуга за пускане.
- SQLite: just a file. Minus: the app does not support it. / Само един файл. Минус: приложението не го поддържа.

## Decision / Решение

PostgreSQL.

## Consequences / Последствия

Notes survive restarts. In Exercise 4 we also run a PostgreSQL container. / Бележките остават след рестарт. В Упражнение 4 пускаме и контейнер с PostgreSQL.