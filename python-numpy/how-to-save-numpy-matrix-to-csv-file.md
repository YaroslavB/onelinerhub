# How to save Numpy matrix to CSV file

```python
import numpy as np

db = np.array([[1,2], [3,4], [5,6]])
np.savetxt('/tmp/db.csv', db, delimiter=',')
```

- `import numpy as np` - load [lib:Numpy module](/python-numpy/how-to-install-python-numpy-lib) for Python
- `np.array` - declare Numpy array (or matrix)
- `.savetxt` - saves specified matrix to `csv` file
- `/tmp/db.csv` - path to `csv` file to save matrix to
- `db` - matrix to save to `csv` file
- `delimiter=','` - specify delimiter to match `csv` format

group: csv

## Example: 
```python
import numpy as np

matrix = np.array([[1,2], [3,4], [5,6]])
np.savetxt('/tmp/db.csv', matrix, delimiter=',')

with open('/tmp/db.csv', 'r') as f:
  print(f.read())

```
```
1.000000000000000000e+00,2.000000000000000000e+00
3.000000000000000000e+00,4.000000000000000000e+00
5.000000000000000000e+00,6.000000000000000000e+00


```

