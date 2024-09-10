ANOVA_stimStrength-att
================
Karen Tian
2024-09-09

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
