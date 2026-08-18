[`scipy.special.cbrt`{.python}](https://docs.scipy.org/doc/scipy/reference/generated/scipy.special.cbrt.html) computes the cube roots of individual values, or collections of numbers

## Individual Numbers

`cbrt`{.python} can calculate the cube root of a single number, including negative numbers.

```py-cell
from scipy.special import cbrt

# Single values
print("cbrt(8) =", cbrt(8))
print("cbrt(27) =", cbrt(27))
print("cbrt(-8) =", cbrt(-8))
```

## Element-wise on arrays

`cbrt`{.python} can also be used to calculate the cube roots of a NumPy array, or other collection of numbers (such as a list). The function will return a NumPy array of the same shape, with the cube roots of each element.

```py-cell
import numpy as np
from scipy.special import cbrt

# NumPy array of values
numpy_input = np.array([1, 8, 27, 64, 125])
roots = cbrt(numpy_input)
print("NumPy Input:", numpy_input)
print("Cube roots:", roots)

# List of values
list_input = [1, 8, 27, 64, 125]
roots = cbrt(list_input)
print("List Input:", list_input)
print("Cube roots:", roots)
```