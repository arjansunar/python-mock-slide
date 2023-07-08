---
fonts:
  # basically the text
  sans: "Robot"
  # use with `font-serif` css class from windicss
  serif: "Robot Slab"
  # for code blocks, inline code, etc.
  mono: "Fira Code"
transition: fade
---

# Python mock with decorators

### Use Case

- create a service that changes its `Class` or behaviour in runtime
- use the actual service in `PROD` but mock service in `DEV`

### Goal 🚀

```python
@with_mock(cls=ServiceA, mock=ServiceB)
class SomeService:
    """
    Service class that dynamically changes during runtime
    """
```


---
src: ./pages/2-possible-solution.md
---
---
src: ./pages/3-solution.md
---
---
src: ./pages/4-basic-decorator.md
---
---
src: ./pages/5-with-mock-decorator.md
---
