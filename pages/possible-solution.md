# How to achieve dynamic classes at runtime ?

Maybe use an intermediary class/function that provides the right class.

<div style="height: 10px" />

```python
def get_service(condition: bool, cls_a, cls_b):
  """Returns the specified classes acording to provided condition."""
  return cls_a if condition else cls_b
```

<v-click>

<div style="height: 10px" />

## Downside of this approach

- need to create an intermidiary function/class to handle the assignment of the `cls` needed.

</v-click>

<v-click>

<div style="height: 10px" />

## What I had envisioned

I wanted a method to easily extend this usecase by adding a simple decorator.

<v-click>

> Concise and easily added to other services

</v-click>

</v-click>
