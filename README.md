# Parallel implementation of time-varying parameter quantile regression on Windows
This is an implementation of time-varying parameter quantile regression (TVP-QR) on Windows which can be run in parallel. The original R codes are published by [Michael Pfarrhofer](https://github.com/mpfarrho/tvp-qr) in Github as the implementation TVP-QR in his work [Modeling tail risks of inflation using unobserved component quantile regressions](https://www.sciencedirect.com/science/article/pii/S016518892200197X).

However, the R codes he provided can not be run in parallel in Windows environment. This project make it possible for it to be run in parallel on Windows by constructing two Rcpparmadillo packages: "FFBS" and "JPR" using the original Cpp codes "ffbs.cpp" and "jpr.cpp" and importing them into the parallel function.

Please follow the following steps to run the algorithm.
1.Install "FFBS_1.0.tar.gz" and "JPR_1.0.tar.gz" locally in your R.
2.Open every single .R file
3.Install the prerequisites R packages (Rstudio is recommended for helping you install them by its notification appeared in every .R file you have opened)
4.Run the algorithm with default dataset or your dataset after select the number of cores and quantiles by setting the variables $cpu$ and $grid.p$, respectively.

If you have any problem, please contact me.