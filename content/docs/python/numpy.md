---
title: numpy
aliases:
  - numpy
tags: 
date: 2023-09-19
---
```python
import numpy as np
```

## `np.arange()`
The `np.arange()` function generates a list of values from the lower to the upper value, separated by `step`.

```python
import numpy as np

generated_values = np.arange (lower, upper, step)

```

## `numpy.linspace`

The following function should generate a list of values spaced apart by `step`. This is a workaround to getting some floats and other weird things that `np.arange()` doesn't like.

```python
import numpy as np

def generate_bounds(lower, upper, step):
	samples = round(((upper-lower)/step),0) + 1
	generated_values = np.linspace(lower, upper, samples)
	return generated_values
```