ANOVA_stimStrength-att
================
Karen Tian
2024-09-10

## Performance as a function of stimulus strength (all expts)

Remove contrast 0 for Expt 3 for balanced design

``` r
dS <- data %>% filter(stimStrength!=0) 
m_anova = ezANOVA(
  data = dS,
  dv = .(correctDis),
  wid = .(subjectID),
  within = .(attention,stimStrength),
  between = .(site),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

``` r
knitr::kable(m_anova, digits=3, caption="Performance by stimulus strength (expts 1-4) ANOVA")
```

<table class="kable_wrapper">
<caption>
Performance by stimulus strength (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn |  DFd |      SSn |   SSd |         F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|-----:|---------:|------:|----------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  117 | 1458.355 | 8.787 | 19418.253 | 0.000 | \*     | 0.986 |
| 2   | site                        |   1 |  117 |    0.407 | 8.787 |     5.416 | 0.022 | \*     | 0.019 |
| 3   | attention                   |   2 |  234 |   18.467 | 3.243 |   666.256 | 0.000 | \*     | 0.463 |
| 5   | stimStrength                |   6 |  702 |   26.764 | 5.551 |   564.069 | 0.000 | \*     | 0.556 |
| 4   | site:attention              |   2 |  234 |    0.059 | 3.243 |     2.118 | 0.123 |        | 0.003 |
| 6   | site:stimStrength           |   6 |  702 |    0.007 | 5.551 |     0.150 | 0.989 |        | 0.000 |
| 7   | attention:stimStrength      |  12 | 1404 |    1.587 | 3.818 |    48.644 | 0.000 | \*     | 0.069 |
| 8   | site:attention:stimStrength |  12 | 1404 |    0.062 | 3.818 |     1.906 | 0.030 | \*     | 0.003 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.530 |   0 | \*     |
| 4   | site:attention              | 0.530 |   0 | \*     |
| 5   | stimStrength                | 0.035 |   0 | \*     |
| 6   | site:stimStrength           | 0.035 |   0 | \*     |
| 7   | attention:stimStrength      | 0.069 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.069 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.680 |   0.000 | \*           | 0.685 |   0.000 | \*           |
| 4   | site:attention              | 0.680 |   0.140 |              | 0.685 |   0.140 |              |
| 5   | stimStrength                | 0.427 |   0.000 | \*           | 0.437 |   0.000 | \*           |
| 6   | site:stimStrength           | 0.427 |   0.906 |              | 0.437 |   0.910 |              |
| 7   | attention:stimStrength      | 0.707 |   0.000 | \*           | 0.767 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.707 |   0.052 |              | 0.767 |   0.046 | \*           |

</td>
</tr>
</tbody>
</table>

``` r
## Performance by stimulus strength
d <- dS %>% group_by(stimStrength) %>%
  summarise(mean=mean(correctDis), sd=sd(correctDis), n=n_distinct(subjectID)) %>% mutate(se = sd / sqrt(n),
         ci.lower = mean - qt(1 - (0.05 / 2), n - 1) * se,
         ci.upper = mean + qt(1 - (0.05 / 2), n - 1) * se)
knitr::kable(d, digits=3, caption="Performance by stimulus strength (expts 1-4) summary stats")
```

| stimStrength |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-------------|------:|------:|----:|------:|---------:|---------:|
| 1            | 0.576 | 0.103 | 119 | 0.009 |    0.557 |    0.595 |
| 2            | 0.668 | 0.129 | 119 | 0.012 |    0.644 |    0.691 |
| 3            | 0.742 | 0.140 | 119 | 0.013 |    0.716 |    0.767 |
| 4            | 0.783 | 0.147 | 119 | 0.013 |    0.756 |    0.809 |
| 5            | 0.830 | 0.139 | 119 | 0.013 |    0.805 |    0.855 |
| 6            | 0.858 | 0.129 | 119 | 0.012 |    0.834 |    0.881 |
| 7            | 0.892 | 0.116 | 119 | 0.011 |    0.871 |    0.913 |

Performance by stimulus strength (expts 1-4) summary stats

## Performance as a function of stimulus strength (expt 1)

``` r
dS <- data %>% filter(expt==1)
m_anova = ezANOVA(
  data = dS,
  dv = .(correctDis),
  wid = .(subjectID),
  within = .(attention,stimStrength),
  between = .(site),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subjectID" for ANOVA.

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |         SSn |       SSd |            F |         p | p\<.05 |       ges |
|:----|:----------------------------|----:|----:|------------:|----------:|-------------:|----------:|:-------|----------:|
| 1   | (Intercept)                 |   1 |  28 | 374.3478071 | 1.0568290 | 9918.1024530 | 0.0000000 | \*     | 0.9893167 |
| 2   | site                        |   1 |  28 |   0.0226398 | 1.0568290 |    0.5998259 | 0.4451356 |        | 0.0055693 |
| 3   | attention                   |   2 |  56 |   2.3274901 | 0.5808956 |  112.1883592 | 0.0000000 | \*     | 0.3653866 |
| 5   | stimStrength                |   6 | 168 |  11.6294018 | 1.4801778 |  219.9892743 | 0.0000000 | \*     | 0.7420567 |
| 4   | site:attention              |   2 |  56 |   0.0151282 | 0.5808956 |    0.7292026 | 0.4868160 |        | 0.0037284 |
| 6   | site:stimStrength           |   6 | 168 |   0.0421947 | 1.4801778 |    0.7981818 | 0.5725900 |        | 0.0103301 |
| 7   | attention:stimStrength      |  12 | 336 |   0.4260557 | 0.9245460 |   12.9031537 | 0.0000000 | \*     | 0.0953464 |
| 8   | site:attention:stimStrength |  12 | 336 |   0.0487557 | 0.9245460 |    1.4765723 | 0.1309787 |        | 0.0119172 |

</td>
<td>

|     | Effect                      |         W |         p | p\<.05 |
|:----|:----------------------------|----------:|----------:|:-------|
| 3   | attention                   | 0.3853454 | 0.0000026 | \*     |
| 4   | site:attention              | 0.3853454 | 0.0000026 | \*     |
| 5   | stimStrength                | 0.0200243 | 0.0000000 | \*     |
| 6   | site:stimStrength           | 0.0200243 | 0.0000000 | \*     |
| 7   | attention:stimStrength      | 0.0043043 | 0.0002547 | \*     |
| 8   | site:attention:stimStrength | 0.0043043 | 0.0002547 | \*     |

</td>
<td>

|     | Effect                      |       GGe |   p\[GG\] | p\[GG\]\<.05 |       HFe |   p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|----------:|----------:|:-------------|----------:|----------:|:-------------|
| 3   | attention                   | 0.6193275 | 0.0000000 | \*           | 0.6337685 | 0.0000000 | \*           |
| 4   | site:attention              | 0.6193275 | 0.4271556 |              | 0.6337685 | 0.4300338 |              |
| 5   | stimStrength                | 0.3799700 | 0.0000000 | \*           | 0.4154636 | 0.0000000 | \*           |
| 6   | site:stimStrength           | 0.3799700 | 0.4691845 |              | 0.4154636 | 0.4786784 |              |
| 7   | attention:stimStrength      | 0.6171142 | 0.0000000 | \*           | 0.8608868 | 0.0000000 | \*           |
| 8   | site:attention:stimStrength | 0.6171142 | 0.1730804 |              | 0.8608868 | 0.1446842 |              |

</td>
</tr>
</tbody>
</table>

``` r
## Performance by stimulus strength
d <- dS %>% group_by(stimStrength) %>%
  summarise(mean=mean(correctDis), sd=sd(correctDis), n=n_distinct(subjectID)) %>% mutate(se = sd / sqrt(n),
         ci.lower = mean - qt(1 - (0.05 / 2), n - 1) * se,
         ci.upper = mean + qt(1 - (0.05 / 2), n - 1) * se)
knitr::kable(d, digits=3, caption="Performance by stimulus strength (expt 1)")
```

| stimStrength |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-------------|------:|------:|----:|------:|---------:|---------:|
| 1            | 0.509 | 0.062 |  30 | 0.011 |    0.486 |    0.532 |
| 2            | 0.651 | 0.127 |  30 | 0.023 |    0.604 |    0.699 |
| 3            | 0.757 | 0.117 |  30 | 0.021 |    0.713 |    0.801 |
| 4            | 0.812 | 0.119 |  30 | 0.022 |    0.767 |    0.857 |
| 5            | 0.858 | 0.112 |  30 | 0.021 |    0.816 |    0.900 |
| 6            | 0.882 | 0.107 |  30 | 0.020 |    0.842 |    0.922 |
| 7            | 0.927 | 0.074 |  30 | 0.014 |    0.899 |    0.955 |

Performance by stimulus strength (expt 1)
