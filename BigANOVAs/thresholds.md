TWCF Thresholds
================
2024-02-29

## Threshold ANOVA: all experiments

``` r
m_anova = ezANOVA(
  data = data,
  dv = .(threshold),
  wid = .(subject),
  between = .(site,expt),
  detailed = TRUE,
  )
```

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

    ## Coefficient covariances computed by hccm()

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>

| Effect    | DFn | DFd |       SSn |      SSd |         F |         p | p\<.05 |       ges |
|:----------|----:|----:|----------:|---------:|----------:|----------:|:-------|----------:|
| site      |   1 | 111 | 0.0377513 | 1.980067 |  2.116291 | 0.1485612 |        | 0.0187090 |
| expt      |   3 | 111 | 1.1929671 | 1.980067 | 22.292063 | 0.0000000 | \*     | 0.3759704 |
| site:expt |   3 | 111 | 0.1198578 | 1.980067 |  2.239691 | 0.0876073 |        | 0.0570772 |

</td>
<td>

| DFn | DFd |       SSn |      SSd |        F |         p | p\<.05 |
|----:|----:|----------:|---------:|---------:|----------:|:-------|
|   7 | 111 | 0.4040958 | 1.732702 | 3.698158 | 0.0012454 | \*     |

</td>
</tr>
</tbody>
</table>

## Threshold ANOVA: Experiment 1 (cue_tex_det)

``` r
d <- data %>% filter(expt==1)
m_anova = ezANOVA(
  data = d,
  dv = .(threshold),
  wid = .(subject),
  between = .(site),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subject" for ANOVA.

    ## Coefficient covariances computed by hccm()

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>

| Effect | DFn | DFd |     SSn |      SSd |        F |        p | p\<.05 |       ges |
|:-------|----:|----:|--------:|---------:|---------:|---------:|:-------|----------:|
| site   |   1 |  28 | 0.15751 | 1.952904 | 2.258319 | 0.144094 |        | 0.0746346 |

</td>
<td>

| DFn | DFd |       SSn |      SSd |        F |         p | p\<.05 |
|----:|----:|----------:|---------:|---------:|----------:|:-------|
|   1 |  28 | 0.1688531 | 1.720334 | 2.748237 | 0.1085254 |        |

</td>
</tr>
</tbody>
</table>

## Threshold ANOVA: Experiment 3 (cue_gab_det)

``` r
d <- data %>% filter(expt==3)
m_anova = ezANOVA(
  data = d,
  dv = .(threshold),
  wid = .(subject),
  between = .(site),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subject" for ANOVA.

    ## Coefficient covariances computed by hccm()

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>

| Effect | DFn | DFd |      SSn |       SSd |         F |         p | p\<.05 |       ges |
|:-------|----:|----:|---------:|----------:|----------:|----------:|:-------|----------:|
| site   |   1 |  28 | 9.92e-05 | 0.0271636 | 0.1022517 | 0.7515178 |        | 0.0036386 |

</td>
<td>

| DFn | DFd |      SSn |       SSd |         F |         p | p\<.05 |
|----:|----:|---------:|----------:|----------:|----------:|:-------|
|   1 |  28 | 1.63e-05 | 0.0123673 | 0.0369457 | 0.8489628 |        |

</td>
</tr>
</tbody>
</table>
