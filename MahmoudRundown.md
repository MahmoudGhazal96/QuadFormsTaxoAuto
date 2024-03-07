# Mahmoud's Tree of Questions
```
For each formula `f`:
    1. Do we include `f` in the main text
    2. a. Should we talk about the derivation?
       b. If Yes? Should we use the original formulation while talking about the derivation?
    3. a. Should talk about the application? 
    4. What are our criticisms?
```

### How to answer question 1?
1. Is it useful?
2. Is it ugly? Do we want an ugliness scale? (1 - 10)
3. Is there something "interesting" to say about it?
    - Can they "use" it? Use it as in apply it to their own research, not in the engineering sense of applying it to a practical problem?
4. Criticisms? Commentary? Speculations?

# Papers
#### 1. A. Gardini, F. Greco, and C. Trivisano, “The Mellin Transform to Manage Quadratic Forms in Normal Random Variables,” Journal of Computational and Graphical Statistics, vol. 31, no. 4, pp. 1416–1425, Oct. 2, 2022. doi: 10.1080/10618600.2022.2034639. [Online]. Available: https://www.tandfonline.com/doi/full/10.1080/10618600.2022.2034639 PD Single

- Main formula can be replaced by the phrase: "Gardini numerically inverts the Mellin transform", since he didn't use anything other than the standard inversion formula.
- The bounds may actually be useful to truncate the series and the improper integral; this depends on their tightness. 
- Another factor that must be taken into consideration is the presence of recent research results, at least in the first draft (to make the text look newer!)

<span style="color:red"> Should we look for more recent single quadratic forms papers?</span> YES

##### **Answers** 
1. Do we include the formula in the main text? If we find no more recent formulae dealing with single quadratic forms we include it in the main text. --> YES
2. a. We include a synopsys of the derivation of which the main points are:
    - Gardini applies the Mellin transform to the Expansion in Chi squared densities (derived in Ruben or Mathai).
    - The inverse transform is given by some formula, which is anayltically intractable.
    - Gardini uses numerical rectangular inversion and derives some bounds for the accuarcy.
    - There is an error control procedure. **ONE LINER SUMMARRY NEEDED**
3. NO APPLICATIONS IN PAPER
4. Criticisms? Commentary? Speculations?
    - Straightforward derivation. 
    - When are the bounds tight?

#### 2. A. Gardini, F. Greco, and C. Trivisano, “The Mellin Transform to Manage Quadratic Forms in Normal Random Variables,” Journal of Computational and Graphical Statistics, vol. 31, no. 4, pp. 1416–1425, Oct. 2, 2022. doi: 10.1080/10618600.2022.2034639. [Online]. Available: https://www.tandfonline.com/doi/full/10.1080/10618600.2022.2034639 PD Ratios

- Same 

#### 3. M. Khammassi, A. Kammoun, and M.-S. Alouini. “A New Analytical Approximation of the Fluid Antenna System Channel.” arXiv: 2203.09318 [cs, eess, math]. (Mar. 17, 2022), [Online]. Available: http://arxiv.org/abs/2203.09318 (visited on 06/20/2022), preprint

##### **Answers**
1. There are actually two formulas: First Stage and Second Stage.
    - Mahmoud says NO: The author after inspection of her code (that she kindly shared!) appears to not have used the formula directly. She actually just directly  "montecarloed" the problem. We don't want Montecarlo. She proceeds to simplify this via another approximation to a second stage. Which she actually uses.
2. YES. We want to talk about her derivation. Mahmoud wants to unify it with Royen (M-factorial) and Beaulieu and Hemachandra (2011). 1-factorial pushed further.

3. We should mention the applications in some other part of the text. Fluidic Antenna systmes are pushing the range of computable no. of forms in the QF literature.

4. Criticisms? Commentary? Speculations?
    - Can the second stage approximation be perceived as the distribution of some Rayleigh variables or only as a maximum of Rayleigh distributions.
    - What is the numeric stability of the 1st stage approximation CDF integrals?
    - Performance gains of the 1st stage approximation? Depends on $\epsilon\text{-rank}$.

#### 4. O. Laverny, E. Masiello, V. Maume-Deschamps, and D. Rulli`ere, “Estimation of multivariate generalized gamma convolutions through Laguerre expansions,” Jul. 23, 2021. arXiv: 2103 . 03200 [math, stat]. [Online]. Available: http://arxiv.org/abs/2103.03200 (visited on 11/15/2021)

##### **Answers**
1. YES. It is the only simultaneously diagonlizable case multivariate case. The only meaningful non $\chi^2$ Multivariate case.
2. We want the derivation.
    - Can we make it appear as a generalizaiton of the Laguerre expansion from single quadratic forms (in Mathai).
3. FIND THE APPLICATION
4.  Criticisms? Commentary? Speculations?
    - Should we implement (or find his implementation)? YES Find his implementation. 

We should note that applying the reported formula to QFs was not the authors original target. It is the result of some manipulations we applied to the resulting formuale.

- DO Laverny's derivation. In his context and in our context(notation).

#### 5. D. Gu, “On The Quotient of a Centralized and a Non-centralized Complex Gaussian Random Variable,” Journal of Research of the National Institute of Standards and Technology, vol. 125, p. 125 030, Sep. 23, 2020. doi: 10.6028/jres.125.030. [Online]. Available: https://nvlpubs.nist.gov/nistpubs/jres/125/jres.125.030.pdf (visited on 06/21/2022)

##### **Answers**
1. Include but remember if we need to cut things down.
2. YES. But look at combining "derivation synopsis" section with Nadimi / Nadarajah and Kwong.
3. <span style="color: lime;font-weight: bold;font-size: 14pt"> FIND AND FILL UP</span>
4. Criticisms? Commentary? Speculations? NONE

#### 6. M. Tekinay and C. Beard, “Moments of the quadrivariate Rayleigh distribution with applications for diversity receivers,” Annals of Telecommunications, vol. 75, no. 7, pp. 447–459, Aug. 1, 2020. doi: 10.1007/s12243-020-00755-6. [Online]. Available: https://doi.org/10.1007/s12243-020-00755-6 (visited on 06/20/2022)

##### **Answers**
1. NO. Because its ugly. Multiple infinite sums.
    - Is there a clear truncation method? ARe there bounds? NO
    - Can we make it nicer?
2. Synopsis of Derivation:
    - Use PDF from the 1960 reference. Replace the exponential of the cosine with infinite fourier series of which the coefficients seem to be modified bessel functions. $$e^{A\cos x} = I_0(A) + 2\sum_{a = 1}^\infty I_a(A) \cos {a x}$$
    - Marginalize over the phases to achieve his formula.
    - To get CDF expand the bessel functions collect each variable with its $e^{-x^2}$ and then integrate. This should give incomplete gamma functions.

4. Criticisms? Commentary? Speculations?
    - The Condition of real correlation parameters on the Complex covariance matrix leads to a block marix structure (if we sort real alone and imag alone). This means the inverse (i.e. precision matrix) is also block in structure. If we further make the matrix toeplitz then we get another specialized structure in the precision matrix. for the 4x4 case this can be represented by six parameters.

#### 7. H. Zhang, J. Shen, and Z. Wu. “An efficient and accurate approximation to the distribution of quadratic forms of Gaussian variables.” arXiv: 2005.00905 [q-bio, stat]. (Sep. 23, 2020), [Online]. Available: http://arxiv.org/abs/2005.00905 (visited on 01/12/2023), preprint |||||||| 
*H. Zhang, J. Shen, and Z. Wu, “A Fast and Accurate Approximation to the Distributions of Quadratic Forms of Gaussian Variables,” Journal of Computational and Graphical Statistics, vol. 31, no. 1, pp. 304–311, Jan. 2, 2022. doi: 10.1080/10618600.2021.2000423. [Online]. Available: https://www.tandfonline.com/doi/full/10.1080/10618600.2021.2000423 (visited on 04/01/2023)*

##### **Answers**

1. YES Final formula is simple and compact.
2. YES
3. WE NEED TO Examine the proposed synthetic data he is generating.
4. Criticisms? Commentary? Speculations?
    - No real dataset.
    - Update Duchesne's work to include comparison of newer moment matching methods.

#### 8. P. S. Bithas, A. G. Kanatas, D. B. da Costa, P. K. Upadhyay, and A. Hatziefremidis, “Novel results for the multivariate ricean distribution with non-identical parameters,” IEEE Transactions on Vehicular Technology, vol. 68, no. 5, pp. 5129–5133, 2019. doi: 10.1109/TVT.2019.2902321

##### **Answers**

1. YES
2. In context with Beaulieu and Hemachandra and Royen's one factorials.
3. Fading channels. One of the applications we will discuss in more detail.
4. Comments
    - Generalization of Beaulieu and Hemachandra 2011 paper.
    - Good from application point of view.
    - Condition is vacously/always satisfied. We can reformulate problem in more convenient way.

#### 9. T. Chen and T. Lumley, “Numerical evaluation of methods approximating the distribution of a large quadratic form in normal variables,” Computational Statistics & Data Analysis, vol. 139, pp. 75–81, Nov. 2019. doi: 10.1016/j.csda.2019.05.002. [Online]. Available: https://linkinghub.elsevier.com/retrieve/pii/S0167947319301136

##### **Answers**

1. This can be divided divided into two questions: Should we include the new linear combination? Should we include the algorithm (for diagonalization and obtaining k dominant eigenvalues)?
    1. YES.
    2. NO. Just cite.
2. The whole idea is: replace by a smaller linear combinatiom and convolute using another method.
3. NO. We will dedicate a section in the larger chapter for that.
4. Comments
    - The algorithm is not easy.

#### 10. P. Ramirez-Espinosa, L. Moreno-Pozas, J. F. Paris, J. A. Cortes, and E. Martos-Naya, “A New Approach to the Statistical Analysis of Non-Central Complex Gaussian Quadratic Forms With Applications,” IEEE Transactions on Vehicular Technology, vol. 68, no. 7, pp. 6734–6746, Jul. 2019. doi: 10.1109/TVT.2019.2916725. [Online]. Available: https://ieeexplore.ieee.org/document/8715664/ (visited on 04/06/2022) (cit. on p. 11).

##### **Answers**
 1. YES. It is fairly recent, and compared to other formulae that are quan of sequences of RVs, the formula is mild.
 2. YES. The method is relatively easy.
 3. NO. Classical MRC application.
 4. Comments:
    - Can we use the MSE to choose an $m$?

#### 11. P. Ram´ırez-Espinosa, D. Morales-Jimenez, J. A. Cort´es, J. F. Paris, and E. Martos-Naya, “New Approximation to Distribution of Positive RVs Applied to Gaussian Quadratic Forms,” IEEE Signal Processing Letters, vol. 26, no. 6, pp. 923–927, Jun. 2019. doi: 10.1109/LSP.2019.2912295

##### **Answers**

1. YES. It is fairly recent, and compared to other formulae that are quan of sequences of RVs, the formula is mild.
 2. YES. The method is relatively easy.
 3. The paper is a short letter; no detailed application.
 4. Comments:
    - The method works for any positive RV.
    - Can it be generalized to indefinite forms? To multivariate positive?

#### 12. M. Wiegand and S. Nadarajah, “Series approximations for Rayleigh distributions of arbitrary dimensions and covariance matrices,” Signal Processing, vol. 165, pp. 20–29, Dec. 1, 2019. doi: 10.1016/j.sigpro.2019.06.035. [Online]. Available: https://www.sciencedirect.com/science/article/pii/S0165168419302439

#### 15. M. Wiegand and S. Nadarajah, “A series representation for multidimensional Rayleigh distributions,” International Journal of Communication Systems, vol. 31, no. 6, e3510, 2018. doi: 10.1002/dac.3510. [Online]. Available: https://onlinelibrary.wiley.com/doi/abs/10.1002/dac.3510

##### **Answers**

1. If we can simplify the formula.
2. YES, it seems that the derivation is similar to Tekinay. 2018: "In this note, we generalise the results of Beard and Tekinay for quadrivariate random variables to cases of unconstrained order and provide a simple algorithm for evaluation."
3. NO.
4. Comments:
    - Read their comparison part.
    - No need to report both formuale, as the 2019 paper is a relaxation of the Toeplitz conditon. 

#### 13. S. Nadarajah and H. S. Kwong, “A note on “On the ratio of independent complex Gaussian random variables”,”Multidimensional Systems and Signal Processing, vol. 29, no. 4, pp. 1839–1843, Oct. 2018. doi: 10.1007/s11045-017-0537-1. [Online]. Available: http://link.springer.com/10.1007/s11045-017-0537-1

##### **Answers**

1. YES, the formula is simple.
2. YES, we can talk about the 3 papers (Nadarjah & Kwong, Nadimi, and Gu) together.
3. NO detailed application.
4. Comments:
    - None

#### 14. E. S. Nadimi, M. H. Ramezani, and V. Blanes-Vidal, “On the ratio of independent complex Gaussian random variables,” Multidimensional Systems and Signal Processing, vol. 29, no. 4, pp. 1553–1561, Oct. 1, 2018. doi: 10.1007/s11045-017-0519-3. [Online]. Available: https://doi.org/10.1007/s11045-017-0519-3 (visited on 06/21/2022)

##### **Answers**

1. YES, the formula is simple.
2. YES, we can talk about the 3 papers (Nadarjah & Kwong, Nadimi, and Gu) together.
3. NO detailed application; beware that the applications mentioned in the introduction may apply only to the ratio of complex Gaussians, not the moduli.
4. Comments:
    - None

#### 16. N. C. Beaulieu and Y. Zhang, “New Simplest Exact Forms for the 3-D and 4-D Multivariate Rayleigh PDFs With Applications to Antenna Array Geometries,” IEEE Transactions on Communications, vol. 65, no. 9, pp. 3976–3984, Sep. 2017. doi: 10.1109/TCOMM.2017.2709307 [MultiV: Trivariate Case]

#### 17.  N. C. Beaulieu and Y. Zhang, “New Simplest Exact Forms for the 3-D and 4-D Multivariate Rayleigh PDFs With Applications to Antenna Array Geometries,” IEEE Transactions on Communications, vol. 65, no. 9, pp. 3976–3984, Sep. 2017. doi: 10.1109/TCOMM.2017.2709307 [MultiV: Quadrivariate Case]


##### **Answers**

1. YES, the formula is relatively simple.
2. YES, it incorporates steps similar to the Gaussian integral we were working on.
3. YES, we can talk at least of usage of the outage probability for optimizing the antenna placement.
4. Comments:
    - Read its comparison with Weigand.

#### 18. J.-B. Lasserre. “Computing gaussian & exponential measures of semi-algebraic sets.” arXiv: 1508 . 06132 [math]. (Jul. 10, 2017), [Online]. Available: http://arxiv.org/abs/1508.06132 

##### **Answers**

1. YES, the formula is not simple, but it must be reported for covering general multivariate forms.
2. YES, so that the formual is better understood.
3. NO detailed application.
4. Comments:
    - Replicate using the basis of Hermite polynomials.
    - Does the particular case of quadratic polynomials offer a simplification we aren't aware of?

#### 19. G. Cui, X. Yu, S. Iommelli, and L. Kong, “Exact Distribution for the Product of Two Correlated Gaussian Random Variables,” IEEE Signal Processing Letters, vol. 23, no. 11, pp. 1662–1666, Nov. 2016. doi:10.1109/LSP.2016.2614539 

##### **Answers**

1. NO, it is a very particular case with an infinite series in Bessel functions.
2. NO need.
3. NO detailed application.
4. Comments:
    - Can we rederive it from other formula(e)? This is not trivial, as I don't recall a formula with modified Bessel functions of the second kind.
    - How much is it more efficient than other formulae? In other words, is it useful to express a product of Gaussians as a linear combination of chi-squares?

#### 20. T. Y. Al-Naffouri, M. Moinuddin, N. Ajeeb, B. Hassibi, and A. L. Moustakas, “On the Distribution of Indefinite Quadratic Forms in Gaussian Random Variables,” IEEE Transactions on Communications, vol. 64, no. 1, pp. 153–165, Jan. 2016. doi: 10.1109/TCOMM.2015.2496592 [SingleV: Central Complex]

##### **Answers**

1. YES.
2. YES, to reveal the simplification a special case yields.
3. NO, talk later.
4. Comments: 
    - Rederive the formula from finite expressions in Mathai.

#### 21. T. Y. Al-Naffouri, M. Moinuddin, N. Ajeeb, B. Hassibi, and A. L. Moustakas, “On the Distribution of Indefinite Quadratic Forms in Gaussian Random Variables,” IEEE Transactions on Communications, vol. 64, no. 1, pp. 153–165, Jan. 2016. doi: 10.1109/TCOMM.2015.2496592 [SingleV: Non-central Complex / Saddlepoint Approx]

##### **Answers**

1. YES.
2. YES, we've already gone through that.
3. NO, talk later.
4. Comments:
    - Can we give a clear criterion for the choice between tail and head formulae? 
        - From the derivation perspective
        - From an implementation persective (choice of the cutoff point)

#### 22. T. Y. Al-Naffouri, M. Moinuddin, N. Ajeeb, B. Hassibi, and A. L. Moustakas, “On the Distribution of Indefinite Quadratic Forms in Gaussian Random Variables,” IEEE Transactions on Communications, vol. 64, no. 1, pp. 153–165, Jan. 2016. doi: 10.1109/TCOMM.2015.2496592 [SingleV: Central Real / Saddlepoint Approx]

##### **Answers**

1. YES.
2. No need, since it's similar to the complex case. (Mention this derivation style once.)
3. NO
4. Comments:
    - Do we need a head/tail distinction?
    - Can we implement the non-central generalization?
        - If yes, what's the point of the complex case?

#### 23. T. Y. Al-Naffouri, M. Moinuddin, N. Ajeeb, B. Hassibi, and A. L. Moustakas, “On the Distribution of Indefinite Quadratic Forms in Gaussian Random Variables,” IEEE Transactions on Communications, vol. 64, no. 1, pp. 153–165, Jan. 2016. doi: 10.1109/TCOMM.2015.2496592 [Ratio: Central Real]

##### **Answers**

1. YES, due to the lack of formulae in the case of dependent num/den.
2. YES, the proof is nothing but two lines.
3. NO
4. Comments:
    - What's the point of singling out the central complex case? Is it something to do with the nature of the application, or the complexity?


#### 23.5. T. Y. Al-Naffouri, M. Moinuddin, N. Ajeeb, B. Hassibi, and A. L. Moustakas, “On the Distribution of Indefinite Quadratic Forms in Gaussian Random Variables,” IEEE Transactions on Communications, vol. 64, no. 1, pp. 153–165, Jan. 2016. doi: 10.1109/TCOMM.2015.2496592 [Bivaraite: Simultaneously Diagonalizable]

##### **Answers**

1. Can we write a clear formula, not just "do this and that"? Anyway, it's worth mentioning so that the SIM DIAG category contains another formula.



#### 24. T. Royen, “Non-Central Multivariate Chi-Square and Gamma Distributions,” Jul. 5, 2016. arXiv: 1604.06906 [math, stat]. [Online]. Available: http://arxiv.org/abs/1604.06906 (visited on 04/08/2021) [$p$-variate intergal]

##### **Answers**

1. YES, the formula is relatively simple.
2. YES, try to grasp the "unifying soul" of Royen's proofs.
3. NO.
4. Comments:
    - Despite being simpler than $(p-1)$-integral, it may not be as practical. Royen mentions that the $(p-1)$-case is computable for $p\leq 3$.

#### 24. T. Royen, “Non-Central Multivariate Chi-Square and Gamma Distributions,” Jul. 5, 2016. arXiv: 1604.06906 [math, stat]. [Online]. Available: http://arxiv.org/abs/1604.06906 (visited on 04/08/2021) [$(p-1)$-variate intergal]

##### **Answers**

1. YES, despite being mostrous. See 4.
2. YES, try to grasp the "unifying soul" of Royen's proofs.
3. NO.
4. Comments:
    - Compare with 2007 convolution last section; try to wrtie the better formula if there is any difference.


#### 25. W.-J. Yan and W.-X. Ren, “Circularly-symmetric complex normal ratio distribution for scalar transmissibility functions. Part II: Probabilistic model and validation,” Mechanical Systems and Signal Processing, vol. 80, pp. 78–98, Dec. 2016. doi: 10.1016/j.ymssp.2016.02.068. [Online]. Available: https://linkinghub.elsevier.com/retrieve/pii/S0888327016001242 

##### **Answers**

0. I think we report Part I not II.
1. YES.
2. Check if this particular formula is applied.
3. Comments:
    - Since it is a simple corollary, it may be presented as a sort of verification. We need to check somehow if the authors were the first to publish this case.
    - It isn't a special case of the group (Nadajah, Nadimi and Gu) since the numerator and the denominator are correlated.

#### 26. T. Dickhaus and T. Royen, “A survey on multivariate chi-square distributions and their applications in testing multiple hypotheses,” Statistics, vol. 49, no. 2, pp. 427–454, Mar. 4, 2015. doi: 10.1080/02331888.2014.993639. [Online]. Available: http://www.tandfonline.com/doi/abs/10.1080/02331888.2014.993639 [real one-factorial]

##### **Answers**

1. YES, we couldn't find the "real one-factorial case" in any other available paper.
2. YES, inspect the effect of the relaxation of the positivity of the diagonal matrix in an $m$-factorial factorization.
3. Check if the particuar case has an application.
4. Comments: NONE

#### 26.5. T. Dickhaus and T. Royen, “A survey on multivariate chi-square distributions and their applications in testing multiple hypotheses,” Statistics, vol. 49, no. 2, pp. 427–454, Mar. 4, 2015. doi: 10.1080/02331888.2014.993639. [Online]. Available: http://www.tandfonline.com/doi/abs/10.1080/02331888.2014.993639 [other cases]

##### **Answers**

1. Add Jensen's csae; report Jensen's paper.

#### 27. Y. Bao and R. Kan, “On the moments of ratios of quadratic forms in normal random variables,” Journal of Multivariate Analysis, vol. 117, pp. 229–245, May 1, 2013. doi: 10 . 1016 / j . jmva . 2013 . 03 . 002. [Online]. Available: https : //www.sciencedirect.com/science/article/pii/S0047259X13000298

##### **Answers**

1. YES, at least one formula.
2. NO.
3. NO detailed application.
4. Comments: 
    - Check the algorithm.
    - Report older results.

#### 28. H.-T. Ha, “An accurate approximation to the distribution of a linear combination of non-central chi-square random variables,” REVSTAT-Statistical Journal, vol. 11, no. 3, pp. 231–254, 2013

##### **Answers**

1. NO, the formula is monstrous.
2. YES, so that we demonstrate it is a sequence of RVs.
3. NO detailed application.
4. Comments: 
    - Can we generalize to multivariate forms?

#### 29. A. Joarder and M. Omar, “Exact distribution of the sum of two correlated chi-square variables and its application,” Kuwait Journal of Science, vol. 40, Sep. 1, 2013

##### **Answers**

1. NO, the form is very specific.
2. NO, for the same reason.
3. YES, mention the statistical application.
4. Comments: 
    - Can we rederive the formula from Simon's 2006 handbook - Linear Combinations of 2 chi-squares? 
    - What is the difference? Is it evdient whenever we write the form as a linear combination of independent chi-squares?

#### 30. Z. Mao and M. Todd, “A model for quantifying uncertainty in the estimation of noise-contaminated measurements of transmissibility,” Mechanical Systems and Signal Processing, Interdisciplinary and Integration Aspects in Structural Health Monitoring, vol. 28, pp. 470–481, Apr. 1, 2012. doi: 10.1016/j.ymssp.2011.10.002. [Online]. Available: https://www.sciencedirect.com/science/article/pii/S0888327011003992

##### **Answers**

1. YES, it is a closed-form expression.
2. YES.
3. YES, mention the transmissivity application. 
4. Comments: 
    - Check again the implementation.
    - Check again the derivation of the formula.

#### 31. A. A. Mohsenipour, “On the Distribution of Quadratic Expressions in Various Types of Random Vectors,” Nov. 2012

##### **Answers**

0. Cite the papers instead of the thesis.
1. NO, on top of being an approximation, the expressions are monstrous.
2. YES, mention he convolutes PD moment matching methods to obtain formulae for indefnite forms.
3. NO detailed application.
4. Comments: NONE

#### 32. K. T. Hemachandra and N. C. Beaulieu, “Novel Representations for the Equicorrelated Multivariate Non-Central Chi-Square Distribution and Applications to MIMO Systems in Correlated Rician Fading,” IEEE Transactions on Communications, vol. 59, no. 9, pp. 2349–2354, Sep. 2011. doi: 10.1109/TCOMM.2011.062311.100108

##### **Answers**

1. YES, it is a single integral.
2. YES, in light of Beaulieu and Hemachandra 2011.
3. NO, we'll elaborate on the MIMO application.
4. Comments:
    - What's the difference from Beaulieu and Hemachandra
        - Derivation-wise
        - Application-wise

##### 33. N. O’Donoughue and J. M. F. Moura, “On the product of independent complex gaussians,” IEEE Transactions on Signal Processing, vol. 60, no. 3, pp. 1050–1063, 2012. doi: 10.1109/TSP.2011.2177264

***NOT** in our scope*:
1. Product of independent complex Gaussians is not a Hermitian form.
2. Squared modulus of the product is a qaurtic polynomial.

#### 34. N. C. Beaulieu and K. T. Hemachandra, “Novel Representations for the Bivariate Rician Distribution,” IEEE Transactions on Communications, vol. 59, no. 11, pp. 2951–2954, Nov. 2011. doi: 10.1109/TCOMM.2011.092011.09

##### **Answers**

1. NO, it is just a special case of the $M$-variate correlated Rician in their next paper (36).
2. YES.
3. NO, 
4. Comments: NONE

#### 35. N. C. Beaulieu and K. T. Hemachandra, “Novel simple representations for Gaussian class multivariate distributions with generalized correlation,” IEEE Transactions on Information Theory, vol. 57, no. 12, pp. 8072–8083, 2011 [Multivariate Rayleigh]

##### **Answers**

1. YES, it is a single integral.
2. Mention the derivation for the first case, and talk about the "generalization".
3. NO, we'll elaborate in the MIMO application.
4. Comments: Compare it with Royen 1991.

#### 36. N. C. Beaulieu and K. T. Hemachandra, “Novel simple representations for Gaussian class multivariate distributions with generalized correlation,” IEEE Transactions on Information Theory, vol. 57, no. 12, pp. 8072–8083, 2011 [Multivariate Rician]

##### **Answers**

1. YES, it is a single integral.
2. Mention the derivation for the first case, and talk about the "generalization".
3. NO, we'll elaborate in the MIMO application.
4. Comments: NONE

#### 37. N. C. Beaulieu and K. T. Hemachandra, “Novel simple representations for Gaussian class multivariate distributions with generalized correlation,” IEEE Transactions on Information Theory, vol. 57, no. 12, pp. 8072–8083, 2011 [Multivariate Nakagami-m]

##### **Answers**

1. YES, it is a single integral.
2. Mention the derivation for the first case, and talk about the "generalization".
3. NO, we'll elaborate in the MIMO application.
4. Comments: NONE

#### 38.  N. C. Beaulieu and K. T. Hemachandra, “Novel simple representations for Gaussian class multivariate distributions with generalized correlation,” IEEE Transactions on Information Theory, vol. 57, no. 12, pp. 8072–8083, 2011 [Multivariate Generalized Rician]

##### **Answers**

1. YES, it is a single integral.
2. Mention the derivation for the first case, and talk about the "generalization".
3. NO, we'll elaborate in the MIMO application.
4. Comments: NONE

#### 39. D. Morales-Jimenez, J. F. Paris, J. T. Entrambasaguas, and K.-K. Wong, “On the Diagonal Distribution of a Complex Wishart Matrix and its Application to the Analysis of MIMO Systems,” IEEE Transactions on Communications, vol. 59, no. 12, pp. 3475–3484, Dec. 2011. doi: 10.1109/TCOMM.2011.100611.100641. [Online]. Available: http://ieeexplore.ieee.org/document/6047541/ 

##### **Answers**

1. Yes, it covers a braod range.
2. Yes, in light of Royen.
3. NO, we'll elaborate in the MIMO application.
4. Comments:
    - Calculate the intersection formula, i.e., when the correlation matrix is real.

#### 40. H. Liu, Y. Tang, and H. H. Zhang, “A new chi-square approximation to the distribution of non-negative definite quadratic forms in non-central normal variables,” Computational Statistics and Data Analysis, vol. 53, no. 4, pp. 853–856, 2009. doi: https://doi.org/10.1016/j.csda.2008.11.025. [Online]. Available: https://www.sciencedirect.com/science/article/pii/S0167947308005653

##### **Answers**

1. YES, it is one of the most cited papers.
2. YES.
3. NO, we'll elaborate in the genetics application.
4. Comments:
    - A more thorough study, theoretically and numerically, is useful as it is widely applied.

####  41. P. Dharmawansa and M. R. McKay, “Diagonal distribution of a complex non-central Wishart matrix: A new trivariate non-central chi-squared density,” Journal of Multivariate Analysis, vol. 100, no. 4, pp. 561–580, Apr. 1, 2009. doi: 10.1016/j.jmva.2008.06.007. [Online]. Available: https://www.sciencedirect.com/science/article/pii/S0047259X08001577 

##### **Answers**

1. NO, the formula is monstrous.
2. NO need, we will have given a large chunk of proofs.
3. NO, we'll elaborate in the MIMO application.
4. Comments:
    - Compare with Royen 2016 complex.

#### 42. P. Dharmawansa, N. Rajatheva, and C. Tellambura, “New series representation for the trivariate non-central chi-squared distribution,” IEEE Transactions on Communications, vol. 57, no. 3, pp. 665–675, Mar. 2009. doi: 10.1109/TCOMM.2009.03.070083

##### **Answers**

1. NO, the formula is monstrous.
2. NO need, we will have given a large chunk of proofs.
3. NO, we'll elaborate in the MIMO application.
4. Comments:
    - Compare with the complex paper (with McKay).

#### 43. K. Peppas and N. C. Sagias, “A trivariate nakagami-m distribution with arbitrary covariance matrix and applications to generalized-selection diversity receivers,” IEEE Transactions on Communications, vol. 57, no. 7, pp. 1896–1902, Jul. 2009. doi: 10.1109/TCOMM.2009.07.070071

##### **Answers**

1. NO, 4 nested infinite summations.
2. Yes, in light of Hagedorn.
3. NO, we'll elaborate in the MIMO application.
4. Comments: NONE

#### 44. G. A. Ropokis, A. A. Rontogiannis, and P. T. Mathiopoulos, “Quadratic forms in normal RVs: Theory and applications to OSTBC over hoyt fading channels,” IEEE Transactions on Wireless Communications, vol. 7, no. 12, pp. 5009–5019, Dec. 2008. doi: 10.1109/T-WC.2008.070830

##### **Answers**

1. YES, it demonstarates that the expansion in chi-square densities is still relevant - 46 years after Ruben.
2. YES, to demonstrate the need of even degrees of freedom.
3. NO, we'll elaborate in the MIMO application.
4. Comments:
    - Can we gereralize to odd degrees?
    
#### 45. T. Royen, “Integral Representations and Approximations for Multivariate Gamma Distributions,” Annals of the Institute of Statistical Mathematics, vol. 59, no. 3, pp. 499–513, Sep. 11, 2007. doi: 10.1007/s10463-006-0057-5. [Online]. Available: http://link.springer.com/10.1007/s10463-006-0057-5

It must be removed as it is solely MC. We can just cite and mention that.

#### 46. T. Royen. “Integral representations for convolutions of non-central multivariate gamma distributions.” arXiv: 0704.0539 [math, stat]. (Apr. 4, 2007), [Online]. Available: http://arxiv.org/abs/0704.0539 (visited on 06/20/2022), preprint

##### **Answers**

0. Cite the published version.
1. YES, it is "generalized Royen", so cite at least one formula from the three.
2. NO need.
3. NO detailed application.
4. Comments: 
    - If we can relax the non-singularity condition on $\Sigma_k, k=1.\ldots, n$, we can account for the simultaneously diagonalizable case.

#### 47. G. N. Tavares and L. M. Tavares, “On the Statistics of the Sum of Squared Complex Gaussian Random Variables,”IEEE Transactions on Communications, vol. 55, no. 10, pp. 1857–1862, Oct. 2007. doi: 10.1109/TCOMM.2007.906387

##### **Answers**

1. NO, it is a very spoecific.
2. NO need.
3. NO detailed application.
4. Comments: 
    - If we can relax the non-singularity condition on $\Sigma_k, k=1.\ldots, n$, we can account for the simultaneously diagonalizable case.

#### 48. M. Hagedorn, P. J. Smith, P. J. Bones, R. P. Millane, and D. Pairman, “A trivariate chi-squared distribution derived from the complex Wishart distribution,” Journal of Multivariate Analysis, vol. 97, no. 3, pp. 655–674, Mar. 1, 2006. doi: 10.1016/j.jmva.2005.05.014. [Online]. Available: https://www.sciencedirect.com/science/article/pii/S0047259X05000795 (visited on 04/08/2021) [Trivariate]

##### **Answers**

1. YES, since we implemented it.
2. YES. They convert into real and start from the joint Gaussian density, integrating over the intersection of hypercylinderical regions.
3. NO, we'll elaborate in the MIMO application.
4. Commments:
    - Implement using a numerical modified Bessel function.

#### 49. M. Hagedorn, P. J. Smith, P. J. Bones, R. P. Millane, and D. Pairman, “A trivariate chi-squared distribution derived from the complex Wishart distribution,” Journal of Multivariate Analysis, vol. 97, no. 3, pp. 655–674, Mar. 1, 2006. doi: 10.1016/j.jmva.2005.05.014. [Online]. Available: https://www.sciencedirect.com/science/article/pii/S0047259X05000795 (visited on 04/08/2021) [Bivariate]

##### **Answers**

1. YES, since it is used by Mao and Todd.
2. YES, using the trivariate formula.
3. NO, we'll elaborate in the MIMO application.
4. Commments: NONE.

#### 50. Y. Chen and C. Tellambura, “Infinite series representations of the trivariate and quadrivariate Rayleigh distribution and their applications,” IEEE Transactions on Communications, vol. 53, no. 12, pp. 2092–2101, Dec. 2005. doi: 10.1109/TCOMM.2005.860059 [Trivariate]

##### **Answers**

1. YES, since its proof is easy.
2. YES. 
3. NO, we'll elaborate in the MIMO application.
4. Comments:
    - Does the writer allow a cross correlation in the applications?
    - In general, how much is the assumpton of zero cross-correlation (as in Wiegand and Tekinay) realistic?
    - Report the paper from whcih he takes the PDF from.

#### 51. Y. Chen and C. Tellambura, “Infinite series representations of the trivariate and quadrivariate Rayleigh distribution and their applications,” IEEE Transactions on Communications, vol. 53, no. 12, pp. 2092–2101, Dec. 2005. doi: 10.1109/TCOMM.2005.860059 [Quadrivariate]
 
##### **Answers**

1. NO, since we will have given a sample of the paper (it is old now).
2. YES, as an easy way to escape writing the formula.
3. NO, we'll elaborate in the MIMO application.
4. Comments:
    - Why is it necessary to assume an off-diagonal zero in the precision matrix?
    

#### 52. H. Holm and M.-S. Alouini, “Sum and difference of two squared correlated Nakagami variates in connection with the McKay distribution,” IEEE Transactions on Communications, vol. 52, no. 8, pp. 1367–1376, Aug. 2004. doi: 10.1109/TCOMM.2004.833019

*We ended up not reporting this since the interesting case (gamma -> chi-square) is reported in Simon's 2006 handbook.*

*Simon's handbook presents a **dilemma** for us:*
- The formulae are already in a handbook. BUT they are not written in our unified notation, as he allows a scale parameter in the chi-square distribution.
- He does not cite the original authors.
- Chasing the original authors is not an easy task; we do not know the manipulations he used to present the final formulae.

#### 53. M. Simon and M.-S. Alouini, “On the difference of two chi-square variates with application to outage probability computation,” IEEE Transactions on Communications, vol. 49, no. 11, pp. 1946–1954, Nov. 2001. doi: 10.1109/26.966071

##### **Answers**

1. YES, at least one formula.
2. NO need.
3. NO, we'll elaborate in the MIMO application.
4. Comments:
    - Check the follow up correction paper.
    - Check why the formulae are giving the CCDF instaed of the CDF.


#### 54. A. Sch¨one and W. Schmid, “On the Joint Distribution of a Quadratic and a Linear Form in Normal Variables,” Journal of Multivariate Analysis, vol. 72, no. 2, pp. 163–182, Feb. 1, 2000. doi: 10.1006/jmva.1999.1860. [Online]. Available: https://www.sciencedirect.com/science/article/pii/S0047259X99918602

##### **Answers**

1. YES. On one hand, the formula is ugly. On the other, it is the only specific multivariate polynomial in GRVs, and it is closely connected to the Laguerre expansion.
2. YES, so that we present the relation of single and multivariate forms.
3. YES, mention the statistical application.
4. Comments:
    - Can we generalize to more than one affine polynomial?
    - If we used the notation of the expansion in chi-square densities, will the sub-formualae be easier to grasp?

####  55. B. G. Lindsay, R. S. Pilla, and P. Basak, “Moment-based approximations of distributions using mixtures: Theory and applications,” Annals of the Institute of Statistical Mathematics, vol. 52, pp. 215–230, 2000

##### **Answers**

1. NO, the formula looks more similar to a tutorial than to a formula.
2. NO.
3. NO detailed application.
4. Comments: NONE

#### 56.  D. Kuonen, “Saddlepoint Approximations for Distributions of Quadratic Forms in Normal Variables,” Biometrika, vol. 86, no. 4, pp. 929–935, 1999. JSTOR: 2673596. [Online]. Available: https://www.jstor.org/stable/2673596

##### **Answers**

1. YES. One of the most important formulae of the paper.
2. NO, unless we think that we can embark on a long journery in the world of saddlepoint approximations and Barndorff-Nielsen's *easy* papers.
3. NO, we'll elaborate in the genetics section.
4. Comments:
    - Compare with Al-Naffouri's formula. We deduced that they are not the same, so demonstrate that.

#### 57. S. B. Provost and E. M. Rudiuk, “The exact distribution of indefinite quadratic forms in noncentral normal vectors,” Annals of the Institute of Statistical Mathematics, vol. 48, no. 2, pp. 381–394, Jun. 1996. doi: 10.1007/BF00054797. [Online]. Available: http://link.springer.com/10.1007/BF00054797

##### **Answers**

1. NO. The formulae are monstrous.
2. YES, to demonstrate that the convolution of two PD forms is usually used to study the indefinite forms.
3. NO detaield approximation.
4. Comments:
    - Restudy the Whittaker function, it seems that cdefinition given in the indefinite section in Matahi does not work for ratios of gammas of negative integers.
    - Even the symbolic functions in Julia were not able to beat the MC simulation for a large number of variables.

#### 58. D. Raphaeli, “Distribution of noncentral indefinite quadratic forms in complex normal variables,” IEEE Transactions on Information Theory, vol. 42, no. 3, pp. 1002–1007, May 1996. doi: 10.1109/18.490565

##### **Answers** 

1. YES, so that we demonstrate that infinite series were used for Hermitian forms.
2. NO. The proof comprises inverse trnasform and residue theory.
3. NO, we'll elaborate on MIMO later.
4.  Comments:
    - Compare computation time with Ramirez-Espinoza.

#### 59. RobertsExistenceMomentsRatios1995

Just for existence, subsumed by Bao and Kann.

#### 60. Royen, “ON SOME CENTRAL AND NON-CENTRAL MULTIVARIATE CHI-SQUARE DISTRIBUTIONS,” Statistica Sinica, vol. 5, no. 1, pp. 373–397, 1995. JSTOR: 24305576. [Online]. Available: https://www.jstor.org/stable/24305576 (visited on 12/18/2021) [MultiV: 2-Factorial]

##### **Answers**

1. Yes, we cannot talk about $m$-factorial and report only one-factorial. The general $m$-factorial case incorporoates MC.
2. The thing here is that we want to readapt the general $m$-factorial case, or report it as an imtermediate step.
3. No detailed application.
4. Comments: NONE

#### 61. T. Royen, “ON SOME CENTRAL AND NON-CENTRAL MULTIVARIATE CHI-SQUARE DISTRIBUTIONS,” Statistica Sinica, vol. 5, no. 1, pp. 373–397, 1995. JSTOR: 24305576. [Online]. Available: https://www.jstor.org/stable/24305576 (visited on 12/18/2021) [MultiV: 1-Factorial]

##### **Answers**

1. Yes, the formula seems computable.
2. Same: The thing here is that we want to readapt the general $m$-factorial case, or report it as an imtermediate step.
3. No detailed application.
4. Comments: NONE

#### 62. Royen, “ON SOME CENTRAL AND NON-CENTRAL MULTIVARIATE CHI-SQUARE DISTRIBUTIONS,” Statistica Sinica, vol. 5, no. 1, pp. 373–397, 1995. JSTOR: 24305576. [Online]. Available: https://www.jstor.org/stable/24305576 (visited on 12/18/2021) [MultiV: 1-Factorial Rank 1 Non-centrality]

##### **Answers**

1. Yes, the formula seems computable.
2. Same: The thing here is that we want to readapt the general $m$-factorial case, or report it as an imtermediate step.
3. No detailed application.
4. Comments: 
    - This incorporates the case of $\mu_j=\mu$, which may be assumed in correlated Rician.

#### 63.  T. Royen, “On some multivariate gamma-distributions connected with spanning trees,” Annals of the Institute of Statistical Mathematics, vol. 46, no. 2, pp. 361–371, Jun. 1994. doi: 10.1007/BF01720592. [Online]. Available: http://link.springer.com/10.1007/BF01720592 (visited on 06/21/2022)

##### **Answers**

1. NO, the formulae are monstrous; just report the form and mention it subsumes tridiagonal.
2. NO
3. No detailed application.
4. Comments: 
    - Check if the trivaraite case simplifies the formula. Especially for trivariate precision matrix, this may be useful.

#### 64. T. Royen, “Expansions for the multivariate chi-square distribution,” Journal of Multivariate Analysis, vol. 38, no. 2, pp. 213–232, Aug. 1, 1991. doi: 10.1016/0047-259X(91)90041-Y. [Online]. Available: https://www.sciencedirect.com/science/article/pii/0047259X9190041Y (visited on 04/08/2021)

##### **Answers**

1. YES, it is the most general computable Royen's formula. It was replicated for the complex counterpart in Morsles-Jimenez 2011.
2. YES, one proof *almost* covers two methods.
3. NO detailed application.
4. Comments:
    - Use Morales-Jimenez's code to implement.

#### 65. T. Royen, “Multivariate gamma distributions with one-factorial accompanying correlation matrices and applications to the distribution of the multivariate range,” Metrika, vol. 38, no. 1, pp. 299–315, Dec. 1, 1991. doi: 10.1007/BF02613625. [Online]. Available: https://doi.org/10.1007/BF02613625

##### **Answers**

1. YES, it is the simplest amongst Royen's formualae.
2. YES, preferably unified with non-central one factorial.
3. YES, it is among the few times Royen details applications.
4. Comments: NONE

#### 66. A. T. A. Wood, “An f approximation to the distribution of a linear combination of chi-squared variables.,” Communications in Statistics - Simulation and Computation, vol. 18, no. 4, pp. 1439–1456, 1989. d

#### 67. M. Buckley and G. Eagleson, “An approximation to the distribution of quadratic forms in normal random variables,”Australian Journal of Statistics, vol. 30A, no. 1, pp. 150–159, 1988. doi: https://doi.org/10.1111/j.1467-842X.1988.tb00471.x. eprint: https://onlinelibrary.wiley.com/doi/pdf/10.1111/j.1467-842X.1988.tb00471.x. [Online]. Available: https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1467-842X.1988.tb00471.x

#### 68. P. Hall, “Chi squared approximations to the distribution of a sum of independent random variables,” The Annals of Probability, vol. 11, no. 4, pp. 1028–1036, 1983. [Online]. Available: http://www.jstor.org/stable/2243514 (visited on 10/24/2023)

#### 69. F. E. Satterthwaite, “An approximate distribution of estimates of variance components,” Biometrics Bulletin, vol. 2, no. 6, pp. 110–114, 1946. [Online]. Available: http://www.jstor.org/stable/3002019 (visited on 10/24/2023)



##### **Answers** 

1. YES. The formulae are simple.
2. YES, prefarably in a unified way. For each mehtod, answer the following questions:
    - How many moments are used?
    - How many are equated and how many differences are minimised?
    - How are the used distributions related to quadratic forms and to each other?
3. NO, elaborate on geentics and relaibility later.
4. Comments: NONE









# IDEAS:
- Use M-Factorial to analyze a Fluidic Antenna system with Nakagami-m model. 

Say we are using a Fluidic Antenna with Millimeter or Terahertz frequencies. The antennas will definitely have a LOS component directed at them. Thus we migth need teh Rician or generalized Rician case.

 