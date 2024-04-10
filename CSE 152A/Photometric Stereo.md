## Assumptions
- Lambertian reflectance
	- Image formation model: Image intensity = albedo * surface normal * s
	- $I^k(x,y) = \rho(x,y)\hat{n}(x,y)s^k = b(x,y)*s^k$ 
- Light sources is infinitely far so at any point on the surface we don't care about fall offs
- Relative the the size of the object the camera is far away
	- Why? We parameterized the image plane $z(x,y)$ which is why we can parameterize the entire image based on the image plane. 

## Solving Method
- 3 observations per pixel
	- This characterizes our problem
- This gives us values for $b(x,y)$ and since we know our light source intensities $s$ we can solve for b
- $e(x,y) = Sb(x,y)$
- $b(x,y) = S^{-1}e(x,y)$
- By definition, the surface normal is a unit vector therefore if we find the unit vector of b it gives us the surface normal $\hat{n}$
- Our byproduct is thus albedo $\rho$
## Using more than 3 observations
- Increases the signal to noise ratio
- Put our observations in a K dimensional vector
- We want to solve for b but S is not an invertible matrix because it's not a square so do the following:
	- Multiply the transpose $S^T$ (which represents our light source intensities) on both sides
	- Results in the normal equation: $b(x,y) =(S^TS)^{-1}S^Te(x,y)$
## Recovering Surface from Normals
- Goal: recover $z(x,y)$ from the surface normals $\hat{n}$
- By definition: ![[Pasted image 20240119173115.png]]
- $\hat{n}=(\hat{n}_{1}, \hat{n}_{2}, \hat{n_{3}})$
- ![[Pasted image 20240119173132.png]]
- Now that we have $\frac{dz}{dx}$ and $\frac{dz}{dy}$ we can integrate to find our surface
- By definition of a derivative: $\frac{z(t + \Delta t) -z(t)}{\Delta t}$
- Our $\Delta t$ is 1 pixel on the pixel grid
- So our derivatives are just changes between 1 pixel. We can start at an arbitrary point and add the derivative for the next point.
	- Integration sums this up so we can just integrate $\frac{dz}{dx}$ along row 0 to get $z(x,0)$, same thing for $\frac{dz}{dy}$
## Integratabilnty Problem
- Because of noise there may be 2 "paths" to a pixel from the original pixel using different x and y values that result in that pixel having a different value
- Formulaic function in homework given