# Parallel implementation of time-varying parameter quantile regression on Windows
This is an implementation of time-varying parameter quantile regression (TVP-QR) on Windows which can be run in parallel. The original R codes are published by [Michael Pfarrhofer](https://github.com/mpfarrho/tvp-qr) in Github as the implementation TVP-QR in his work [Modeling tail risks of inflation using unobserved component quantile regressions](https://www.sciencedirect.com/science/article/pii/S016518892200197X).

However, the R codes he provided can not be run in parallel in Windows environment. This project make it possible for it to be run in parallel on Windows by constructing two Rcpparmadillo packages: "FFBS" and "JPR" using the original Cpp codes "ffbs.cpp" and "jpr.cpp" and importing them into the parallel function.

If you have any problem, please contact me.