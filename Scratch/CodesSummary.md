`Royen2016/Royen2016NonCentralBivariate4x4.m`
A quadrivariate implementation of p-variate integral from Royen's 2016 paper, tested in the independent chi squares case. Can be changed to P-variate by changing the variable P. Nonindependent cases require comparison with Montecarlo.
```
lexico_royen.m: computes multiindex in lexicographic order
```

`Royen2016/Scratches\Gcal.m`
Contains the function $\mathcal{G}_\alpha(x, y)$ in the notation of Royen's 2016 paper.

$$\mathcal{G}_\alpha(x, y) = \begin{cases} \frac{1}{1- y}\left( G_\alpha(x) - y^{1-\alpha}e^{x(1-y)}G_\alpha(xy) \right) \quad &y \neq 0 \\ G_\alpha(x) \quad &y=0\end{cases}$$
Note that if $y = 0, \alpha = 1$ then we need the second case. Otherwise you can always use the first case.

`Royen2016/RoyenMC.m` [FAILED]
An attempt at reducing the complexity of the numerical integration of the p-variate royen by using a montecarlo scheme with a von-Mises distribution as the base distribution. This has failed.
```
vmrand.m: draws random variates from a von-Mises distribution.
```

`Royen2016/RoyenVsKhammassi.m` [FAILED]
We want to compare khammassi method against royens. We are not sure what is the cause of the problem.
```
SigmaKhammasi5.mat
```

`Royen2016/Royen2016NonCentralBivariateIntegrand1.m`
Plots the integrand of Royen's 2016 P-Variate in the Bivariate case (the last visible case).
It also attempts to sweep for different values of $x_1, x_2$ and store the integrand in a big array, such that slices in the last two dimensions represent the integrand for fixed $x_1$ and $x_2$. To obtain nicer plots use higher number of mesh points. Modify Line 15 `z = 20` and reduce `values` Line 36 to singleton to reduce run time.

`Royen2016/Royen2016NonCentralBivariate.m`
Very similar to the previous

`Royen2016/SomeDataFiles\*`
Royens 2016 Integrand at some values which Mahmoud cannot recall currently.

`Royen2016/Royen2016NonCentralSingularIntegrand.m`
Single variate non-central chi-square attempt at comparison with "matlab builtin" formula for non-central density. Run Line 42 again to see the comparison plot.

`Royen2016/Royen2016NonCentralSingular.m`
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

`KuonenAndSaddlePoints\Kuonen2.m`
Not Working

`KuonenAndSaddlePoints\KuonenCentralArgument.pdf` shows how the argument at 2 produces a failure, and how this can be ficed by a Taylor expansion at 1.8 or 2.2

`KuonenAndSaddlePoints\save_to_pdf_example.m` saves a plot to pdf allowing with vector graphics.

`KuonenAndSaddlePoints\ArgumentVSaRgument.m` shows one-sided approximation, without a scale.

`KuonenAndSaddlePoints\ArgumentVSaRgument.fig` shows the same left approximation with a scale.

`KuonenAndSaddlePoints\Kuonen.m` produces the graph comparing a MC simulation and Kuonen's saddlepoint approximation showing that the latter does not work for a middle interval.

`KuonenAndSaddlePoints\KuonenNVar7.m` demonstrates, using four differerent scenarios, that non-centrality produces a whole range of complex argument, and centrality seemingly produces one division by zero.

`KuonenAndSaddlePoints\KuonenAbsolute.m` tries to replace $v$ by its modulus; no meaningful result is obtained.

`KuonenAndSaddlePoints\Kuonen3NC.fig` is th egraph of a non-central form on 3 variabvles.

`KuonenAndSaddlePoints\KuonenZetaHatvsQ.m` shows the linear approximation of the argument in a central case.  
`KuonenAndSaddlePoints\KuonenZetaHatvsQ2.m` shows the linear approximation of the argument in a non-central case.

`KuonenAndSaddlePoints\KuonenNonCentral.jpg` is a graph for a non-central case.

`KuonenAndSaddlePoints\CompareKuonenAlNaffouri` is an undone attempt to compare the saddlepoint approximations.

`Simon_Alouini\Simon_Alouini.m` compares the three analytical expressions and the MC simulation of the CDF of a particular indefinite form at zero. The mean is changed to produce a number of points and plot a graph. It seems that the analytical expressions produce the complement (1-P is used instead of P).

`Simon_Alouini\DifferencePSIM.m` and `Simon_Alouini\DifferenceP.m` show the same idea, but are seperated.

`Simon_Alouini\Data` contains some data files, a graph, and a screenshot of the input.

`Imhof/Imhof.tex` shows the derivation of Imhof's formula.

`Imhof/Data` shows some results.


`Imhof/Imhof_CDF_1962.m` plots the Imhof CDF of a QF in 50 vars with a mean of tens. This shows two things:
    - Imhof's formula is very powerful.
    - It tends to be less accurate at heads and tails (for N_int = 2000 for example).

`ImhofNMPDF.m` does the same for the PDF. Imhof mentions that the PDF integrand is (obviously) slower.

`Imhof/ImhofNM_Mohanad` is Mohanad's version of the implementation.

`Imhof/Imhof_Complex2Real_PDF_1962.m` converts a Hermitian form into a real form and computes the CDF.


`Mathai_Provost_Chi_Square_Expansion_PDF_1992.m` implements the expansion in chi-square densities.

`Al-Naffouri/Al_Naffouri_Complex_Central_2016.m` implements the PDF closed-form expression.

`Al-Naffouri/AlNaffouriSaddlepoint.jpg` and `AlNaffouriSaddlepoint.pdf` show an example of applying saddlepoint head and tail approximations.

`Al-Naffouri/Al_Naffouri_Complex_Non-Central_2016.m` aplies the saddlepoint approxiamtions to a non-central hermitian form.

`NaffouriRatio.m` and `NaffouriRatio.m` are failed attempts to implement the central ratioj formula.

`Lasserre/LasserreGloptiPoly.m` is my failed attempt to use gloptipoly to implement Lasserre.

`Lasserre/LasserreExample3.m` is another failed attempt to directly use SeDuMi.

`Lasserre/LasserreExample3.m` is another failed attempt to directly use SeDuMi.

The folder `Lasserre` contatins the necessary folders ot implemsent glopotipoly and sedumi and a dovumetnation pdf.

`Nadimi_Nadarjah_Gu` contains many fialed attempts and some data --- needs more checking.

`Nadimi_Nadarjah_Gu/Gu_2020.m` is an implementation of the closed-form PDF of Gu.

`Liu_et_al.m` is an implementation of Liu's 2009 moment matching method.

`Provost_Rudiuk/ProvostRudiuk.m` is a MATLAB implementation of the method.

`Provost_Rudiuk/Provost Rudiuk.jl` is a Julia implementation of the method.

`Hagedorn` contains Hagedorn trivariate simulations and data.


`Hagedorn/TrivariateChiSquaredSIM1.m` uses L2 to approximate the probability at the diagonal. This method is not efficient; instead we used again a grid in `Hagedorn/GridTest.m`

`Royen/Hdist.m` proves that the $H$ function is not a CDF.

`Royen/Royen1facNonCentral.m` computes the one-factorial rank 1- noncentral Royen bivariate distribution. The method is slow.

`Mathai_Provost` contains implementations of power series, Laguerre series, and expansion in chi-square densities.




