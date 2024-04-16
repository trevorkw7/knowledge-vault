## Continuous Time Unit Step $u(t)$

> [!Definition]
> 
$u(t) = \begin{cases} 0, t < 0 \\ 1, t\geq 0\end{cases}$
- 0 for negative time
- 1 for positive time
## Continuous Time Unit Impulse $\delta(t)$
> [!Definition]
> 
$\delta(t) = \begin{cases} 0, t \neq 0 \\ 1, t=0 \end{cases}$
- 1 at t=0, 0 everywhere else
### Mathematical Definition
- First define $\delta_{\Delta}(t) =\begin{cases} \frac{1}{\Delta}, \text{if t} \in [0, \Delta] \\ 0, \text{else}\end{cases}$
- Since no matter how small $\Delta$ is, $\frac{1}{\Delta} * \Delta = 1$, we can define $\delta(t) = \lim_{ \Delta \to \infty } \delta_{\Delta}(t)$ 
### Properties
- Interesting property as a result of mathematical def: 
	- $\int \delta(\tau)d\tau = 1$
	- Unit mass is 1 at t = 0
- All the rules of calculus apply to it
- Relation between $u(t)$ and $\delta(t)$ is that:
	- $u(t) = \int_{-\infty}^t \delta(t) \, dx$
	- This is because if $t < 0$ then the integral will be 0 and if $t \geq 0$ it will include the unit impulse and must be 1.
- Continuous unit impulse properties are similar except summation is replaced with integration, $\delta[n], u[n]$ replaced with $d(t), u(t)$.
	- [[Sampling Properties]]
	- [[Sifting Properties]]
	- [[Representation Properties]]




