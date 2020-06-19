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

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExMTYyMTgwNDldfQ==
-->