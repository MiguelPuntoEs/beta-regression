# Beta regression

Example for beta regression from `statsmodels` package.

Data exported from `GasolineYield{betareg}` from [betareg package](https://search.r-project.org/CRAN/refmans/betareg/html/GasolineYield.html) as follows:

```r
install.packages('betareg')
data("GasolineYield", package = "betareg")
write.csv(GasolineYield, 'gasoline.csv')
```

Another possibility: `Gasoline{nlme}` from [nlme package](https://stat.ethz.ch/R-manual/R-devel/library/nlme/html/Gasoline.html).

## Theory

Probability density function:

$$f(y; \mu,\phi) = \frac{\Gamma(\phi)}{\Gamma(\mu\phi)\Gamma((1-\mu)\phi)}y^{\mu\phi-1}(1-y)^{(1-\mu)\phi-1}$$
$0<y<1$