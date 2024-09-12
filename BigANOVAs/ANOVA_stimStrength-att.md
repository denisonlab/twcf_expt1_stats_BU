ANOVA_stimStrength-att
================
Karen Tian
2024-09-11

Performance  
• [all
expts](#Performance-as-a-function-of-stimulus-strength-(all-expts))  
Overall visibility  
Task-relevant feature visibility

## Performance as a function of stimulus strength (all expts)

Remove contrast 0 for Expt 3 for balanced design

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: "stimType" will be treated as numeric.

    ## Warning: "taskType" will be treated as numeric.

    ## Warning: Data is unbalanced (unequal N per group). Make sure you specified a
    ## well-considered value for the type argument to ezANOVA().

<table class="kable_wrapper">
<caption>
Performance by stimulus strength (expts 1-4) ANOVA
</caption>
<tbody>
<tr>
<td>

|     | Effect                                        | DFn |  DFd |      SSn |   SSd |         F |     p | p\<.05 |   ges |
|:----|:----------------------------------------------|----:|-----:|---------:|------:|----------:|------:|:-------|------:|
| 1   | (Intercept)                                   |   1 |  111 | 1458.355 | 7.692 | 21043.961 | 0.000 | \*     | 0.988 |
| 2   | site                                          |   1 |  111 |    0.407 | 7.692 |     5.873 | 0.017 | \*     | 0.023 |
| 3   | stimType                                      |   1 |  111 |    0.026 | 7.692 |     0.370 | 0.544 |        | 0.001 |
| 4   | taskType                                      |   1 |  111 |    0.164 | 7.692 |     2.372 | 0.126 |        | 0.009 |
| 9   | attention                                     |   2 |  222 |   18.467 | 2.296 |   892.798 | 0.000 | \*     | 0.517 |
| 17  | stimStrength                                  |   6 |  666 |   26.764 | 3.971 |   748.050 | 0.000 | \*     | 0.608 |
| 5   | site:stimType                                 |   1 |  111 |    0.001 | 7.692 |     0.008 | 0.929 |        | 0.000 |
| 6   | site:taskType                                 |   1 |  111 |    0.512 | 7.692 |     7.382 | 0.008 | \*     | 0.029 |
| 7   | stimType:taskType                             |   1 |  111 |    0.356 | 7.692 |     5.136 | 0.025 | \*     | 0.020 |
| 10  | site:attention                                |   2 |  222 |    0.057 | 2.296 |     2.777 | 0.064 |        | 0.003 |
| 11  | stimType:attention                            |   2 |  222 |    0.664 | 2.296 |    32.079 | 0.000 | \*     | 0.037 |
| 12  | taskType:attention                            |   2 |  222 |    0.144 | 2.296 |     6.975 | 0.001 | \*     | 0.008 |
| 18  | site:stimStrength                             |   6 |  666 |    0.006 | 3.971 |     0.177 | 0.983 |        | 0.000 |
| 19  | stimType:stimStrength                         |   6 |  666 |    0.053 | 3.971 |     1.469 | 0.186 |        | 0.003 |
| 20  | taskType:stimStrength                         |   6 |  666 |    0.555 | 3.971 |    15.521 | 0.000 | \*     | 0.031 |
| 25  | attention:stimStrength                        |  12 | 1332 |    1.587 | 3.267 |    53.926 | 0.000 | \*     | 0.084 |
| 8   | site:stimType:taskType                        |   1 |  111 |    0.043 | 7.692 |     0.616 | 0.434 |        | 0.002 |
| 13  | site:stimType:attention                       |   2 |  222 |    0.022 | 2.296 |     1.060 | 0.348 |        | 0.001 |
| 14  | site:taskType:attention                       |   2 |  222 |    0.000 | 2.296 |     0.024 | 0.977 |        | 0.000 |
| 15  | stimType:taskType:attention                   |   2 |  222 |    0.103 | 2.296 |     4.989 | 0.008 | \*     | 0.006 |
| 21  | site:stimType:stimStrength                    |   6 |  666 |    0.023 | 3.971 |     0.639 | 0.699 |        | 0.001 |
| 22  | site:taskType:stimStrength                    |   6 |  666 |    0.022 | 3.971 |     0.606 | 0.726 |        | 0.001 |
| 23  | stimType:taskType:stimStrength                |   6 |  666 |    0.869 | 3.971 |    24.292 | 0.000 | \*     | 0.048 |
| 26  | site:attention:stimStrength                   |  12 | 1332 |    0.060 | 3.267 |     2.045 | 0.018 | \*     | 0.003 |
| 27  | stimType:attention:stimStrength               |  12 | 1332 |    0.118 | 3.267 |     4.008 | 0.000 | \*     | 0.007 |
| 28  | taskType:attention:stimStrength               |  12 | 1332 |    0.207 | 3.267 |     7.027 | 0.000 | \*     | 0.012 |
| 16  | site:stimType:taskType:attention              |   2 |  222 |    0.008 | 2.296 |     0.367 | 0.693 |        | 0.000 |
| 24  | site:stimType:taskType:stimStrength           |   6 |  666 |    0.056 | 3.971 |     1.552 | 0.159 |        | 0.003 |
| 29  | site:stimType:attention:stimStrength          |  12 | 1332 |    0.060 | 3.267 |     2.043 | 0.018 | \*     | 0.003 |
| 30  | site:taskType:attention:stimStrength          |  12 | 1332 |    0.029 | 3.267 |     0.991 | 0.455 |        | 0.002 |
| 31  | stimType:taskType:attention:stimStrength      |  12 | 1332 |    0.070 | 3.267 |     2.366 | 0.005 | \*     | 0.004 |
| 32  | site:stimType:taskType:attention:stimStrength |  12 | 1332 |    0.068 | 3.267 |     2.294 | 0.007 | \*     | 0.004 |

</td>
<td>

|     | Effect                                        |     W |   p | p\<.05 |
|:----|:----------------------------------------------|------:|----:|:-------|
| 9   | attention                                     | 0.564 |   0 | \*     |
| 10  | site:attention                                | 0.564 |   0 | \*     |
| 11  | stimType:attention                            | 0.564 |   0 | \*     |
| 12  | taskType:attention                            | 0.564 |   0 | \*     |
| 13  | site:stimType:attention                       | 0.564 |   0 | \*     |
| 14  | site:taskType:attention                       | 0.564 |   0 | \*     |
| 15  | stimType:taskType:attention                   | 0.564 |   0 | \*     |
| 16  | site:stimType:taskType:attention              | 0.564 |   0 | \*     |
| 17  | stimStrength                                  | 0.073 |   0 | \*     |
| 18  | site:stimStrength                             | 0.073 |   0 | \*     |
| 19  | stimType:stimStrength                         | 0.073 |   0 | \*     |
| 20  | taskType:stimStrength                         | 0.073 |   0 | \*     |
| 21  | site:stimType:stimStrength                    | 0.073 |   0 | \*     |
| 22  | site:taskType:stimStrength                    | 0.073 |   0 | \*     |
| 23  | stimType:taskType:stimStrength                | 0.073 |   0 | \*     |
| 24  | site:stimType:taskType:stimStrength           | 0.073 |   0 | \*     |
| 25  | attention:stimStrength                        | 0.086 |   0 | \*     |
| 26  | site:attention:stimStrength                   | 0.086 |   0 | \*     |
| 27  | stimType:attention:stimStrength               | 0.086 |   0 | \*     |
| 28  | taskType:attention:stimStrength               | 0.086 |   0 | \*     |
| 29  | site:stimType:attention:stimStrength          | 0.086 |   0 | \*     |
| 30  | site:taskType:attention:stimStrength          | 0.086 |   0 | \*     |
| 31  | stimType:taskType:attention:stimStrength      | 0.086 |   0 | \*     |
| 32  | site:stimType:taskType:attention:stimStrength | 0.086 |   0 | \*     |

</td>
<td>

|     | Effect                                        |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 9   | attention                                     | 0.696 |   0.000 | \*           | 0.702 |   0.000 | \*           |
| 10  | site:attention                                | 0.696 |   0.084 |              | 0.702 |   0.084 |              |
| 11  | stimType:attention                            | 0.696 |   0.000 | \*           | 0.702 |   0.000 | \*           |
| 12  | taskType:attention                            | 0.696 |   0.004 | \*           | 0.702 |   0.004 | \*           |
| 13  | site:stimType:attention                       | 0.696 |   0.328 |              | 0.702 |   0.328 |              |
| 14  | site:taskType:attention                       | 0.696 |   0.938 |              | 0.702 |   0.939 |              |
| 15  | stimType:taskType:attention                   | 0.696 |   0.017 | \*           | 0.702 |   0.016 | \*           |
| 16  | site:stimType:taskType:attention              | 0.696 |   0.616 |              | 0.702 |   0.618 |              |
| 17  | stimStrength                                  | 0.484 |   0.000 | \*           | 0.499 |   0.000 | \*           |
| 18  | site:stimStrength                             | 0.484 |   0.907 |              | 0.499 |   0.912 |              |
| 19  | stimType:stimStrength                         | 0.484 |   0.224 |              | 0.499 |   0.223 |              |
| 20  | taskType:stimStrength                         | 0.484 |   0.000 | \*           | 0.499 |   0.000 | \*           |
| 21  | site:stimType:stimStrength                    | 0.484 |   0.586 |              | 0.499 |   0.590 |              |
| 22  | site:taskType:stimStrength                    | 0.484 |   0.607 |              | 0.499 |   0.611 |              |
| 23  | stimType:taskType:stimStrength                | 0.484 |   0.000 | \*           | 0.499 |   0.000 | \*           |
| 24  | site:stimType:taskType:stimStrength           | 0.484 |   0.202 |              | 0.499 |   0.201 |              |
| 25  | attention:stimStrength                        | 0.748 |   0.000 | \*           | 0.820 |   0.000 | \*           |
| 26  | site:attention:stimStrength                   | 0.748 |   0.032 | \*           | 0.820 |   0.027 | \*           |
| 27  | stimType:attention:stimStrength               | 0.748 |   0.000 | \*           | 0.820 |   0.000 | \*           |
| 28  | taskType:attention:stimStrength               | 0.748 |   0.000 | \*           | 0.820 |   0.000 | \*           |
| 29  | site:stimType:attention:stimStrength          | 0.748 |   0.032 | \*           | 0.820 |   0.027 | \*           |
| 30  | site:taskType:attention:stimStrength          | 0.748 |   0.445 |              | 0.820 |   0.448 |              |
| 31  | stimType:taskType:attention:stimStrength      | 0.748 |   0.012 | \*           | 0.820 |   0.009 | \*           |
| 32  | site:stimType:taskType:attention:stimStrength | 0.748 |   0.015 | \*           | 0.820 |   0.012 | \*           |

</td>
</tr>
</tbody>
</table>

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

## Performance across successive stim strenghts

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
  between = .(site,stimType,taskType),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more levels from variable "stimStrength".
    ## Refactoring for ANOVA.

    ## Warning: "stimType" will be treated as numeric.

    ## Warning: "taskType" will be treated as numeric.

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

|     | Effect                                        | DFn |  DFd |     SSn |    SSd |        F |     p | p\<.05 |   ges |
|:----|:----------------------------------------------|----:|-----:|--------:|-------:|---------:|------:|:-------|------:|
| 1   | (Intercept)                                   |   1 |  111 | 757.182 | 32.091 | 2619.066 | 0.000 | \*     | 0.916 |
| 2   | site                                          |   1 |  111 |   0.037 | 32.091 |    0.130 | 0.720 |        | 0.001 |
| 3   | stimType                                      |   1 |  111 |  11.362 | 32.091 |   39.300 | 0.000 | \*     | 0.141 |
| 4   | taskType                                      |   1 |  111 |  60.806 | 32.091 |  210.324 | 0.000 | \*     | 0.467 |
| 9   | attention                                     |   2 |  222 |   3.775 |  5.089 |   82.333 | 0.000 | \*     | 0.052 |
| 17  | stimStrength                                  |   6 |  666 | 130.266 | 26.546 |  544.707 | 0.000 | \*     | 0.653 |
| 5   | site:stimType                                 |   1 |  111 |   0.006 | 32.091 |    0.019 | 0.890 |        | 0.000 |
| 6   | site:taskType                                 |   1 |  111 |   0.156 | 32.091 |    0.539 | 0.464 |        | 0.002 |
| 7   | stimType:taskType                             |   1 |  111 |   3.179 | 32.091 |   10.995 | 0.001 | \*     | 0.044 |
| 10  | site:attention                                |   2 |  222 |   0.118 |  5.089 |    2.565 | 0.079 |        | 0.002 |
| 11  | stimType:attention                            |   2 |  222 |   1.150 |  5.089 |   25.073 | 0.000 | \*     | 0.016 |
| 12  | taskType:attention                            |   2 |  222 |   2.343 |  5.089 |   51.099 | 0.000 | \*     | 0.033 |
| 18  | site:stimStrength                             |   6 |  666 |   0.137 | 26.546 |    0.572 | 0.753 |        | 0.002 |
| 19  | stimType:stimStrength                         |   6 |  666 |   5.412 | 26.546 |   22.630 | 0.000 | \*     | 0.072 |
| 20  | taskType:stimStrength                         |   6 |  666 |  17.603 | 26.546 |   73.608 | 0.000 | \*     | 0.202 |
| 25  | attention:stimStrength                        |  12 | 1332 |   3.430 |  5.638 |   67.516 | 0.000 | \*     | 0.047 |
| 8   | site:stimType:taskType                        |   1 |  111 |   0.004 | 32.091 |    0.012 | 0.913 |        | 0.000 |
| 13  | site:stimType:attention                       |   2 |  222 |   0.041 |  5.089 |    0.905 | 0.406 |        | 0.001 |
| 14  | site:taskType:attention                       |   2 |  222 |   0.332 |  5.089 |    7.233 | 0.001 | \*     | 0.005 |
| 15  | stimType:taskType:attention                   |   2 |  222 |   0.091 |  5.089 |    1.984 | 0.140 |        | 0.001 |
| 21  | site:stimType:stimStrength                    |   6 |  666 |   0.192 | 26.546 |    0.801 | 0.569 |        | 0.003 |
| 22  | site:taskType:stimStrength                    |   6 |  666 |   0.415 | 26.546 |    1.737 | 0.110 |        | 0.006 |
| 23  | stimType:taskType:stimStrength                |   6 |  666 |   1.728 | 26.546 |    7.226 | 0.000 | \*     | 0.024 |
| 26  | site:attention:stimStrength                   |  12 | 1332 |   0.105 |  5.638 |    2.071 | 0.016 | \*     | 0.002 |
| 27  | stimType:attention:stimStrength               |  12 | 1332 |   0.318 |  5.638 |    6.270 | 0.000 | \*     | 0.005 |
| 28  | taskType:attention:stimStrength               |  12 | 1332 |   1.670 |  5.638 |   32.871 | 0.000 | \*     | 0.024 |
| 16  | site:stimType:taskType:attention              |   2 |  222 |   0.071 |  5.089 |    1.556 | 0.213 |        | 0.001 |
| 24  | site:stimType:taskType:stimStrength           |   6 |  666 |   0.475 | 26.546 |    1.986 | 0.065 |        | 0.007 |
| 29  | site:stimType:attention:stimStrength          |  12 | 1332 |   0.032 |  5.638 |    0.632 | 0.816 |        | 0.000 |
| 30  | site:taskType:attention:stimStrength          |  12 | 1332 |   0.054 |  5.638 |    1.059 | 0.391 |        | 0.001 |
| 31  | stimType:taskType:attention:stimStrength      |  12 | 1332 |   0.138 |  5.638 |    2.720 | 0.001 | \*     | 0.002 |
| 32  | site:stimType:taskType:attention:stimStrength |  12 | 1332 |   0.028 |  5.638 |    0.559 | 0.876 |        | 0.000 |

</td>
<td>

|     | Effect                                        |     W |   p | p\<.05 |
|:----|:----------------------------------------------|------:|----:|:-------|
| 9   | attention                                     | 0.566 |   0 | \*     |
| 10  | site:attention                                | 0.566 |   0 | \*     |
| 11  | stimType:attention                            | 0.566 |   0 | \*     |
| 12  | taskType:attention                            | 0.566 |   0 | \*     |
| 13  | site:stimType:attention                       | 0.566 |   0 | \*     |
| 14  | site:taskType:attention                       | 0.566 |   0 | \*     |
| 15  | stimType:taskType:attention                   | 0.566 |   0 | \*     |
| 16  | site:stimType:taskType:attention              | 0.566 |   0 | \*     |
| 17  | stimStrength                                  | 0.005 |   0 | \*     |
| 18  | site:stimStrength                             | 0.005 |   0 | \*     |
| 19  | stimType:stimStrength                         | 0.005 |   0 | \*     |
| 20  | taskType:stimStrength                         | 0.005 |   0 | \*     |
| 21  | site:stimType:stimStrength                    | 0.005 |   0 | \*     |
| 22  | site:taskType:stimStrength                    | 0.005 |   0 | \*     |
| 23  | stimType:taskType:stimStrength                | 0.005 |   0 | \*     |
| 24  | site:stimType:taskType:stimStrength           | 0.005 |   0 | \*     |
| 25  | attention:stimStrength                        | 0.016 |   0 | \*     |
| 26  | site:attention:stimStrength                   | 0.016 |   0 | \*     |
| 27  | stimType:attention:stimStrength               | 0.016 |   0 | \*     |
| 28  | taskType:attention:stimStrength               | 0.016 |   0 | \*     |
| 29  | site:stimType:attention:stimStrength          | 0.016 |   0 | \*     |
| 30  | site:taskType:attention:stimStrength          | 0.016 |   0 | \*     |
| 31  | stimType:taskType:attention:stimStrength      | 0.016 |   0 | \*     |
| 32  | site:stimType:taskType:attention:stimStrength | 0.016 |   0 | \*     |

</td>
<td>

|     | Effect                                        |   GGe | p\[GG\] | p\[GG\]\<.05 |   HFe | p\[HF\] | p\[HF\]\<.05 |
|:----|:----------------------------------------------|------:|--------:|:-------------|------:|--------:|:-------------|
| 9   | attention                                     | 0.697 |   0.000 | \*           | 0.704 |   0.000 | \*           |
| 10  | site:attention                                | 0.697 |   0.099 |              | 0.704 |   0.098 |              |
| 11  | stimType:attention                            | 0.697 |   0.000 | \*           | 0.704 |   0.000 | \*           |
| 12  | taskType:attention                            | 0.697 |   0.000 | \*           | 0.704 |   0.000 | \*           |
| 13  | site:stimType:attention                       | 0.697 |   0.375 |              | 0.704 |   0.375 |              |
| 14  | site:taskType:attention                       | 0.697 |   0.003 | \*           | 0.704 |   0.003 | \*           |
| 15  | stimType:taskType:attention                   | 0.697 |   0.155 |              | 0.704 |   0.154 |              |
| 16  | site:stimType:taskType:attention              | 0.697 |   0.217 |              | 0.704 |   0.217 |              |
| 17  | stimStrength                                  | 0.343 |   0.000 | \*           | 0.349 |   0.000 | \*           |
| 18  | site:stimStrength                             | 0.343 |   0.570 |              | 0.349 |   0.573 |              |
| 19  | stimType:stimStrength                         | 0.343 |   0.000 | \*           | 0.349 |   0.000 | \*           |
| 20  | taskType:stimStrength                         | 0.343 |   0.000 | \*           | 0.349 |   0.000 | \*           |
| 21  | site:stimType:stimStrength                    | 0.343 |   0.453 |              | 0.349 |   0.455 |              |
| 22  | site:taskType:stimStrength                    | 0.343 |   0.177 |              | 0.349 |   0.177 |              |
| 23  | stimType:taskType:stimStrength                | 0.343 |   0.001 | \*           | 0.349 |   0.001 | \*           |
| 24  | site:stimType:taskType:stimStrength           | 0.343 |   0.138 |              | 0.349 |   0.137 |              |
| 25  | attention:stimStrength                        | 0.532 |   0.000 | \*           | 0.568 |   0.000 | \*           |
| 26  | site:attention:stimStrength                   | 0.532 |   0.050 |              | 0.568 |   0.046 | \*           |
| 27  | stimType:attention:stimStrength               | 0.532 |   0.000 | \*           | 0.568 |   0.000 | \*           |
| 28  | taskType:attention:stimStrength               | 0.532 |   0.000 | \*           | 0.568 |   0.000 | \*           |
| 29  | site:stimType:attention:stimStrength          | 0.532 |   0.714 |              | 0.568 |   0.725 |              |
| 30  | site:taskType:attention:stimStrength          | 0.532 |   0.387 |              | 0.568 |   0.388 |              |
| 31  | stimType:taskType:attention:stimStrength      | 0.532 |   0.011 | \*           | 0.568 |   0.009 | \*           |
| 32  | site:stimType:taskType:attention:stimStrength | 0.532 |   0.773 |              | 0.568 |   0.784 |              |

</td>
</tr>
</tbody>
</table>

``` r
## Overall visibility by stimulus strength
d <- dS %>% group_by(stimStrength) %>%
  summarise(mean=mean(pSeen), sd=sd(pSeen), n=n_distinct(subjectID)) %>% mutate(se = sd / sqrt(n),
         ci.lower = mean - qt(1 - (0.05 / 2), n - 1) * se,
         ci.upper = mean + qt(1 - (0.05 / 2), n - 1) * se)
knitr::kable(d, digits=3, caption="Overall visibility by stimulus strength (expts 1-4) summary stats")
```

| stimStrength |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-------------|------:|------:|----:|------:|---------:|---------:|
| 1            | 0.182 | 0.220 | 119 | 0.020 |    0.142 |    0.222 |
| 2            | 0.353 | 0.296 | 119 | 0.027 |    0.300 |    0.407 |
| 3            | 0.460 | 0.341 | 119 | 0.031 |    0.399 |    0.522 |
| 4            | 0.526 | 0.338 | 119 | 0.031 |    0.464 |    0.587 |
| 5            | 0.656 | 0.290 | 119 | 0.027 |    0.603 |    0.708 |
| 6            | 0.789 | 0.214 | 119 | 0.020 |    0.750 |    0.828 |
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
         ci.lower = mean - qt(1 - (0.05 / 2), n - 1) * se,
         ci.upper = mean + qt(1 - (0.05 / 2), n - 1) * se)
knitr::kable(d, digits=3, caption="Task-relevant feature visibility by stimulus strength (expts 1-4) summary stats")
```

| stimStrength |  mean |    sd |   n |    se | ci.lower | ci.upper |
|:-------------|------:|------:|----:|------:|---------:|---------:|
| 1            | 0.161 | 0.226 |  90 | 0.024 |    0.114 |    0.208 |
| 2            | 0.291 | 0.259 |  90 | 0.027 |    0.237 |    0.346 |
| 3            | 0.427 | 0.271 |  90 | 0.029 |    0.370 |    0.484 |
| 4            | 0.517 | 0.286 |  90 | 0.030 |    0.457 |    0.577 |
| 5            | 0.607 | 0.275 |  90 | 0.029 |    0.550 |    0.665 |
| 6            | 0.679 | 0.261 |  90 | 0.028 |    0.625 |    0.734 |
| 7            | 0.809 | 0.221 |  90 | 0.023 |    0.762 |    0.855 |

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
