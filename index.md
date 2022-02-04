# Project 1

Here is a cool picture of the Cherenkov Radiation in the Advanced Test Reactor in Idaho:
<p align="center">
  <img src="Advanced_Test_Reactor.jpg" width="300">
</p>

Cherenkov Radiation can occur if a charged partice with some velocity <img src="https://latex.codecogs.com/svg.image?v&space;" title="v " /> enters a material with refractive index $n$. The speed of light in this material is $c/n$, and if is value is less than $v$, then the particle will emit light known as Cherenkov radiation. The angle of radiation emission is directly related to the relative speeds:

<p align="center">
<img src="https://latex.codecogs.com/svg.image?\cos{\theta_c}&space;=&space;\frac{c}{nv}." title="\cos{\theta_c} = \frac{c}{nv}." />
</p>

You can get the Cherenkov angle $\theta_c$ this with Python with the following code:

```
import numpy as np

thetac = lambda v, n: np.arccos((2.998*(10**8))/(n*v))
```

This assumes a velocity in \[m/s], and returns a value in radians.
