---
fonts:
  # basically the text
  sans: "Robot"
  # use with `font-serif` css class from windicss
  serif: "Robot Slab"
  # for code blocks, inline code, etc.
  mono: "Fira Code"

layout: cover
---

# Python mock with decorators

```python
@with_mock(cls=ServiceA, mock=ServiceB)
class SomeService:
    """
    Service class that dynamically changes during runtime
    """
```
