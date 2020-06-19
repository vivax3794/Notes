# Decorators
## instance decorator
makes a class into a instance.

### code
```python
from typing import TypeVar, Type

T = TypeVar("T")

def instance(cls: Type[T]) -> T:
	return cls()
```

### example
```python
@instance
class God:
	def \
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTU1OTAyMzI3N119
-->