# Remaining Action Items and Future Questions

1. Conditional Distribution:
    - Given the values of $M$ quadratic forms $Y_I = x^TA_ix, i=1,\ldots,M$ where $x\sim \mathcal{N}(\mu, \Sigma)$, what is the distribution of $x$? $$f_{x|Y_1,\ldots,Y_m}(x|y_1,\ldots,y_m)=?$$
    - Algebraic Problem: What is the support of this distribution? 
        - It is an algebraic variety of dimension $N-M$ under some condition [Wikipedia](https://en.wikipedia.org/wiki/Dimension_of_an_algebraic_variety#Computation_of_the_dimension).
        - It is a submaninfold of a stronger condition.

2. Why do the formualae in Simon & Alouini's 2001 paper produce the $1-P$ instead of $P$? There is a follow up paper [Correction](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=1658230).

3. Why doesn't Mao & Todd's site formula (which agrees with the formula I derived) does not match the MC simulation?

4. Make a final decision on the Whittaker function implementation as it appears in Provost and Rudiuk's first PDF, in particular for the case of $L$ and $N-L$ being simulatanously even.

5. Add the citation count of each category in the formula type table so that it becomes "more balannced".

6. Complete the derivations / approach table (common themes).

7. Add the missing papers:
    1. [AFTER] Yunus
    1. [BEFORE] K. S. Miller, Multidimensional Gaussian Distributions. New York: Wiley, 1964. <span style="color:red"> PDFs and CDFs of statistical distributions derived from the Gaussian distribution </span>
    2.  [AFTER] R. K. Mallik, “On multivariate Rayleigh and exponential distributions,” IEEE Trans. Inform. Theory., vol. 49, no. 6, pp. 1499–1515, Jun. 2003. <span style="color:red"> multivariate probability distributions for the Rayleigh distribution were investigated </span>
    3.  [AFTER] C. C. Tan and N. C. Beaulieu, “Infinite series representations of the bivariate Rayleigh and Nakagami-m distributions,” IEEE Trans. Commun., vol. 45, no. 10, pp. 1159–1161, Oct 1997. <span style="color:red"> An infinite series representation (ISR) for the bivariate Rayleigh CDF, Certain forms of multivariate probability distributions for the Nakagami-m distribution </span>
    4. [AFTER] M. K. Simon and M.-S. Alouini, “A simple single integral representation of the bivariate Rayleigh distribution,” IEEE Commun. Lett., vol. 2, no. 5, pp. 128–130, May 1998. <span style="color:red">  A finite range single integral representation for the bivariate Rayleigh distribution </span>
    5. [BEFORE] D. Middleton, An Introduction to Statistical Communication Theory. New York: McGraw-Hill, 1964. <span style="color:red">  bivariate Rician CDF is given as an infinite summation </span>
    6. [AFTER] D. A. Zogas and G. K. Karagiannidis, “Infinite-series representations associated with the bivariate Rician distribution and their applications,” IEEE Trans. Commun., vol. 53, no. 11, pp. 1790–1794, Nov. 2005. <span style="color:red">  bivariate Rician PDF is given as an infinite summation </span>
    7.  [AFTER] M. K. Simon, “Comments on ”Infinite-series representations associated with the bivariate Rician distribution and their applications”,” IEEE Trans. Commun., vol. 54, no. 8, pp. 1511–1512, Aug. 2006. <span style="color:red">  bivariate Rician PDF is given as an infinite summation </span>
    8. [AFTER] P. Dharmawansa, N. Rajatheva, and C. Tellambura, “On the trivariate Rician distribution,” IEEE Trans. Commun., vol. 56, no. 12, pp. 1993–1997, Dec. 2008. <span style="color:red"> an infinite series representations of the PDF and CDF of the tri-variate Rician distribution, when the underlying Gaussian RVs have a tri-diagonal
    inverse covariance matrix </span>
    9. [AFTER] A. A. Abu-Dayya and N. C. Beaulieu, “Switched diversity on microcellular Ricean
    channels,” IEEE Trans. Veh. Technol., vol. 43, no. 4, pp. 970–976, Nov. 1994. <span style="color:red"> useful single integral representation for the bivariate Rician PDF </span>
    10.  [BEFORE] M. Nakagami, “The m-distribution, a general formula of intensity distribution of rapid fading,” Statistical Methods in Radio Wave Propagation, 1960. <span style="color:red">  Certain forms of multivariate probability distributions for the Nakagami-m distribution </span>
    11. [AFTER] J. Reig, L. Rubio, and N. Cardona, “Bivariate Nakagami-m distribution with arbitrary fading parameters,” Electronics Letters, vol. 38, no. 25, pp. 1715–1717, Dec. 2002. <span style="color:red">  Certain forms of multivariate probability distributions for the Nakagami-m distribution </span>
    12. [AFTER] G. K. Karagiannidis, D. A. Zogas, and S. A. Kotsopoulos, “On the multivariate Nakagami-m distribution with exponential correlation,” IEEE Trans. Commun., vol. 51, no. 8, pp. 1240–1244, Aug. 2003. <span style="color:red">  Certain forms of multivariate probability distributions for the Nakagami-m distribution </span>
    13. [AFTER] R. A. A. de Souza and M. D. Yacoub, “Bivariate Nakagami-m distribution with arbitrary correlation and fading parameters,” IEEE Trans. Wireless Commun., vol. 7, pp.
    5227–5232, Dec. 2008. <span style="color:red">  Certain forms of multivariate probability distributions for the Nakagami-m distribution </span>
    14. [AFTER] R. A. A. de Souza and M. D. Yacoub, “On the multivariate Nakagami-m distribution with arbitrary correlation and fading parameters,” in Proc. IEEE Int. Microwave and Optoelectronics Conf. (IMOC 2007)., Oct./Nov. 2007, pp. 812–816. <span style="color:red">  Certain forms of multivariate probability distributions for the Nakagami-m distribution </span>
    15. [AFTER] X. Zhang and N. C. Beaulieu, “Performance analysis of generalized selection combining in generalized correlated Nakagami-m fading,” IEEE Trans. Commun., vol. 54, no. 11, pp. 2103–2112, Nov. 2006. [40] <span style="color:red"> Generation of vars </span>
    16. [BEFORE] S. O. Rice, “Mathematical analysis of random noise,” Bell Systems Tech. J., vol. 23, pp. 282–332, 1944. <span style="color:red"> Bivariate Rayleigh for constant correaltion; finite expression </span>


8. Complete the supplementary material:
    1. Complete the formuala list.
    2. Create a seperate file for algorithms pseudo-codes.
    3. Create the library of codes so that we can add the links to the formula list.

9. Standardize the multivariate forms.
    - We cannot write them as linear combs of the same chi squares in the chi-squares.
    - We can standardize the Gaussian, in this case, there remains the permutation of the forms. 
    - This seems to be feasible for central forms. We used this "project" to prove that $I_K \otimes E_{ii}$ forms do not fall in the SimDiag categore except in a trivial case.

10. Kuonen's saddlepoint approximation:
    1. Derivation: Barndorff-Nielsen's papers (whom Kuonen cites) do not seem readable. 
        - Kuonen's thesis may provide an alternative.
    2. Implementation: For some points, the method requires the square root of a complex number to be later plugged in the standard normal CDF, or to divide by zero (see Quadratic Forms Working Draft/ zProblemsForLater).
        - Characterize this set in terms of the the parameters of the quadratic form.
        - Use Taylor's expansion to account for the missing region. This worked in the case of division by zero (a single point). 
        - A higher order approximation is needed for missing intervals. We have not finished the latter.

11. Royen's convolution:
    - Generalize Royen's 2007 convolution relaxing the non-singualrity condition on $\Sigma_k,\;k=1,\ldots,n$ to account for simultaneously diagonalizable positive definite forms.
    - Can we do that with a different number of variables?
        - Compare integral transforms.

12. Find Laverny's application. CHECK if its gammas are chi-squares. Try to implement Laverny. Is it a genralioztion of Laguerre expansion? (Take M=1)

13. Replicate Khammassi's work for Rician and Nakagami-$m$ fading.


Open Problems as they appear in the seminar:

1. **Problem 1**: Computation of General Quadratic Forms
    1. What are the limits/bounds on computational methods for computing quadratic forms?
    2. A generic method that performs reasonably ``well''?
    3.  Mathematical Statement: \textit{Given $M$ ``generalized'' quadratic forms}: $$Y_i =  x^T A_i x + b_i^T x + c_i,\quad i = 1 \ldots M$$ \textit{compute the joint CDF, joint PDF and joint moments}
    4. SUBPROBLEM: broad subcategories of Problem 1

2. **Problem 2**: Numerically Stable solutions of the generalized problem of moments
    1.  Lasserre explicitly mentions that what he proposes is terrible numerically. 
    2. Lasserre conjectures that using Hermite polynomials is superiour to using the canonical basis (which leads to usual moments)
    3. Mathematical Statement: \textit{Let $\Omega$ be a semi-algebraic set defined by polynomials $g_i(x), i = 1 \ldots M$. Let $\mu$ be a standard gaussian measure. Derive the semidefinite problem whose solution approximates $\mu(\Omega)$ the measure of the semialgebraic set, and whose variables are the projections of the gaussian measure on the hermite polynomials on the set $\Omega$}

3. **Problem 3**: Extend Khammassi's/Morales-Jimenez approximation to general (non-central) multivariate $\chi^2$ or general QFs
    1. *Let $x \sim \mathcal{CN}(\mu, \Sigma)$ and let $X = \begin{bmatrix}x_1 & x_2 & \ldots x_K\end{bmatrix}$ with $x_i$ independent samples of $x$. Let $Y = \text{diag}(XX^H)$ be the vector of the diagonal elements of $XX^H$. Given that $\Sigma$ can be represented in M-factorial form, derive explicit direct numerical integration formulae for the CDF PDF and other quantities of interest.*
    2. Smaller subproblems include $K=1, \mu\neq 0$ or $\mu = 0, K > 1$.

4. **Problem 4**: PDF of ratios without independence condition between Numerator and denominator
    1. Obtaining a PDF from the CDF that results from indefinite form expressions requires differentiating through the eigenvalues (roots of the characteristic function). Approximations with bounds or compact numerical approaches might be useful.
    2. Note roots of polynomial are continuous in its coefficients [Link1](https://arxiv.org/abs/2206.13013)
    [Link2](https://arxiv.org/abs/2206.13013)

5. **Problem 5**: Error Bounds on approximate methods
    1. *Let $Q \sim \sum_{i = 1}^N\lambda_i (x_i + h_i)^2$ and let $Q_A$ be a variate from the exponential family (gamma, chi square, gaussian ... etc.) or linear combinations thereof, derive (approximate) upper bounds for any of the of following:* $$\begin{gathered}
                \mathbb{E}[|Q - Q_A|^2] \\
                \mathbb{P}[|Q - Q_A| > \epsilon]\quad \forall \epsilon \in \mathbb{R}^+ \\
                \int (f_Q(q) - f_{Q_A}(q))^2 dq
            \end{gathered}$$
    2. Same question for the Saddle point approximations

6. **Problem 6**: Asymbolic Calculation of Morales-Jimenez/Royen's coefficients
    1. The current method to compute the coefficients used by Moralez-Jimenez \cite{morales-jimenezDiagonalDistributionComplex2011}\footfullcite{morales-jimenezDiagonalDistributionComplex2011} (which can be utilized for closely related Royen's papers) is symbolic and hence computationally very inefficient as the number of variables increases.
    2. Can we do this asymbollicaly? 