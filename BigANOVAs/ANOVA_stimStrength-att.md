ANOVA_stimStrength-att
================
Karen Tian
2024-11-03

Performance  
• [all
expts](#Performance-as-a-function-of-stimulus-strength-(all-expts))  
Overall visibility  
Task-relevant feature visibility

## Reaction time as a function of stimulus strength (all expts)

Remove contrast 0 for Expt 3 for balanced design

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Reaction time (s) by stimulus strength (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn |  DFd |      SSn |     SSd |        F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|-----:|---------:|--------:|---------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  117 | 1585.910 | 141.799 | 1308.551 | 0.000 | \*     | 0.900 |
| 2   | site                        |   1 |  117 |    5.581 | 141.799 |    4.605 | 0.034 | \*     | 0.031 |
| 3   | stimStrength                |   6 |  702 |    1.837 |  14.759 |   14.560 | 0.000 | \*     | 0.010 |
| 5   | attention                   |   2 |  234 |   77.877 |  14.889 |  611.969 | 0.000 | \*     | 0.305 |
| 4   | site:stimStrength           |   6 |  702 |    0.658 |  14.759 |    5.218 | 0.000 | \*     | 0.004 |
| 6   | site:attention              |   2 |  234 |    0.665 |  14.889 |    5.222 | 0.006 | \*     | 0.004 |
| 7   | stimStrength:attention      |  12 | 1404 |    1.508 |   5.657 |   31.195 | 0.000 | \*     | 0.008 |
| 8   | site:stimStrength:attention |  12 | 1404 |    0.078 |   5.657 |    1.608 | 0.083 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | stimStrength                | 0.011 |   0 | \*     |
| 4   | site:stimStrength           | 0.011 |   0 | \*     |
| 5   | attention                   | 0.377 |   0 | \*     |
| 6   | site:attention              | 0.377 |   0 | \*     |
| 7   | stimStrength:attention      | 0.049 |   0 | \*     |
| 8   | site:stimStrength:attention | 0.049 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | stimStrength                | 0.383 |   0.000 | \*           | 0.391 |   0.000 | \*           |
| 4   | site:stimStrength           | 0.383 |   0.004 | \*           | 0.391 |   0.004 | \*           |
| 5   | attention                   | 0.616 |   0.000 | \*           | 0.620 |   0.000 | \*           |
| 6   | site:attention              | 0.616 |   0.017 | \*           | 0.620 |   0.017 | \*           |
| 7   | stimStrength:attention      | 0.646 |   0.000 | \*           | 0.696 |   0.000 | \*           |
| 8   | site:stimStrength:attention | 0.646 |   0.121 |              | 0.696 |   0.115 |              |

</td>
</tr>
</tbody>
</table>

| stimStrength |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-------------|------:|------:|----:|------:|---------:|---------:|
| 1            | 0.756 | 0.103 | 119 | 0.009 |    0.737 |    0.774 |
| 2            | 0.807 | 0.129 | 119 | 0.012 |    0.784 |    0.830 |
| 3            | 0.814 | 0.140 | 119 | 0.013 |    0.789 |    0.840 |
| 4            | 0.823 | 0.147 | 119 | 0.013 |    0.797 |    0.850 |
| 5            | 0.823 | 0.139 | 119 | 0.013 |    0.798 |    0.848 |
| 6            | 0.797 | 0.129 | 119 | 0.012 |    0.773 |    0.820 |
| 7            | 0.756 | 0.116 | 119 | 0.011 |    0.735 |    0.777 |

RT by stimulus strength (expts 1-4) summary stats

| site |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-----|------:|------:|----:|------:|---------:|---------:|
| 0    | 0.749 | 0.167 |  59 | 0.022 |    0.706 |    0.792 |
| 1    | 0.843 | 0.164 |  60 | 0.021 |    0.802 |    0.885 |

RT by stimulus strength by site (expts 1-4)

| attention |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:----------|------:|------:|----:|------:|---------:|---------:|
| -1        | 0.968 | 0.130 | 119 | 0.012 |    0.944 |    0.991 |
| 0         | 0.868 | 0.151 | 119 | 0.014 |    0.841 |    0.895 |
| 1         | 0.554 | 0.144 | 119 | 0.013 |    0.528 |    0.580 |

RT by stimulus strength by attention (expts 1-4)

## Performance as a function of stimulus strength (all expts)

Remove contrast 0 for Expt 3 for balanced design

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

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
| 3   | stimStrength                |   6 |  702 |   26.764 | 5.551 |   564.069 | 0.000 | \*     | 0.556 |
| 5   | attention                   |   2 |  234 |   18.467 | 3.243 |   666.256 | 0.000 | \*     | 0.463 |
| 4   | site:stimStrength           |   6 |  702 |    0.007 | 5.551 |     0.150 | 0.989 |        | 0.000 |
| 6   | site:attention              |   2 |  234 |    0.059 | 3.243 |     2.118 | 0.123 |        | 0.003 |
| 7   | stimStrength:attention      |  12 | 1404 |    1.587 | 3.818 |    48.644 | 0.000 | \*     | 0.069 |
| 8   | site:stimStrength:attention |  12 | 1404 |    0.062 | 3.818 |     1.906 | 0.030 | \*     | 0.003 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | stimStrength                | 0.035 |   0 | \*     |
| 4   | site:stimStrength           | 0.035 |   0 | \*     |
| 5   | attention                   | 0.530 |   0 | \*     |
| 6   | site:attention              | 0.530 |   0 | \*     |
| 7   | stimStrength:attention      | 0.069 |   0 | \*     |
| 8   | site:stimStrength:attention | 0.069 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | stimStrength                | 0.427 |   0.000 | \*           | 0.437 |   0.000 | \*           |
| 4   | site:stimStrength           | 0.427 |   0.906 |              | 0.437 |   0.910 |              |
| 5   | attention                   | 0.680 |   0.000 | \*           | 0.685 |   0.000 | \*           |
| 6   | site:attention              | 0.680 |   0.140 |              | 0.685 |   0.140 |              |
| 7   | stimStrength:attention      | 0.707 |   0.000 | \*           | 0.767 |   0.000 | \*           |
| 8   | site:stimStrength:attention | 0.707 |   0.052 |              | 0.767 |   0.046 | \*           |

</td>
</tr>
</tbody>
</table>

| stimStrength |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-------------|------:|------:|----:|------:|---------:|---------:|
| 1            | 0.576 | 0.103 | 119 | 0.009 |    0.557 |    0.594 |
| 2            | 0.668 | 0.129 | 119 | 0.012 |    0.644 |    0.691 |
| 3            | 0.742 | 0.140 | 119 | 0.013 |    0.717 |    0.767 |
| 4            | 0.783 | 0.147 | 119 | 0.013 |    0.757 |    0.809 |
| 5            | 0.830 | 0.139 | 119 | 0.013 |    0.805 |    0.855 |
| 6            | 0.858 | 0.129 | 119 | 0.012 |    0.835 |    0.881 |
| 7            | 0.892 | 0.116 | 119 | 0.011 |    0.871 |    0.913 |

Performance by stimulus strength (expts 1-4) summary stats

| site |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-----|------:|------:|----:|------:|---------:|---------:|
| 0    | 0.751 | 0.167 |  59 | 0.022 |    0.709 |    0.794 |
| 1    | 0.777 | 0.164 |  60 | 0.021 |    0.735 |    0.818 |

Performance by stimulus strength by site (expts 1-4)

| attention |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:----------|------:|------:|----:|------:|---------:|---------:|
| -1        | 0.658 | 0.130 | 119 | 0.012 |    0.635 |    0.681 |
| 0         | 0.765 | 0.151 | 119 | 0.014 |    0.738 |    0.792 |
| 1         | 0.869 | 0.144 | 119 | 0.013 |    0.843 |    0.895 |

Performance by stimulus strength by attention (expts 1-4)

## Performance as a function of stimulus strength (all expts) - alternative approach to ezANOVA

Remove contrast 0 for Expt 3 for balanced design

    ## Warning in knit_print.huxtable(ht): Unrecognized output format "gfm+tex". Using `to_screen` to print huxtables.
    ## Set options("huxtable.knitr_output_format") manually to "latex", "html", "rtf", "docx", "pptx", "md" or "screen".

        ┌──────────────────────────────────────────────────────────────┐
        │ Effect      DFn   DFd        F          p   p<.05        ges │
        ├──────────────────────────────────────────────────────────────┤
        │ site       1      117     5.42   0.022      *       0.019    │
        │                                                              │
        │ attentio   1.36   159   667      3.67e-67   *       0.463    │
        │ n                                                            │
        │ stimStre   2.56   300   564      9.52e-11   *       0.556    │
        │ ngth                                    5                    │
        │ site:att   1.36   159     2.12   0.14               0.003    │
        │ ention                                                       │
        │ site:sti   2.56   300     0.15   0.906              0.000332 │
        │ mStrengt                                                     │
        │ h                                                            │
        │ attentio   8.48   992    48.7    1.3e-69    *       0.069    │
        │ n:stimSt                                                     │
        │ rength                                                       │
        │ site:att   8.48   992     1.91   0.052              0.003    │
        │ ention:s                                                     │
        │ timStren                                                     │
        │ gth                                                          │
        └──────────────────────────────────────────────────────────────┘

Column names: Effect, DFn, DFd, F, p, p\<.05, ges

    ## 
    ## Error: subjectID
    ##            Df Sum Sq Mean Sq F value Pr(>F)
    ## Residuals 118  9.194 0.07791               
    ## 
    ## Error: Within
    ##                          Df Sum Sq Mean Sq F value Pr(>F)    
    ## attention                 2 18.467   9.234  1710.4 <2e-16 ***
    ## stimStrength              6 26.764   4.461   826.3 <2e-16 ***
    ## attention:stimStrength   12  1.587   0.132    24.5 <2e-16 ***
    ## Residuals              2360 12.740   0.005                   
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

    ## 
    ##  Pairwise comparisons using t tests with pooled SD 
    ## 
    ## data:  dS$correctDis and dS$stimStrength 
    ## 
    ##   1       2       3       4       5       6     
    ## 2 < 2e-16 -       -       -       -       -     
    ## 3 < 2e-16 1.9e-13 -       -       -       -     
    ## 4 < 2e-16 < 2e-16 7.5e-05 -       -       -     
    ## 5 < 2e-16 < 2e-16 < 2e-16 6.0e-06 -       -     
    ## 6 < 2e-16 < 2e-16 < 2e-16 1.1e-13 0.0038  -     
    ## 7 < 2e-16 < 2e-16 < 2e-16 < 2e-16 1.0e-09 0.0010
    ## 
    ## P value adjustment method: holm

## Posthoc performance across successive stim strengths

## Performance across successive stim strengths

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Performance between stimulus strengths 1 vs 2 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |   SSd |        F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|------:|---------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 276.013 | 3.659 | 8826.257 | 0.000 | \*     | 0.977 |
| 2   | site                        |   1 | 117 |   0.132 | 3.659 |    4.210 | 0.042 | \*     | 0.020 |
| 3   | attention                   |   2 | 234 |   2.773 | 1.448 |  224.115 | 0.000 | \*     | 0.297 |
| 5   | stimStrength                |   1 | 117 |   1.505 | 0.854 |  206.226 | 0.000 | \*     | 0.187 |
| 4   | site:attention              |   2 | 234 |   0.013 | 1.448 |    1.040 | 0.355 |        | 0.002 |
| 6   | site:stimStrength           |   1 | 117 |   0.003 | 0.854 |    0.375 | 0.541 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.238 | 0.596 |   46.845 | 0.000 | \*     | 0.035 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.003 | 0.596 |    0.526 | 0.592 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |     p | p\<.05 |
|:----|:----------------------------|------:|------:|:-------|
| 3   | attention                   | 0.778 | 0.000 | \*     |
| 4   | site:attention              | 0.778 | 0.000 | \*     |
| 7   | attention:stimStrength      | 0.975 | 0.233 |        |
| 8   | site:attention:stimStrength | 0.975 | 0.233 |        |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.818 |   0.000 | \*           | 0.828 |   0.000 | \*           |
| 4   | site:attention              | 0.818 |   0.343 |              | 0.828 |   0.344 |              |
| 7   | attention:stimStrength      | 0.976 |   0.000 | \*           | 0.992 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.976 |   0.587 |              | 0.992 |   0.590 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Performance between stimulus strengths 2 vs 3 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |   SSd |         F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|------:|----------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 354.621 | 4.123 | 10063.408 | 0.000 | \*     | 0.981 |
| 2   | site                        |   1 | 117 |   0.104 | 4.123 |     2.948 | 0.089 |        | 0.015 |
| 3   | attention                   |   2 | 234 |   5.880 | 1.616 |   425.791 | 0.000 | \*     | 0.462 |
| 5   | stimStrength                |   1 | 117 |   0.982 | 0.535 |   214.697 | 0.000 | \*     | 0.125 |
| 4   | site:attention              |   2 | 234 |   0.017 | 1.616 |     1.230 | 0.294 |        | 0.002 |
| 6   | site:stimStrength           |   1 | 117 |   0.000 | 0.535 |     0.030 | 0.862 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.096 | 0.575 |    19.548 | 0.000 | \*     | 0.014 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.007 | 0.575 |     1.518 | 0.221 |        | 0.001 |

</td>
<td>

|     | Effect                      |     W |    p | p\<.05 |
|:----|:----------------------------|------:|-----:|:-------|
| 3   | attention                   | 0.822 | 0.00 | \*     |
| 4   | site:attention              | 0.822 | 0.00 | \*     |
| 7   | attention:stimStrength      | 0.935 | 0.02 | \*     |
| 8   | site:attention:stimStrength | 0.935 | 0.02 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.849 |   0.000 | \*           | 0.860 |   0.000 | \*           |
| 4   | site:attention              | 0.849 |   0.290 |              | 0.860 |   0.291 |              |
| 7   | attention:stimStrength      | 0.939 |   0.000 | \*           | 0.954 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.939 |   0.222 |              | 0.954 |   0.222 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Performance between stimulus strengths 3 vs 4 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |   SSd |         F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|------:|----------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 414.947 | 3.879 | 12514.379 | 0.000 | \*     | 0.985 |
| 2   | site                        |   1 | 117 |   0.106 | 3.879 |     3.206 | 0.076 |        | 0.016 |
| 3   | attention                   |   2 | 234 |   8.054 | 1.695 |   555.963 | 0.000 | \*     | 0.556 |
| 5   | stimStrength                |   1 | 117 |   0.300 | 0.352 |    99.815 | 0.000 | \*     | 0.045 |
| 4   | site:attention              |   2 | 234 |   0.026 | 1.695 |     1.821 | 0.164 |        | 0.004 |
| 6   | site:stimStrength           |   1 | 117 |   0.000 | 0.352 |     0.022 | 0.883 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.050 | 0.498 |    11.785 | 0.000 | \*     | 0.008 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.004 | 0.498 |     0.983 | 0.376 |        | 0.001 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.821 |   0 | \*     |
| 4   | site:attention              | 0.821 |   0 | \*     |
| 7   | attention:stimStrength      | 0.801 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.801 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.848 |   0.000 | \*           | 0.859 |   0.000 | \*           |
| 4   | site:attention              | 0.848 |   0.170 |              | 0.859 |   0.170 |              |
| 7   | attention:stimStrength      | 0.834 |   0.000 | \*           | 0.844 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.834 |   0.363 |              | 0.844 |   0.364 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Performance between stimulus strengths 4 vs 5 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |   SSd |         F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|------:|----------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 464.153 | 3.797 | 14300.693 | 0.000 | \*     | 0.987 |
| 2   | site                        |   1 | 117 |   0.087 | 3.797 |     2.677 | 0.104 |        | 0.014 |
| 3   | attention                   |   2 | 234 |   8.134 | 1.582 |   601.695 | 0.000 | \*     | 0.566 |
| 5   | stimStrength                |   1 | 117 |   0.392 | 0.321 |   142.695 | 0.000 | \*     | 0.059 |
| 4   | site:attention              |   2 | 234 |   0.032 | 1.582 |     2.365 | 0.096 |        | 0.005 |
| 6   | site:stimStrength           |   1 | 117 |   0.001 | 0.321 |     0.195 | 0.659 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.026 | 0.525 |     5.690 | 0.004 | \*     | 0.004 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.000 | 0.525 |     0.022 | 0.978 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.712 |   0 | \*     |
| 4   | site:attention              | 0.712 |   0 | \*     |
| 7   | attention:stimStrength      | 0.791 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.791 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.776 |   0.000 | \*           | 0.785 |   0.000 | \*           |
| 4   | site:attention              | 0.776 |   0.110 |              | 0.785 |   0.109 |              |
| 7   | attention:stimStrength      | 0.827 |   0.007 | \*           | 0.837 |   0.006 | \*           |
| 8   | site:attention:stimStrength | 0.827 |   0.961 |              | 0.837 |   0.963 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Performance between stimulus strengths 5 vs 6 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |   SSd |         F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|------:|----------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 508.352 | 3.493 | 17026.998 | 0.000 | \*     | 0.989 |
| 2   | site                        |   1 | 117 |   0.109 | 3.493 |     3.661 | 0.058 |        | 0.019 |
| 3   | attention                   |   2 | 234 |   6.812 | 1.513 |   526.823 | 0.000 | \*     | 0.541 |
| 5   | stimStrength                |   1 | 117 |   0.142 | 0.290 |    57.100 | 0.000 | \*     | 0.024 |
| 4   | site:attention              |   2 | 234 |   0.039 | 1.513 |     3.050 | 0.049 | \*     | 0.007 |
| 6   | site:stimStrength           |   1 | 117 |   0.003 | 0.290 |     1.403 | 0.239 |        | 0.001 |
| 7   | attention:stimStrength      |   2 | 234 |   0.027 | 0.490 |     6.545 | 0.002 | \*     | 0.005 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.003 | 0.490 |     0.743 | 0.477 |        | 0.001 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.607 |   0 | \*     |
| 4   | site:attention              | 0.607 |   0 | \*     |
| 7   | attention:stimStrength      | 0.736 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.736 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.718 |   0.000 | \*           | 0.724 |   0.000 | \*           |
| 4   | site:attention              | 0.718 |   0.067 |              | 0.724 |   0.066 |              |
| 7   | attention:stimStrength      | 0.791 |   0.004 | \*           | 0.800 |   0.004 | \*           |
| 8   | site:attention:stimStrength | 0.791 |   0.448 |              | 0.800 |   0.449 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Performance between stimulus strengths 6 vs 7 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |   SSd |         F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|------:|----------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 546.390 | 3.256 | 19634.550 | 0.000 | \*     | 0.990 |
| 2   | site                        |   1 | 117 |   0.136 | 3.256 |     4.880 | 0.029 | \*     | 0.025 |
| 3   | attention                   |   2 | 234 |   5.166 | 1.365 |   442.860 | 0.000 | \*     | 0.492 |
| 5   | stimStrength                |   1 | 117 |   0.204 | 0.293 |    81.556 | 0.000 | \*     | 0.037 |
| 4   | site:attention              |   2 | 234 |   0.058 | 1.365 |     4.936 | 0.008 | \*     | 0.011 |
| 6   | site:stimStrength           |   1 | 117 |   0.000 | 0.293 |     0.178 | 0.674 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.060 | 0.414 |    17.102 | 0.000 | \*     | 0.011 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.001 | 0.414 |     0.241 | 0.786 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.468 |   0 | \*     |
| 4   | site:attention              | 0.468 |   0 | \*     |
| 7   | attention:stimStrength      | 0.675 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.675 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.653 |   0.000 | \*           | 0.657 |   0.000 | \*           |
| 4   | site:attention              | 0.653 |   0.019 | \*           | 0.657 |   0.019 | \*           |
| 7   | attention:stimStrength      | 0.755 |   0.000 | \*           | 0.763 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.755 |   0.722 |              | 0.763 |   0.725 |              |

</td>
</tr>
</tbody>
</table>

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
options(scipen = 0)
knitr::kable(m_anova$ANOVA, digits=3, escape = FALSE)
```

|     | Effect                      | DFn | DFd |     SSn |   SSd |        F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|------:|---------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  28 | 374.348 | 1.057 | 9918.102 | 0.000 | \*     | 0.989 |
| 2   | site                        |   1 |  28 |   0.023 | 1.057 |    0.600 | 0.445 |        | 0.006 |
| 3   | attention                   |   2 |  56 |   2.327 | 0.581 |  112.188 | 0.000 | \*     | 0.365 |
| 5   | stimStrength                |   6 | 168 |  11.629 | 1.480 |  219.989 | 0.000 | \*     | 0.742 |
| 4   | site:attention              |   2 |  56 |   0.015 | 0.581 |    0.729 | 0.487 |        | 0.004 |
| 6   | site:stimStrength           |   6 | 168 |   0.042 | 1.480 |    0.798 | 0.573 |        | 0.010 |
| 7   | attention:stimStrength      |  12 | 336 |   0.426 | 0.925 |   12.903 | 0.000 | \*     | 0.095 |
| 8   | site:attention:stimStrength |  12 | 336 |   0.049 | 0.925 |    1.477 | 0.131 |        | 0.012 |

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

## Overall visibility as a function of stimulus strength

All expts, remove contrast 0 for Expt 3 for balanced design

``` r
dS <- data %>% filter(stimStrength!=0) 
m_anova = ezANOVA(
  data = dS,
  dv = .(pSeen),
  wid = .(subjectID),
  within = .(attention,stimStrength),
  between = .(site), # ,stimType,taskType
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

``` r
knitr::kable(m_anova, digits=3, caption="Overall visibility by stimulus strength (expts 1-4) ANOVA")
```

<table class="kable_wrapper">
<caption>
Overall visibility by stimulus strength (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn |  DFd |     SSn |     SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|-----:|--------:|--------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  117 | 757.182 | 108.018 | 820.147 | 0.000 | \*     | 0.810 |
| 2   | site                        |   1 |  117 |   0.047 | 108.018 |   0.050 | 0.823 |        | 0.000 |
| 3   | attention                   |   2 |  234 |   3.775 |   9.078 |  48.652 | 0.000 | \*     | 0.021 |
| 5   | stimStrength                |   6 |  702 | 130.266 |  52.533 | 290.123 | 0.000 | \*     | 0.423 |
| 4   | site:attention              |   2 |  234 |   0.131 |   9.078 |   1.689 | 0.187 |        | 0.001 |
| 6   | site:stimStrength           |   6 |  702 |   0.147 |  52.533 |   0.327 | 0.923 |        | 0.001 |
| 7   | attention:stimStrength      |  12 | 1404 |   3.430 |   7.875 |  50.956 | 0.000 | \*     | 0.019 |
| 8   | site:attention:stimStrength |  12 | 1404 |   0.111 |   7.875 |   1.652 | 0.072 |        | 0.001 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.382 |   0 | \*     |
| 4   | site:attention              | 0.382 |   0 | \*     |
| 5   | stimStrength                | 0.001 |   0 | \*     |
| 6   | site:stimStrength           | 0.001 |   0 | \*     |
| 7   | attention:stimStrength      | 0.002 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.002 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.618 |   0.000 | \*           | 0.621 |   0.000 | \*           |
| 4   | site:attention              | 0.618 |   0.196 |              | 0.621 |   0.196 |              |
| 5   | stimStrength                | 0.377 |   0.000 | \*           | 0.385 |   0.000 | \*           |
| 6   | site:stimStrength           | 0.377 |   0.748 |              | 0.385 |   0.752 |              |
| 7   | attention:stimStrength      | 0.391 |   0.000 | \*           | 0.409 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.391 |   0.149 |              | 0.409 |   0.146 |              |

</td>
</tr>
</tbody>
</table>

``` r
## Overall visibility by stimulus strength
d <- dS %>% group_by(stimStrength) %>%
  summarise(mean=mean(pSeen), sd=sd(pSeen), n=n_distinct(subjectID)) %>% mutate(se = sd / sqrt(n),
         ci.lower = mean - 1.96 * se,
         ci.upper = mean + 1.96 * se)
knitr::kable(d, digits=3, caption="Overall visibility by stimulus strength (expts 1-4) summary stats")
```

| stimStrength |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-------------|------:|------:|----:|------:|---------:|---------:|
| 1            | 0.182 | 0.220 | 119 | 0.020 |    0.142 |    0.221 |
| 2            | 0.353 | 0.296 | 119 | 0.027 |    0.300 |    0.406 |
| 3            | 0.460 | 0.341 | 119 | 0.031 |    0.399 |    0.522 |
| 4            | 0.526 | 0.338 | 119 | 0.031 |    0.465 |    0.586 |
| 5            | 0.656 | 0.290 | 119 | 0.027 |    0.603 |    0.708 |
| 6            | 0.789 | 0.214 | 119 | 0.020 |    0.751 |    0.828 |
| 7            | 0.887 | 0.154 | 119 | 0.014 |    0.859 |    0.915 |

Overall visibility by stimulus strength (expts 1-4) summary stats

## Overall visibility across successive stim strengths

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Overall visibility between stimulus strengths 1 vs 2 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |    SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|-------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 51.104 | 35.771 | 167.150 | 0.000 | \*     | 0.516 |
| 2   | site                        |   1 | 117 |  0.021 | 35.771 |   0.070 | 0.792 |        | 0.000 |
| 3   | attention                   |   2 | 234 |  0.104 |  3.855 |   3.148 | 0.045 | \*     | 0.002 |
| 5   | stimStrength                |   1 | 117 |  5.252 |  7.309 |  84.077 | 0.000 | \*     | 0.099 |
| 4   | site:attention              |   2 | 234 |  0.061 |  3.855 |   1.855 | 0.159 |        | 0.001 |
| 6   | site:stimStrength           |   1 | 117 |  0.045 |  7.309 |   0.723 | 0.397 |        | 0.001 |
| 7   | attention:stimStrength      |   2 | 234 |  0.262 |  0.946 |  32.343 | 0.000 | \*     | 0.005 |
| 8   | site:attention:stimStrength |   2 | 234 |  0.023 |  0.946 |   2.905 | 0.057 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.403 |   0 | \*     |
| 4   | site:attention              | 0.403 |   0 | \*     |
| 7   | attention:stimStrength      | 0.777 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.777 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.626 |   0.069 |              | 0.630 |   0.068 |              |
| 4   | site:attention              | 0.626 |   0.173 |              | 0.630 |   0.173 |              |
| 7   | attention:stimStrength      | 0.817 |   0.000 | \*           | 0.827 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.817 |   0.068 |              | 0.827 |   0.067 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Overall visibility between stimulus strengths 2 vs 3 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 118.200 | 63.200 | 218.819 | 0.000 | \*     | 0.622 |
| 2   | site                        |   1 | 117 |   0.115 | 63.200 |   0.213 | 0.646 |        | 0.002 |
| 3   | attention                   |   2 | 234 |   0.234 |  5.919 |   4.626 | 0.011 | \*     | 0.003 |
| 5   | stimStrength                |   1 | 117 |   2.049 |  2.151 | 111.453 | 0.000 | \*     | 0.028 |
| 4   | site:attention              |   2 | 234 |   0.111 |  5.919 |   2.199 | 0.113 |        | 0.002 |
| 6   | site:stimStrength           |   1 | 117 |   0.000 |  2.151 |   0.022 | 0.883 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.069 |  0.667 |  12.093 | 0.000 | \*     | 0.001 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.015 |  0.667 |   2.576 | 0.078 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |     p | p\<.05 |
|:----|:----------------------------|------:|------:|:-------|
| 3   | attention                   | 0.420 | 0.000 | \*     |
| 4   | site:attention              | 0.420 | 0.000 | \*     |
| 7   | attention:stimStrength      | 0.926 | 0.012 | \*     |
| 8   | site:attention:stimStrength | 0.926 | 0.012 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.633 |   0.025 | \*           | 0.637 |   0.025 | \*           |
| 4   | site:attention              | 0.633 |   0.134 |              | 0.637 |   0.134 |              |
| 7   | attention:stimStrength      | 0.931 |   0.000 | \*           | 0.946 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.931 |   0.082 |              | 0.946 |   0.081 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Overall visibility between stimulus strengths 3 vs 4 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 173.596 | 73.318 | 277.022 | 0.000 | \*     | 0.682 |
| 2   | site                        |   1 | 117 |   0.098 | 73.318 |   0.156 | 0.694 |        | 0.001 |
| 3   | attention                   |   2 | 234 |   0.952 |  6.342 |  17.562 | 0.000 | \*     | 0.012 |
| 5   | stimStrength                |   1 | 117 |   0.761 |  0.642 | 138.700 | 0.000 | \*     | 0.009 |
| 4   | site:attention              |   2 | 234 |   0.093 |  6.342 |   1.719 | 0.181 |        | 0.001 |
| 6   | site:stimStrength           |   1 | 117 |   0.000 |  0.642 |   0.007 | 0.933 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.065 |  0.488 |  15.578 | 0.000 | \*     | 0.001 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.001 |  0.488 |   0.250 | 0.779 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |     p | p\<.05 |
|:----|:----------------------------|------:|------:|:-------|
| 3   | attention                   | 0.374 | 0.000 | \*     |
| 4   | site:attention              | 0.374 | 0.000 | \*     |
| 7   | attention:stimStrength      | 0.986 | 0.432 |        |
| 8   | site:attention:stimStrength | 0.986 | 0.432 |        |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.615 |   0.000 | \*           | 0.618 |   0.000 | \*           |
| 4   | site:attention              | 0.615 |   0.192 |              | 0.618 |   0.192 |              |
| 7   | attention:stimStrength      | 0.986 |   0.000 | \*           | 1.003 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.986 |   0.776 |              | 1.003 |   0.779 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Overall visibility between stimulus strengths 4 vs 5 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 249.102 | 59.995 | 485.788 | 0.000 | \*     | 0.785 |
| 2   | site                        |   1 | 117 |   0.045 | 59.995 |   0.088 | 0.767 |        | 0.001 |
| 3   | attention                   |   2 | 234 |   2.461 |  4.315 |  66.739 | 0.000 | \*     | 0.035 |
| 5   | stimStrength                |   1 | 117 |   3.011 |  2.780 | 126.710 | 0.000 | \*     | 0.042 |
| 4   | site:attention              |   2 | 234 |   0.030 |  4.315 |   0.825 | 0.439 |        | 0.000 |
| 6   | site:stimStrength           |   1 | 117 |   0.009 |  2.780 |   0.369 | 0.544 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.116 |  0.957 |  14.190 | 0.000 | \*     | 0.002 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.034 |  0.957 |   4.150 | 0.017 | \*     | 0.000 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.385 |   0 | \*     |
| 4   | site:attention              | 0.385 |   0 | \*     |
| 7   | attention:stimStrength      | 0.723 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.723 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.619 |   0.000 | \*           | 0.623 |   0.000 | \*           |
| 4   | site:attention              | 0.619 |   0.389 |              | 0.623 |   0.389 |              |
| 7   | attention:stimStrength      | 0.783 |   0.000 | \*           | 0.792 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.783 |   0.026 | \*           | 0.792 |   0.025 | \*           |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Overall visibility between stimulus strengths 5 vs 6 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |        F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|---------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 372.636 | 33.963 | 1283.705 | 0.000 | \*     | 0.899 |
| 2   | site                        |   1 | 117 |   0.002 | 33.963 |    0.008 | 0.928 |        | 0.000 |
| 3   | attention                   |   2 | 234 |   4.192 |  3.014 |  162.687 | 0.000 | \*     | 0.091 |
| 5   | stimStrength                |   1 | 117 |   3.188 |  4.374 |   85.276 | 0.000 | \*     | 0.070 |
| 4   | site:attention              |   2 | 234 |   0.013 |  3.014 |    0.514 | 0.599 |        | 0.000 |
| 6   | site:stimStrength           |   1 | 117 |   0.005 |  4.374 |    0.132 | 0.717 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.023 |  0.685 |    3.926 | 0.021 | \*     | 0.001 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.031 |  0.685 |    5.296 | 0.006 | \*     | 0.001 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.452 |   0 | \*     |
| 4   | site:attention              | 0.452 |   0 | \*     |
| 7   | attention:stimStrength      | 0.785 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.785 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.646 |   0.000 | \*           | 0.650 |   0.000 | \*           |
| 4   | site:attention              | 0.646 |   0.520 |              | 0.650 |   0.521 |              |
| 7   | attention:stimStrength      | 0.823 |   0.029 | \*           | 0.833 |   0.028 | \*           |
| 8   | site:attention:stimStrength | 0.823 |   0.009 | \*           | 0.833 |   0.009 | \*           |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Overall visibility between stimulus strengths 6 vs 7 (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |        F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|---------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 | 117 | 501.584 | 14.767 | 3974.051 | 0.000 | \*     | 0.960 |
| 2   | site                        |   1 | 117 |   0.013 | 14.767 |    0.105 | 0.747 |        | 0.001 |
| 3   | attention                   |   2 | 234 |   3.950 |  2.552 |  181.084 | 0.000 | \*     | 0.161 |
| 5   | stimStrength                |   1 | 117 |   1.708 |  2.560 |   78.036 | 0.000 | \*     | 0.076 |
| 4   | site:attention              |   2 | 234 |   0.046 |  2.552 |    2.100 | 0.125 |        | 0.002 |
| 6   | site:stimStrength           |   1 | 117 |   0.009 |  2.560 |    0.397 | 0.530 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 234 |   0.052 |  0.760 |    8.045 | 0.000 | \*     | 0.003 |
| 8   | site:attention:stimStrength |   2 | 234 |   0.002 |  0.760 |    0.253 | 0.777 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.345 |   0 | \*     |
| 4   | site:attention              | 0.345 |   0 | \*     |
| 7   | attention:stimStrength      | 0.692 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.692 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.604 |   0.000 | \*           | 0.607 |   0.000 | \*           |
| 4   | site:attention              | 0.604 |   0.146 |              | 0.607 |   0.145 |              |
| 7   | attention:stimStrength      | 0.764 |   0.001 | \*           | 0.773 |   0.001 | \*           |
| 8   | site:attention:stimStrength | 0.764 |   0.716 |              | 0.773 |   0.719 |              |

</td>
</tr>
</tbody>
</table>

## Task-relevant feature visibility as a function of stimulus strength

Expts 134 (1,2,4), remove contrast 0 for Expt 3 for balanced design

``` r
dS <- data %>% filter(stimStrength!=0) %>% filter(expt!=2)
m_anova = ezANOVA(
  data = dS,
  dv = .(pSeenFeature),
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
knitr::kable(m_anova, digits=3, caption="Task-relevant feature visibility by stimulus strength (3 expts) ANOVA")
```

<table class="kable_wrapper">
<caption>
Task-relevant feature visibility by stimulus strength (3 expts) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn |  DFd |     SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|-----:|--------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |   88 | 470.271 | 59.941 | 690.412 | 0.000 | \*     | 0.834 |
| 2   | site                        |   1 |   88 |   0.006 | 59.941 |   0.009 | 0.923 |        | 0.000 |
| 3   | attention                   |   2 |  176 |  27.272 |  9.383 | 255.762 | 0.000 | \*     | 0.226 |
| 5   | stimStrength                |   6 |  528 |  81.780 | 17.871 | 402.705 | 0.000 | \*     | 0.467 |
| 4   | site:attention              |   2 |  176 |   0.042 |  9.383 |   0.392 | 0.676 |        | 0.000 |
| 6   | site:stimStrength           |   6 |  528 |   0.069 | 17.871 |   0.339 | 0.916 |        | 0.001 |
| 7   | attention:stimStrength      |  12 | 1056 |   4.426 |  6.316 |  61.667 | 0.000 | \*     | 0.045 |
| 8   | site:attention:stimStrength |  12 | 1056 |   0.049 |  6.316 |   0.685 | 0.767 |        | 0.001 |

</td>
<td>

|     | Effect                      |     W |   p | p\<.05 |
|:----|:----------------------------|------:|----:|:-------|
| 3   | attention                   | 0.397 |   0 | \*     |
| 4   | site:attention              | 0.397 |   0 | \*     |
| 5   | stimStrength                | 0.002 |   0 | \*     |
| 6   | site:stimStrength           | 0.002 |   0 | \*     |
| 7   | attention:stimStrength      | 0.005 |   0 | \*     |
| 8   | site:attention:stimStrength | 0.005 |   0 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.624 |   0.000 | \*           | 0.629 |   0.000 | \*           |
| 4   | site:attention              | 0.624 |   0.578 |              | 0.629 |   0.580 |              |
| 5   | stimStrength                | 0.376 |   0.000 | \*           | 0.387 |   0.000 | \*           |
| 6   | site:stimStrength           | 0.376 |   0.739 |              | 0.387 |   0.744 |              |
| 7   | attention:stimStrength      | 0.426 |   0.000 | \*           | 0.455 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.426 |   0.638 |              | 0.455 |   0.648 |              |

</td>
</tr>
</tbody>
</table>

``` r
## Task-relevant feature visibility by stimulus strength
d <- dS %>% group_by(stimStrength) %>%
  summarise(mean=mean(pSeenFeature), sd=sd(pSeenFeature), n=n_distinct(subjectID)) %>% mutate(se = sd / sqrt(n),
         ci.lower = mean - 1.96 * se,
         ci.upper = mean + 1.96 * se)
knitr::kable(d, digits=3, caption="Task-relevant feature visibility by stimulus strength (expts 1-4) summary stats")
```

| stimStrength |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-------------|------:|------:|----:|------:|---------:|---------:|
| 1            | 0.161 | 0.226 |  90 | 0.024 |    0.114 |    0.208 |
| 2            | 0.291 | 0.259 |  90 | 0.027 |    0.238 |    0.345 |
| 3            | 0.427 | 0.271 |  90 | 0.029 |    0.371 |    0.483 |
| 4            | 0.517 | 0.286 |  90 | 0.030 |    0.458 |    0.576 |
| 5            | 0.607 | 0.275 |  90 | 0.029 |    0.550 |    0.664 |
| 6            | 0.679 | 0.261 |  90 | 0.028 |    0.625 |    0.733 |
| 7            | 0.809 | 0.221 |  90 | 0.023 |    0.763 |    0.854 |

Task-relevant feature visibility by stimulus strength (expts 1-4)
summary stats

## Feature visibility across successive stim strenghts

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subjectID" for ANOVA.

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

<table class="kable_wrapper">
<caption>
Feature visibility between stimulus strengths 1 vs 2 (expts 1-3) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |    SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|-------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  88 | 27.638 | 22.981 | 105.836 | 0.000 | \*     | 0.487 |
| 2   | site                        |   1 |  88 |  0.049 | 22.981 |   0.187 | 0.667 |        | 0.002 |
| 3   | attention                   |   2 | 176 |  2.124 |  3.469 |  53.880 | 0.000 | \*     | 0.068 |
| 5   | stimStrength                |   1 |  88 |  2.296 |  2.011 | 100.462 | 0.000 | \*     | 0.073 |
| 4   | site:attention              |   2 | 176 |  0.004 |  3.469 |   0.095 | 0.909 |        | 0.000 |
| 6   | site:stimStrength           |   1 |  88 |  0.008 |  2.011 |   0.369 | 0.545 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 176 |  0.421 |  0.614 |  60.355 | 0.000 | \*     | 0.014 |
| 8   | site:attention:stimStrength |   2 | 176 |  0.001 |  0.614 |   0.108 | 0.897 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |    p | p\<.05 |
|:----|:----------------------------|------:|-----:|:-------|
| 3   | attention                   | 0.308 | 0.00 | \*     |
| 4   | site:attention              | 0.308 | 0.00 | \*     |
| 7   | attention:stimStrength      | 0.944 | 0.08 |        |
| 8   | site:attention:stimStrength | 0.944 | 0.08 |        |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.591 |   0.000 | \*           | 0.594 |   0.000 | \*           |
| 4   | site:attention              | 0.591 |   0.800 |              | 0.594 |   0.801 |              |
| 7   | attention:stimStrength      | 0.947 |   0.000 | \*           | 0.967 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.947 |   0.888 |              | 0.967 |   0.891 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subjectID" for ANOVA.

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

<table class="kable_wrapper">
<caption>
Feature visibility between stimulus strengths 2 vs 3 (expts 1-3) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |    SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|-------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  88 | 69.680 | 25.006 | 245.214 | 0.000 | \*     | 0.690 |
| 2   | site                        |   1 |  88 |  0.032 | 25.006 |   0.113 | 0.737 |        | 0.001 |
| 3   | attention                   |   2 | 176 |  6.170 |  4.649 | 116.784 | 0.000 | \*     | 0.164 |
| 5   | stimStrength                |   1 |  88 |  2.481 |  1.104 | 197.781 | 0.000 | \*     | 0.073 |
| 4   | site:attention              |   2 | 176 |  0.001 |  4.649 |   0.019 | 0.981 |        | 0.000 |
| 6   | site:stimStrength           |   1 |  88 |  0.018 |  1.104 |   1.417 | 0.237 |        | 0.001 |
| 7   | attention:stimStrength      |   2 | 176 |  0.173 |  0.605 |  25.129 | 0.000 | \*     | 0.005 |
| 8   | site:attention:stimStrength |   2 | 176 |  0.008 |  0.605 |   1.203 | 0.303 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |     p | p\<.05 |
|:----|:----------------------------|------:|------:|:-------|
| 3   | attention                   | 0.430 | 0.000 | \*     |
| 4   | site:attention              | 0.430 | 0.000 | \*     |
| 7   | attention:stimStrength      | 0.998 | 0.924 |        |
| 8   | site:attention:stimStrength | 0.998 | 0.924 |        |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.637 |   0.000 | \*           | 0.642 |   0.000 | \*           |
| 4   | site:attention              | 0.637 |   0.934 |              | 0.642 |   0.935 |              |
| 7   | attention:stimStrength      | 0.998 |   0.000 | \*           | 1.021 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.998 |   0.303 |              | 1.021 |   0.303 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subjectID" for ANOVA.

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

<table class="kable_wrapper">
<caption>
Feature visibility between stimulus strengths 3 vs 4 (expts 1-3) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  88 | 120.313 | 24.523 | 431.740 | 0.000 | \*     | 0.796 |
| 2   | site                        |   1 |  88 |   0.002 | 24.523 |   0.009 | 0.926 |        | 0.000 |
| 3   | attention                   |   2 | 176 |  10.804 |  4.908 | 193.696 | 0.000 | \*     | 0.260 |
| 5   | stimStrength                |   1 |  88 |   1.095 |  0.631 | 152.672 | 0.000 | \*     | 0.034 |
| 4   | site:attention              |   2 | 176 |   0.016 |  4.908 |   0.279 | 0.757 |        | 0.001 |
| 6   | site:stimStrength           |   1 |  88 |   0.009 |  0.631 |   1.274 | 0.262 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 176 |   0.185 |  0.683 |  23.789 | 0.000 | \*     | 0.006 |
| 8   | site:attention:stimStrength |   2 | 176 |   0.000 |  0.683 |   0.036 | 0.965 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |     p | p\<.05 |
|:----|:----------------------------|------:|------:|:-------|
| 3   | attention                   | 0.583 | 0.000 | \*     |
| 4   | site:attention              | 0.583 | 0.000 | \*     |
| 7   | attention:stimStrength      | 0.927 | 0.038 | \*     |
| 8   | site:attention:stimStrength | 0.927 | 0.038 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.706 |   0.000 | \*           | 0.714 |   0.000 | \*           |
| 4   | site:attention              | 0.706 |   0.678 |              | 0.714 |   0.681 |              |
| 7   | attention:stimStrength      | 0.932 |   0.000 | \*           | 0.952 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.932 |   0.958 |              | 0.952 |   0.960 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subjectID" for ANOVA.

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

<table class="kable_wrapper">
<caption>
Feature visibility between stimulus strengths 4 vs 5 (expts 1-3) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  88 | 170.663 | 23.285 | 644.968 | 0.000 | \*     | 0.856 |
| 2   | site                        |   1 |  88 |   0.006 | 23.285 |   0.023 | 0.879 |        | 0.000 |
| 3   | attention                   |   2 | 176 |  13.479 |  4.376 | 271.063 | 0.000 | \*     | 0.319 |
| 5   | stimStrength                |   1 |  88 |   1.100 |  0.555 | 174.586 | 0.000 | \*     | 0.037 |
| 4   | site:attention              |   2 | 176 |   0.023 |  4.376 |   0.467 | 0.628 |        | 0.001 |
| 6   | site:stimStrength           |   1 |  88 |   0.004 |  0.555 |   0.701 | 0.405 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 176 |   0.082 |  0.544 |  13.201 | 0.000 | \*     | 0.003 |
| 8   | site:attention:stimStrength |   2 | 176 |   0.000 |  0.544 |   0.068 | 0.934 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |     p | p\<.05 |
|:----|:----------------------------|------:|------:|:-------|
| 3   | attention                   | 0.585 | 0.000 | \*     |
| 4   | site:attention              | 0.585 | 0.000 | \*     |
| 7   | attention:stimStrength      | 0.889 | 0.006 | \*     |
| 8   | site:attention:stimStrength | 0.889 | 0.006 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.707 |   0.000 | \*           | 0.715 |   0.000 | \*           |
| 4   | site:attention              | 0.707 |   0.561 |              | 0.715 |   0.563 |              |
| 7   | attention:stimStrength      | 0.900 |   0.000 | \*           | 0.918 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.900 |   0.918 |              | 0.918 |   0.921 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subjectID" for ANOVA.

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

<table class="kable_wrapper">
<caption>
Feature visibility between stimulus strengths 5 vs 6 (expts 1-3) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |       F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|--------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  88 | 223.511 | 20.844 | 943.620 | 0.000 | \*     | 0.898 |
| 2   | site                        |   1 |  88 |   0.003 | 20.844 |   0.012 | 0.913 |        | 0.000 |
| 3   | attention                   |   2 | 176 |  13.276 |  3.650 | 320.096 | 0.000 | \*     | 0.343 |
| 5   | stimStrength                |   1 |  88 |   0.702 |  0.367 | 168.060 | 0.000 | \*     | 0.027 |
| 4   | site:attention              |   2 | 176 |   0.036 |  3.650 |   0.860 | 0.425 |        | 0.001 |
| 6   | site:stimStrength           |   1 |  88 |   0.002 |  0.367 |   0.403 | 0.527 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 176 |   0.002 |  0.558 |   0.364 | 0.695 |        | 0.000 |
| 8   | site:attention:stimStrength |   2 | 176 |   0.001 |  0.558 |   0.150 | 0.860 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |     p | p\<.05 |
|:----|:----------------------------|------:|------:|:-------|
| 3   | attention                   | 0.518 | 0.000 | \*     |
| 4   | site:attention              | 0.518 | 0.000 | \*     |
| 7   | attention:stimStrength      | 0.941 | 0.072 |        |
| 8   | site:attention:stimStrength | 0.941 | 0.072 |        |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.675 |   0.000 | \*           | 0.682 |   0.000 | \*           |
| 4   | site:attention              | 0.675 |   0.387 |              | 0.682 |   0.388 |              |
| 7   | attention:stimStrength      | 0.944 |   0.683 |              | 0.965 |   0.688 |              |
| 8   | site:attention:stimStrength | 0.944 |   0.849 |              | 0.965 |   0.853 |              |

</td>
</tr>
</tbody>
</table>

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subjectID" for ANOVA.

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

<table class="kable_wrapper">
<caption>
Feature visibility between stimulus strengths 6 vs 7 (expts 1-3) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                      | DFn | DFd |     SSn |    SSd |        F |     p | p\<.05 |   ges |
|:----|:----------------------------|----:|----:|--------:|-------:|---------:|------:|:-------|------:|
| 1   | (Intercept)                 |   1 |  88 | 298.876 | 14.848 | 1771.412 | 0.000 | \*     | 0.937 |
| 2   | site                        |   1 |  88 |   0.000 | 14.848 |    0.002 | 0.968 |        | 0.000 |
| 3   | attention                   |   2 | 176 |  11.270 |  3.122 |  317.706 | 0.000 | \*     | 0.359 |
| 5   | stimStrength                |   1 |  88 |   2.250 |  1.454 |  136.222 | 0.000 | \*     | 0.101 |
| 4   | site:attention              |   2 | 176 |   0.054 |  3.122 |    1.514 | 0.223 |        | 0.003 |
| 6   | site:stimStrength           |   1 |  88 |   0.006 |  1.454 |    0.364 | 0.548 |        | 0.000 |
| 7   | attention:stimStrength      |   2 | 176 |   0.140 |  0.664 |   18.506 | 0.000 | \*     | 0.007 |
| 8   | site:attention:stimStrength |   2 | 176 |   0.002 |  0.664 |    0.301 | 0.740 |        | 0.000 |

</td>
<td>

|     | Effect                      |     W |     p | p\<.05 |
|:----|:----------------------------|------:|------:|:-------|
| 3   | attention                   | 0.381 | 0.000 | \*     |
| 4   | site:attention              | 0.381 | 0.000 | \*     |
| 7   | attention:stimStrength      | 0.932 | 0.047 | \*     |
| 8   | site:attention:stimStrength | 0.932 | 0.047 | \*     |

</td>
<td>

|     | Effect                      |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 3   | attention                   | 0.618 |   0.000 | \*           | 0.622 |   0.000 | \*           |
| 4   | site:attention              | 0.618 |   0.225 |              | 0.622 |   0.225 |              |
| 7   | attention:stimStrength      | 0.936 |   0.000 | \*           | 0.956 |   0.000 | \*           |
| 8   | site:attention:stimStrength | 0.936 |   0.726 |              | 0.956 |   0.731 |              |

</td>
</tr>
</tbody>
</table>

## Feature vs stimulus visibility

Remove contrast 0 for Expt 3 for balanced design

    ##               Df Sum Sq Mean Sq F value Pr(>F)    
    ## pSeen          1  40.44   40.44 1087.43 <2e-16 ***
    ## subjectID     89  99.81    1.12   30.15 <2e-16 ***
    ## Residuals   1799  66.91    0.04                   
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

    ## Warning in knit_print.huxtable(ht): Unrecognized output format "gfm+tex". Using `to_screen` to print huxtables.
    ## Set options("huxtable.knitr_output_format") manually to "latex", "html", "rtf", "docx", "pptx", "md" or "screen".

          ┌──────────────────────────────────────────────────────────┐
          │ Effect   DFn        DFd     F          p   p<.05     ges │
          ├──────────────────────────────────────────────────────────┤
          │ pSeen      1   1.89e+03   458   3.75e-91   *       0.195 │
          └──────────────────────────────────────────────────────────┘

Column names: Effect, DFn, DFd, F, p, p\<.05, ges

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subjectID" for ANOVA.

    ## Warning: Collapsing data to cell means. *IF* the requested effects are a subset
    ## of the full design, you must use the "within_full" argument, else results may
    ## be inaccurate.

    ## Coefficient covariances computed by hccm()

<table class="kable_wrapper">
<tbody>
<tr>
<td>

| Effect | DFn | DFd | SSn |   SSd |     F |     p | p\<.05 | ges |
|:-------|----:|----:|----:|------:|------:|------:|:-------|----:|
| site   |   1 |  88 |   0 | 2.854 | 0.009 | 0.923 |        |   0 |

</td>
<td>

| DFn | DFd | SSn |   SSd |     F |     p | p\<.05 |
|----:|----:|----:|------:|------:|------:|:-------|
|   1 |  88 |   0 | 1.184 | 0.014 | 0.906 |        |

</td>
</tr>
</tbody>
</table>
