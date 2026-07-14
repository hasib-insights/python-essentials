#  Python Data Structures: Comparison

## Quick Overview

| Feature | List `[]` | Dictionary `{}` | Tuple `()` | Set `{}` / `set()` |
|---------|-----------|-----------------|------------|-------------------|
| **Syntax** | `[1, 2, 3]` | `{"a": 1, "b": 2}` | `(1, 2, 3)` | `{1, 2, 3}` |
| **Mutable** | ✅ Yes | ✅ Yes | ❌ No | ✅ Yes |
| **Ordered** | ✅ Yes | ✅ Yes (3.7+) | ✅ Yes | ❌ No |
| **Duplicates** | ✅ Allowed | ❌ No (keys) | ✅ Allowed | ❌ No |
| **Indexed** | ✅ Yes | ✅ By key | ✅ Yes | ❌ No |
| **Memory Usage** | Medium | Large | Small | Medium |
| **Speed (Access)** | Fast | Very Fast | Fast | Medium |
| **Speed (Iteration)** | Fast | Medium | Fast | Medium |
| **Use Case** | Ordered collections | Key-value mapping | Immutable data | Unique items |

---

##  Detailed Comparison

###  Mutability (Changeable?)

| Data Type | Can Change? | Example |
|-----------|-------------|---------|
| **List** | ✅ Yes | `my_list[0] = 10` ✅ |
| **Dictionary** | ✅ Yes | `my_dict["age"] = 30` ✅ |
| **Tuple** | ❌ No | `my_tuple[0] = 10` ❌ |
| **Set** | ✅ Yes | `my_set.add(5)` ✅ |

###  Order (Preserves Insertion Order?)

| Data Type | Ordered? | Example |
|-----------|----------|---------|
| **List** | ✅ Yes | `[1, 2, 3]` always in same order |
| **Dictionary** | ✅ Yes (3.7+) | Keys maintain insertion order |
| **Tuple** | ✅ Yes | `(1, 2, 3)` always in same order |
| **Set** | ❌ No | `{1, 2, 3}` = `{3, 2, 1}` |

###  Duplicates Allowed?

| Data Type | Duplicates? | Example |
|-----------|-------------|---------|
| **List** | ✅ Yes | `[1, 1, 2, 2, 3]` ✅ |
| **Dictionary** | ❌ No (keys) | `{"a": 1, "a": 2}` ❌ (last wins) |
| **Tuple** | ✅ Yes | `(1, 1, 2, 2, 3)` ✅ |
| **Set** | ❌ No | `{1, 1, 2, 2, 3}` → `{1, 2, 3}` |

###  Access Method

| Data Type | Access Method | Example |
|-----------|---------------|---------|
| **List** | By index | `my_list[0]` |
| **Dictionary** | By key | `my_dict["name"]` |
| **Tuple** | By index | `my_tuple[0]` |
| **Set** | No index access | Cannot access individual elements |

---

##  When to Use Which?

### Use LIST when you need:
- ✅ Ordered collection
- ✅ Mutable data
- ✅ Allow duplicates
- ✅ Fast indexing
- ✅ Sequence operations

### Use DICTIONARY when you need:
- ✅ Key-value pairs
- ✅ Fast lookup by key
- ✅ Store relationships
- ✅ Configuration data
- ✅ Count/frequency tracking

### Use TUPLE when you need:
- ✅ Immutable data
- ✅ Faster than lists
- ✅ Dictionary keys
- ✅ Fixed data collection
- ✅ Return multiple values

### Use SET when you need:
- ✅ Unique items
- ✅ Mathematical operations
- ✅ Remove duplicates
- ✅ Membership testing
- ✅ Common elements between collections

---

##  Code Examples

### List
```python
# Ordered, mutable, duplicates allowed
fruits = ["apple", "banana", "cherry", "apple"]
fruits[1] = "orange"  # Change allowed
print(fruits)  # ['apple', 'orange', 'cherry', 'apple']
