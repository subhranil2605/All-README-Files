# Python multi threading to execute a function in multiple threads

```python
import concurrent.futures

def func(*args, **kwargs):
    with concurrent.futures.ThreadPoolExecutor() as executor:
        futures = []
        for i in range(10):
            future = executor.submit(sync_func, *args)
            futures.append(future)

        # Wait for all the futures to complete
        concurrent.futures.wait(futures)

    print("completed!")

def main():
    func(arg1, arg2, arg3)
```
