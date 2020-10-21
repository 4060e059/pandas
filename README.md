# pandas
```
https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html
```
### 載入
```
import numpy as np
import pandas as pd
```
## Object creation
### 數值值列表，用熊貓創建，默認整數索引
```
s = pd.Series([1, 3, 5, np.nan, 6, 8])
s
```
### date_range
```
dates = pd.date_range('20201021', periods=6)
dates
```
### DataFrame
##### random.randn()  用來隨機建立資料
##### index=dates,    顯示日期
```
df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list('ABCD'))
df
```
```
df2 = pd.DataFrame({'A': 1.,
           'B': pd.Timestamp('20201021'),
           'C': pd.Series(1, index=list(range(4)), dtype='float32'),
           'D': np.array([3] * 4, dtype='int32'),
           'E': pd.Categorical(["test", "train", "test", "train"]),
           'F': 'foo'})
df2
```
```

```
