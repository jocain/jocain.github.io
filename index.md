# Project 1

Here is a cool picture of the Cherenkov Radiation in the Advanced Test Reactor in Idaho:

<img src="Advanced_Test_Reactor.jpg" width="100">

Cherenkov Radiation can occur if a charged partice with some velocity $v$ enters a material with refractive index $n$. The speed of light in this material is $c/n$, and if is value is less than $v$, then the particle will emit light known as Cherenkov radiation. The angle of radiation emission is directly related to the relative speeds:

$$ \cos{\theta_c} = \frac{c}{nv}. $$

You can get the Cherenkov angle $\theta_c$ this with Python with the following code:

```
import numpy as np

thetac = lambda v, n: np.arccos((2.998*(10**8))/(n*v))
```

This assumes a velocity in \[m/s], and returns a value in radians.
