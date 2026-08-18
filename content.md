`scipy.special.cbrt` computes the cube roots of individual values, or of NumPy arrays in an elementwise fashion. It is faster and more numerically stable than using `x ** (1/3)`.

## Basic cube root

```py-cell
from scipy.special import cbrt

# Single values
print("cbrt(8) =", cbrt(8))
print("cbrt(27) =", cbrt(27))
print("cbrt(-8) =", cbrt(-8))
```

## Element-wise on arrays

```py-cell
import numpy as np
from scipy.special import cbrt

# Array of values
x = np.array([1, 8, 27, 64, 125])
roots = cbrt(x)
print("Values:", x)
print("Cube roots:", roots)
```
