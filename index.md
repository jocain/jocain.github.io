# Project 1

Here is a cool picture of the Cherenkov Radiation in the Advanced Test Reactor in Idaho:
<p align="center">
  <img src="Advanced_Test_Reactor.jpg" width="300">
</p>

Cherenkov Radiation can occur if a charged partice with some velocity <img src="https://latex.codecogs.com/svg.image?v&space;" title="v " /> enters a material with refractive index <img src="https://latex.codecogs.com/svg.image?n" title="n" />. The speed of light in this material is <img src="https://latex.codecogs.com/svg.image?c" title="c" />/<img src="https://latex.codecogs.com/svg.image?n" title="n" />, and if is value is less than <img src="https://latex.codecogs.com/svg.image?v&space;" title="v " />, then the particle will emit light, called as Cherenkov radiation. The angle of radiation emission is directly related to the relative speeds:

<p align="center">
<img src="https://latex.codecogs.com/svg.image?\cos{\theta_c}&space;=&space;\frac{c}{nv}." title="\cos{\theta_c} = \frac{c}{nv}." />
</p>

You can get the Cherenkov angle <img src="https://latex.codecogs.com/svg.image?\theta_c" title="\theta_c" /> this with Python with the following code:

```
import numpy as np

thetac = lambda v, n: np.arccos((2.998*(10**8))/(n*v))
```

This assumes a velocity in \[m/s], and returns a value in radians. In the picture above, beta particles (electrons) are escaping the reactor and producing Cherenkov radiation in the water, producing the glow. 
