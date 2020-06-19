---
editable: false
---

# BOOL

_Функции преобразования типов_

#### Синтаксис


```
BOOL( expression )
```

#### Описание
Переводит выражение `expression` в логический тип по следующим правилам:

| Тип                                   | `FALSE`              | `TRUE`        |
|:--------------------------------------|:---------------------|:--------------|
| `Число`                               | `0`, `0.0`           | Все остальные |
| `Строка`                              | Пустая строка (`""`) | Все остальные |
| `Логический`                          | `FALSE`              | `TRUE`        |
| <code>Дата &#124; Дата и время</code> | -                    | `TRUE`        |

**Типы аргументов:**
- `expression` — `Логический | Дата | Дата и время | Геоточка | Геополигон | Число | Строка`


**Возвращаемый тип**: `Логический`

#### Примеры

```
BOOL(0) = FALSE
```

```
BOOL(#2019-04-04#) = TRUE
```

```
BOOL("Lorem ipsum") = TRUE
```


#### Поддержка источников данных

`Материализованный датасет`, `ClickHouse 1.1`, `Microsoft SQL Server 2017 (14.0)`, `MySQL 5.6`, `PostgreSQL 9.3`.