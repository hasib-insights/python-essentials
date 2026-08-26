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
─────────────────────────────────────────────────────────────────
                    PANDAS DATA STRUCTURES                       
─────────────────────────────────────────────────────────────────
                                                                 
   SERIES (1D)                    DATAFRAME (2D)                 
                                                                 
   ┌──────────────┐              ┌────────┬────────┬────────┐    
   │ Index │ Value│              │        │ Name   │ Age    │    
   ├──────────────┤              ├────────┼────────┼────────┤    
   │  0    │  10  │              │  0     │ Alice  │  25    │    
   │  1    │  20  │              │  1     │ Bob    │  30    │    
   │  2    │  30  │              │  2     │ Charlie│  35    │    
   |  3    |  40  |              |  3     | Hasib  |  25    |    
   │  4    │  40  │              |  4     | Jhon   |  30    |   
   └──────────────┘              └────────┴────────┴────────┘                                │
                                                                 
   One column = Series           Multiple columns = DataFrame    
                                                                 

```



