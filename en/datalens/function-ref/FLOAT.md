---
editable: false
---

# FLOAT

_Type conversion functions_

#### Syntax


```
FLOAT( expression )
```

#### Description
Converts the `expression` expression to fractional number format according to the following rules:

| Type                              | Value                                                                                                                                                                                                             |
|:----------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `Number`                          | Original value.                                                                                                                                                                                                   |
| <code>Date &#124; Datetime</code> | [Unix time](https://en.wikipedia.org/wiki/Unix_time) corresponding to the date and time. If the value contains time zone data, it's used in the calculation. If the time zone is unknown, the time is set in UTC. |
| `String`                          | A number from a decimal string.                                                                                                                                                                                   |
| `Boolean`                         | `TRUE` — `1.0`, `FALSE` — `0.0`.                                                                                                                                                                                  |

**Argument types:**
- `expression` — `Boolean | Date | Datetime | Number | String`


**Return type**: `Number (decimal)`

#### Examples

```
FLOAT(7) = 7.0
```

```
FLOAT("34.567") = 34.567
```

```
FLOAT(TRUE) = 1.0
```


#### Data source support

`Materialized Dataset`, `ClickHouse 1.1`, `Microsoft SQL Server 2017 (14.0)`, `MySQL 5.6`, `PostgreSQL 9.3`.
