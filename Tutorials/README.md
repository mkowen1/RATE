# Demonstrations and Tutorials on Running RATE
In the file entitled "Centrality_Tutorial.R", we walk through the implementation distributional centrality measures. Specifically, we describe in detail: (1) how to compute a covariance matrix using the Gaussian kernel function; (2) how to fit a standard Bayesian Gaussian process (GP) regression model; (3) retrieving effect size analogue estimates for the original predictor variables; and (4) prioritizing variables via their first, second, third, and fourth order centrality. This script is based on a simple (and small) genetics example where we simulate genotype data for n = 500 individuals with p = 25 measured genetic variants. We randomly assume the last three predictors p* = {23, 24, 25} are causal and have true association with #the generated (continuous) phenotype y. We then assume that the p* predictor variables explain a fixed Vx = 75% (phenotypic variance explained; PVE) of the total variance in the response V(y). This parameter Vx can alternatively be described as a factor controlling the signal-to-noise ratio. The parameter rho represents the proportion of Vx that is contributed by additive effects versus interaction effects. Namely, the additive effects make up rho%, while the pairwise interactions make up the remaining (1 − rho)%.

In the power analyses files, demonstrate the power of distributional centrality via RATE measures. Specifically we compare our approach to: (1) L1- regularized lasso regression; (2) L2-regularized ridge regression; (3) the combined regularization utilized by the elastic net; and (4) a commonly used spike and slab prior model, also known as Bayesian variable selection regression, which computes posterior inclusion probabilities (PIPs) for each covariate as a mixture of a point mass at zero and a diffuse normal centered around zero. This script is based on a similar genetics example where we now assess association mapping ability in the presence of (i) different signal-to-noise ratios in Vx, (ii) varying levels of additive and interaction effects in rho, and (iii) completely independent and partially correlated data.