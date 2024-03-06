`Royen2016NonCentralBivariate4x4.m`
A quadrivariate implementation of p-variate integral from Royen's 2016 paper, tested in the independent chi squares case. Can be changed to P-variate by changing the variable P. Nonindependent cases require comparison with Montecarlo.
```
lexico_royen.m: computes multiindex in lexicographic order
```

`Scratches\Gcal.m`
Contains the function $\mathcal{G}_\alpha(x, y)$ in the notation of Royen's 2016 paper.

$$\mathcal{G}_\alpha(x, y) = \begin{cases} \frac{1}{1- y}\left( G_\alpha(x) - y^{1-\alpha}e^{x(1-y)}G_\alpha(xy) \right) \quad &y \neq 0 \\ G_\alpha(x) \quad &y=0\end{cases}$$
Note that if $y = 0, \alpha = 1$ then we need the second case. Otherwise you can always use the first case.

`RoyenMC.m` [FAILED]
An attempt at reducing the complexity of the numerical integration of the p-variate royen by using a montecarlo scheme with a von-Mises distribution as the base distribution. This has failed.
```
vmrand.m: draws random variates from a von-Mises distribution.
```

`RoyenVsKhammassi.m` [FAILED]
We want to compare khammassi method against royens. We are not sure what is the cause of the problem.
```
SigmaKhammasi5.mat
```

`Royen2016NonCentralBivariateIntegrand1.m`
Plots the integrand of Royen's 2016 P-Variate in the Bivariate case (the last visible case).
It also attempts to sweep for different values of $x_1, x_2$ and store the integrand in a big array, such that slices in the last two dimensions represent the integrand for fixed $x_1$ and $x_2$. To obtain nicer plots use higher number of mesh points. Modify Line 15 `z = 20` and reduce `values` Line 36 to singleton to reduce run time.

`Royen2016NonCentralBivariate.m`
Very similar to the previous

`SomeDataFiles\*`
Royens 2016 Integrand at some values which Mahmoud cannot recall currently.

`Royen2016NonCentralSingularIntegrand.m`
Single variate non-central chi-square attempt at comparison with "matlab builtin" formula for non-central density. Run Line 42 again to see the comparison plot.

`Royen2016NonCentralSingular.m`
Same as above without the Integrand plot.

`Numslog.m`
Computes the logarithms of $M$ (number of Quadratic Forms) and $N$ number of gaussian variables so that we use this in the *NOT TO SCALE* (but more meaningful) M vs. N graph.

`MaoTodd\MaoTodd.m` and `MaoTodd\MaoToddSim.m`
Files attempting to compare MaoTodds formulae. We believe they are wrong. Run MaoToddSim to obatin the montecarlo simulation from which a histogram is obtained. The centers of this histogram are the points at which `MaoTodd.m` evaluates the PDF. Run the folowing code segment to see the results (without legend)
```matlab
cx = Centers(1:100); 
vx = Values(1:100); px = p(1:100); p1x = p1(1:100); pwx = pW(1:100); 
plot(cx, vx, cx, px, cx, p1x, cx, pwx);
```

