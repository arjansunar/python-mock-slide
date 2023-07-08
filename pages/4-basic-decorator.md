### Basic decorator

```python {17-18|1-14|all} {lines:true}
def decorator_function(original_function):
    def wrapper_function(*args, **kwargs):
        # Add some extra functionality before the original function is called
        print("Before the function call")

        # Call the original function
        result = original_function(*args, **kwargs)

        # Add some extra functionality after the original function is called
        print("After the function call")

        return result

    return wrapper_function

@decorator_function
def hello():
    print("Hello, world!")

hello()
```

<v-clicks>
<Arrow x1="10" y1="20" x2="100" y2="150" />
<Arrow x1="10" y1="20" x2="100" y2="250" />
</v-clicks>
