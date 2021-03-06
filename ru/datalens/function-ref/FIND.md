---
editable: false
---

# FIND

_Строковые функции_

#### Синтаксис


```
FIND( string, substring [ , start_index ] )
```

#### Описание
Возвращает индекс позиции первого символа подстроки `substring` в строке `string`.

Если указан опциональный параметр `start_index`, то поиск начнется с указанной позиции.

**Типы аргументов:**
- `string` — `Строка`
- `substring` — `Строка`
- `start_index` — `Целое число`


**Возвращаемый тип**: `Целое число`

#### Примеры

```
FIND("Lorem ipsum dolor sit amet", "abc") = 0
```

```
FIND("Lorem ipsum dolor sit amet", "or") = 2
```

```
FIND("Lorem ipsum dolor sit amet", "or", 7) = 16
```


#### Поддержка источников данных

`Материализованный датасет`, `ClickHouse 1.1`, `Microsoft SQL Server 2017 (14.0)`, `MySQL 5.6`, `PostgreSQL 9.3`.
