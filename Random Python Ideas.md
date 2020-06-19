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
	def heaven_or_hell(self, name: str) -> None:
		if len(name) % 2 == 1: # odd is not nice
			return "hell"
		else:
			return "heaven"

# now this is valid code
God.heaven_or_hell("vivax")
```

## Meta Class Shortcut
Easier to make meta classes.

### code
```python
from typing import TypeVar, Type

T = TypeVar("T")

def meta_shortcut(cls: Type[T]) -> T:
	class wrapper(metaclass=cls):
		pass
	
	wrapper.__name__ = cls.__name__
	return wrapper
```

### Example
```python
@meta_shortcut
class Colors(type):
	def __new__(
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4MzQzNzU0ODksNjIxOTUzMjUsLTExMT
YyMTgwNDldfQ==
-->