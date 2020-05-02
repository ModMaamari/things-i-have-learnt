# Python : 1- Calculating Time :
Using the next snippet:

```
import time

start = time.time()
"Your code goes here"
end = time.time()

print(f"Consumed Time = {end-start} seconds)
```

Example:
```
import time

start = time.time()
time.sleep(3)
end = time.time()

print(f"Consumed Time = {end-start} seconds")
```
Out : ``` Consumed Time = 3.002717971801758 seconds ```

You can make it even prettier by rounding the time by changing the print line to :
``` print(f"Consumed Time = {round(end-start,2)} seconds") ```

Out : ``` Consumed Time = 3.00 seconds ```
