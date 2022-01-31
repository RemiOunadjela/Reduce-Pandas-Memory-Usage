# reduce_mem_usage.py

Using this code, you can automatically reduce the size of your Pandas dataframes by up to 75%.

Note that I didn't write this code. I got it from somewhere (can't recall the original source), it's here mostly so that I have a place to come back to and find it.


Reproducible example:
```python
from sklearn.datasets import load_wine
df = pd.DataFrame(load_wine().data, columns=load_wine().feature_names)
df = reduce_mem_usage(df);
```
