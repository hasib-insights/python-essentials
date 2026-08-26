### Pandas Data Structures
Pandas has two main data structures:

| Data Structure  | Description     | Dimensions |
|-----------------|-----------------|------------|
| Series          |  Labeled array  | 1D         |
| DataFrame       | Tabular data    | 2D         |

 Think of it like:
>
> Series = One column in a table
>
>  DataFrame = The entire table with many columns

```
┌─────────────────────────────────────────────────────────────────┐
│                    PANDAS DATA STRUCTURES                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   SERIES (1D)                    DATAFRAME (2D)                 │
│                                                                 │
│   ┌──────────────┐              ┌────────┬────────┬────────┐    │
│   │ Index │ Value│              │        │ Name   │ Age    │    │
│   ├──────────────┤              ├────────┼────────┼────────┤    │
│   │  a    │  10  │              │  0     │ Alice  │  25    │    │
│   │  b    │  20  │              │  1     │ Bob    │  30    │    │
│   │  c    │  30  │              │  2     │ Charlie│  35    │    │
│   │  d    │  40  │              └────────┴────────┴────────┘    │
│   └──────────────┘                                              │
│                                                                 │
│   One column = Series           Multiple columns = DataFrame    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```



