# Calculating a plane curve with continuous curvature.

![animated curve](https://github.com/dan-reznik/continuous-curvature/blob/master/integrated%20curvature.gif)

###  Animations of the experiment as .gif and .avi. On youtube: https://www.youtube.com/watch?v=EjRqZaAv5c8

### The curvature profile is piecewise parabolic (3 parabolic segments), parametrized from 0 < s < 4.

k[s]:
s^2            : 0 <= s < 1,
-(s - 2)^2 + 2 : 1 <= s < 3,
(s - 4)^2      : 3 <= s < 4

### The plane curve is computed in two steps:

* 1. obtain the angle function as a definite integral from the curvature (w/ scaling param "a"), in closed-form.
* 2. Obtain the curve itself by numerically integrating the cosine and sine of the angle function.

![plane curve integral](https://github.com/dan-reznik/continuous-curvature/blob/master/from%20curvature%20to%20plane%20curve.png)

* Note: curve is "started" at (0,0).
* The animation shows curve(a,s) for 0<s<4, and "a" varied from 0 to 2 in steps of 0.01
* Curve points at s=0,1,3,4 are drawn on curve.
* Note curve surprisingly loops onto itself at a = 1.07761, 2.61733, 4.18347, ...  
