#  Python Data Structures: Comparison

## Quick Overview

| Feature | List `[]` | Dictionary `{}` | Tuple `()` | Set `{}` / `set()` |
|---------|-----------|-----------------|------------|-------------------|
| **Syntax** | `[1, 2, 3]` | `{"a": 1, "b": 2}` | `(1, 2, 3)` | `{1, 2, 3}` |
| **Mutable** |  Yes |  Yes | No |  Yes |
| **Ordered** |  Yes |  Yes  |  Yes |  No |
| **Duplicates** |  Allowed |  No (keys) |  Allowed |  No |
| **Access** |  By index |  By key |  By index | Cannot access |
| **Memory Usage** | Medium | Large | Small | Medium |
| **Speed (Access)** | Fast | Very Fast | Fast | Medium |
| **Speed (Iteration)** | Fast | Medium | Fast | Medium |


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
