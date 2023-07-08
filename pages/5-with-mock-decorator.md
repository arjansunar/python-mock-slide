# ✡️ Path to goal

- some way to generate dynamic class
- a condition to switch class

> See the [implementation](https://github.com/konnectkraft-dev/dms-backend/blob/master/mock/util.py#L33-L44)

<v-click>

```python {all|5|7-12|14|all} {lines:true}
def changeclass(condition: bool, class_a: T, class_b: T):
    """Decorator to change class according to the condition provided"""

    def decorator(cls: T) -> T:
        new_class = class_a if condition else class_b

        cls_name = getattr(new_class, "__name__")
        # INFO:  attr and behavior of the original class
        bases = getattr(cls, "__bases__", ())

        # Create a new class dynamically with the same name and bases as the original class
        modified_class = type(cls_name, bases, dict(new_class.__dict__))

        return modified_class

    return decorator

```

</v-click>
