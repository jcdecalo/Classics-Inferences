# Classics-Inferences
DaiGenix's methodology is simple: "Plow the land first, and you'll be sure of a good harvest".Our strategy, therefore, starts with the foundation: classic yet modern exploratory analysis ("Plow the land"), inferential analytics ("Sowing with precision"), and finally, predictive modelling ("Harvesting the future").

# Areas of specialty
-Scan-scath analysis, validation of data and presentation of results with dashboards. Full data research includes:
--descriptive analysis: Run tests and descriptive statistics (variability, centrality, asymmetry or bias. fashion and kurtosis, in tabulated summary and graphic). Descriptive pre-recognition of the predominant characteristic statograph (mean and standard or medium deviation and interquartile range)
--the structural analysis of the data: such as the graphical pre-recognition (I charts) of non-random patterns (tendency, cyclicity, clustering or clusters, jumps, population mixing. oscillation and extremes), analytical recognition of atypical values (outlier tests), analytical recognition of non-random patterns and autocorrelation analysis of data (for time series or data in chronological order). Initial recognition of assignable or non-assignable causes of data behavior. Final opinion of randomness and independence of data.
-Inferential analysis: Contrasting of hypotriss (normality, homocedasticity, selection of parametric vs. non-parametric tests to contrast hypothesis of homogeneity for any sample size of quantitative data. Frequency analysis for qualitative or categorical data (ordinal or not) to contrast homogeneity and independence. 
-Pre-edictive analysis of time series: ARIMA modeling, waste diagnosis and validation.

# Areas of application
-Data validation, detection of biases or adultery.
-Consistency studies.
-Comparability studies.
Predicting trends and behaviors. Prediction of short and medium-term values.

==============================================================================

# Tool set
# 1. Exploratory Analysis and Data Quality
-Descriptive analysis (analytical and graphic), I chart, Run charts.
--Treating null and duplicate values.
--Detection of outliers by multiple methods:
---Dean and Dixon's test (quantitative method) and BoxPlot (Box and Wiskers or Box and Whisks) (graphic method): For small sample of data (n≤100)(*) with continuous, symmetrical and unimodal distribution,
---Test of Grubbs (quantitative method) or the BoxPlot (graphical method): For sample of data of any size and with continuous, symmetrical and unimodal distribution,
---Camp Meidell extension of the Chebyshev inequality theorem (quantitative method). or the BoxPlot (Box and Wiskers) graphical method: For data sample of any size and with parametric or non-parametric continuous distribution.
---Other methods: IQR, Z-score, Mahalanobis and Isolation Forest.
--Comparison of results between methods to decide the treatment (elimination, windsorption or conservation).
--Analysis of autocorrelation of chronological data:
---Global autocorrelation with Ljung Q statistican and K-order Box.

# 2. Hypothese Contrast
-Tests of normality:
--Shapiro-Wilk Test or Ryan-Joiner Test: For small sample size n≤50 with little or great variability (invariable test power with or without atypical points)
-- Anderson Darling Test: For large sample size n50 with little variability (invariable test power with or without atypical points)
--Test by Kolmagorov-Smirnov-Lilliefors: For large sample size n50 with great variability (potency of the test sensitive to atypical points)
Homogeneity contrast between the sample dispersions
--Parametric statigrapher (mean and standard deviation)
---Populations with Normal distribution
---Analysis of homocedasticity of variances (for populations of any size that meet conditions of independence and normality):
-----Bartlett Test: For samples whose number of levels per factor is less than 12
-----Cochran Test: For samples of equal size and whose number of levels per factor is greater than 12
--Non-Parametric Statigrapher (median and interquartityl range)
---Populations with Non-Parametric distribution
Homogeneity analysis between sample dispersions (for populations of any size that meet randomness and independence conditions):
-----Siegel-Tukey Test: For samples with asymmetry in the same direction
---Other methods: Levene and Breusch-Pagan.
-Contrastion of homogeneity between the central sample measures
--Parametric statigrapher (mean and standard deviation)
---Populations with Normal distribution
---Analysis of homogeneity of the means:
-----Test ANOVA: For populations of any size that meet conditions of independence, normalcy and homocedasticity.
Welch Test: For small-sized data samples, they meet the conditions of independence and normality but without homocedasticity
---Test of multiple paired comparisons (if the null hypothesis of homogeneity of the stockings fails):
Duncan's test (if the number of observations per level is the same)
Multiple comparison test of Bonferroni (if the number of contrasts to be performed is well known a priori and at least equal to the number of treatments or factor levels)
-----Scheffé test (if the number of contrasts is much higher than the number of treatments and if a priori this number is unknown)
--Non-Parametric Statigrapher (median and interquartityl range)
---Populations with Non-Parametric distribution
---Analysis of homogeneity of the medians:
Kruskal-Wallis Test: For data samples of any size that meet the conditions of independence, asymmetry in the same direction, similar dispersions
If the number n of data per sample is equal to or less than 5 (n≤5) it is recommended to use the statister H,
-----If the number n of data per sample is greater than 5 (n>5) it is recommended to use the chi-square stat.
Cochran Q Test: For random data samples of any size that do not meet the independence conditions.
---Test of multiple paired comparisons (if the null hypothesis of homogeneity of the medians fails):
-----Kruskal-Wallis multi-compared test.
Homogeneity contrast between sample dispersions for two simple data samples
--Parametric statigrapher (mean and standard deviation)
---Populations with Normal distribution
---Proof of Homocedasticity (F-test of Fisher-Snedecor for the hypothesis test of the quotient of two population variances): For populations of any size that meet conditions of independence and normality.
--Non-Parametric Statigrapher (median and interquartityl range)
---Populations with Non-Parametric distribution
---Proof of homogeneity for dispersions of two samples (Siegel-Tukey Test): For populations of any size that meet independence conditions.
Homogeneity contrast between the sample central measurements for two simple data samples
--Parametric statigrapher (mean and standard deviation)
---Populations with Normal distribution
Student t-test for the difference of two population means with unknown population variances that can be assumed the same or different: For populations of any size that meet conditions of independence, normality and homocedasticity.
---Test of comparisons paired by the student t for the means of the differences: For populations of any size that meet normal conditions but the data are dependent and paired.
--Non-Parametric Statigrapher (median and interquartityl range)
---Populations with Non-Parametric distribution
---- Test of comparisons between the medians of the Wilcoxon-Mann-Whitney U: For simple comparisons between two independent data samples.
Wilcoxon T test for two paired samples: For simple comparisons between two non-parametric dependent and paired data samples.
-Feed analysis
--Bründen's test of homogeneity against a control group: For cases where the sources of variability of a small sample of data are unknown and qualitative dichotomous comparisons of the observed frequencies of different levels against a control group are required
---Contingency tables 2xc or 2x2 (chi-square statistic): If the sample is considered large, that is, it is such that n>=40 and all expected frequencies are >=1, or 20=<n<40, and all expected frequencies are >=5.
-- Fisher's exact Homogeneity Test: If the sample is considered small, i.e. it is such that n<20.

# 3. Modeling and Forecasting (ARIMA)
- Seasonal analysis (ADF / KPSS) and differentiation.
- Identification of orders (p,d,q) via ACF/PACF and AIC/BIC criteria.
- **Diagnosis of waste**: Ljung-Box and normal waste.
- Out-of-sample validation with metrics (RMSE, MAE, MAPE).
