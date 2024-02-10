# timer
> calc time for module

## 1.install
`pip install git+https://github.com/aidings/timer.git`

## 2.example
```python
import time
from timer import timer, Timer

#Timer('just one function')  # 1. 
@timer('just one function')  # 2.  
def func():
    time.sleep(2)

if __name__ == '__main__':
    func()

    """
    3.
    with Timer('just one function'):
        func()

    4.
    t = Timer('just one function')
    t.start()
    func()
    t.stop()

    t.time()
    """
    
```