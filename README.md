---
title: "ReadMe"
output: html_document
---


<!-- README.md is generated from README.Rmd. Please edit that file -->

```{r, include = FALSE}
knitr::opts_chunk$set(
  collapse = TRUE,
  comment = "#>",
  fig.path = "man/figures/README-",
  out.width = "100%"
)
```

# OD2WEIRT 
MCMC Algorithm for The Explanatory Two-way Outlier Detection Model

The goal of OD2WEIRT is to provide a MCMC routine for the Explanatory Two-way Outlier Detection Model.

## Example: Data Generation

This is an example showing how to simulate binary item response data including covariates.

source("simData_cov.R")

Y.sim <- simData_M3(N = 1000, J = 50, Lambda = Lambda0, A = A0, Phi = Phi0, B = B0,
                    s2_theta = 0.5, s2_beta = 0.5, C = C0, D = D0, delta = 0.5)
