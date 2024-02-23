TWCF FOHO BigANOVA3
================
Karen Tian
2024-02-21

## ANOVA 3

``` r
m_anova = ezANOVA(
  data = data,
  dv = .(AUC),
  wid = .(subject),
  within = .(att),
  between = .(site,expt),
  detailed = TRUE,
  )
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
DFn
</th>
<th style="text-align:right;">
DFd
</th>
<th style="text-align:right;">
SSn
</th>
<th style="text-align:right;">
SSd
</th>
<th style="text-align:right;">
F
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
<th style="text-align:right;">
ges
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
1
</td>
<td style="text-align:left;">
(Intercept)
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
84
</td>
<td style="text-align:right;">
3.4750340
</td>
<td style="text-align:right;">
1.4500972
</td>
<td style="text-align:right;">
201.2988233
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.6756235
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  2
  </td>
  <td style="text-align:left;">
  site
  </td>
  <td style="text-align:right;">
  1
  </td>
  <td style="text-align:right;">
  84
  </td>
  <td style="text-align:right;">
  0.0308879
  </td>
  <td style="text-align:right;">
  1.4500972
  </td>
  <td style="text-align:right;">
  1.7892503
  </td>
  <td style="text-align:right;">
  0.1846280
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0181768
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  3
  </td>
  <td style="text-align:left;">
  expt
  </td>
  <td style="text-align:right;">
  2
  </td>
  <td style="text-align:right;">
  84
  </td>
  <td style="text-align:right;">
  0.3066300
  </td>
  <td style="text-align:right;">
  1.4500972
  </td>
  <td style="text-align:right;">
  8.8811009
  </td>
  <td style="text-align:right;">
  0.0003170
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.1552522
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    5
    </td>
    <td style="text-align:left;">
    att
    </td>
    <td style="text-align:right;">
    2
    </td>
    <td style="text-align:right;">
    168
    </td>
    <td style="text-align:right;">
    0.0099534
    </td>
    <td style="text-align:right;">
    0.2183166
    </td>
    <td style="text-align:right;">
    3.8297001
    </td>
    <td style="text-align:right;">
    0.0236365
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.0059304
      </td>
      </tr>
      <tr>
      <td style="text-align:left;">
      4
      </td>
      <td style="text-align:left;">
      site:expt
      </td>
      <td style="text-align:right;">
      2
      </td>
      <td style="text-align:right;">
      84
      </td>
      <td style="text-align:right;">
      0.0506244
      </td>
      <td style="text-align:right;">
      1.4500972
      </td>
      <td style="text-align:right;">
      1.4662630
      </td>
      <td style="text-align:right;">
      0.2366320
      </td>
      <td style="text-align:left;">
      </td>
      <td style="text-align:right;">
      0.0294492
      </td>
      </tr>
      <tr>
      <td style="text-align:left;">
      6
      </td>
      <td style="text-align:left;">
      site:att
      </td>
      <td style="text-align:right;">
      2
      </td>
      <td style="text-align:right;">
      168
      </td>
      <td style="text-align:right;">
      0.0012471
      </td>
      <td style="text-align:right;">
      0.2183166
      </td>
      <td style="text-align:right;">
      0.4798481
      </td>
      <td style="text-align:right;">
      0.6197229
      </td>
      <td style="text-align:left;">
      </td>
      <td style="text-align:right;">
      0.0007469
      </td>
      </tr>
      <tr>
      <td style="text-align:left;">
      7
      </td>
      <td style="text-align:left;">
      expt:att
      </td>
      <td style="text-align:right;">
      4
      </td>
      <td style="text-align:right;">
      168
      </td>
      <td style="text-align:right;">
      0.0421698
      </td>
      <td style="text-align:right;">
      0.2183166
      </td>
      <td style="text-align:right;">
      8.1126805
      </td>
      <td style="text-align:right;">
      0.0000053
      </td>
      <td style="text-align:left;">

      - </td>
        <td style="text-align:right;">
        0.0246523
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        8
        </td>
        <td style="text-align:left;">
        site:expt:att
        </td>
        <td style="text-align:right;">
        4
        </td>
        <td style="text-align:right;">
        168
        </td>
        <td style="text-align:right;">
        0.0141094
        </td>
        <td style="text-align:right;">
        0.2183166
        </td>
        <td style="text-align:right;">
        2.7143748
        </td>
        <td style="text-align:right;">
        0.0316702
        </td>
        <td style="text-align:left;">

        - </td>
          <td style="text-align:right;">
          0.0083858
          </td>
          </tr>
          </tbody>
          </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
W
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
5
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.6021217
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:left;">

- </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  6
  </td>
  <td style="text-align:left;">
  site:att
  </td>
  <td style="text-align:right;">
  0.6021217
  </td>
  <td style="text-align:right;">
  0
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    7
    </td>
    <td style="text-align:left;">
    expt:att
    </td>
    <td style="text-align:right;">
    0.6021217
    </td>
    <td style="text-align:right;">
    0
    </td>
    <td style="text-align:left;">

    - </td>
      </tr>
      <tr>
      <td style="text-align:left;">
      8
      </td>
      <td style="text-align:left;">
      site:expt:att
      </td>
      <td style="text-align:right;">
      0.6021217
      </td>
      <td style="text-align:right;">
      0
      </td>
      <td style="text-align:left;">

      - </td>
        </tr>
        </tbody>
        </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
GGe
</th>
<th style="text-align:right;">
p\[GG\]
</th>
<th style="text-align:left;">
p\[GG\]\<.05
</th>
<th style="text-align:right;">
HFe
</th>
<th style="text-align:right;">
p\[HF\]
</th>
<th style="text-align:left;">
p\[HF\]\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
5
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.7153699
</td>
<td style="text-align:right;">
0.0378272
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7243184
  </td>
  <td style="text-align:right;">
  0.0372737
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    6
    </td>
    <td style="text-align:left;">
    site:att
    </td>
    <td style="text-align:right;">
    0.7153699
    </td>
    <td style="text-align:right;">
    0.5566397
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.7243184
    </td>
    <td style="text-align:right;">
    0.5589651
    </td>
    <td style="text-align:left;">
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    7
    </td>
    <td style="text-align:left;">
    expt:att
    </td>
    <td style="text-align:right;">
    0.7153699
    </td>
    <td style="text-align:right;">
    0.0000770
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.7243184
      </td>
      <td style="text-align:right;">
      0.0000707
      </td>
      <td style="text-align:left;">

      - </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        8
        </td>
        <td style="text-align:left;">
        site:expt:att
        </td>
        <td style="text-align:right;">
        0.7153699
        </td>
        <td style="text-align:right;">
        0.0504556
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.7243184
        </td>
        <td style="text-align:right;">
        0.0497160
        </td>
        <td style="text-align:left;">

        - </td>
          </tr>
          </tbody>
          </table>

</td>
</tr>
</tbody>
</table>

## Task-relevant feature visibility: BU

``` r
d <- data %>% filter(site=="1")
m_anova = ezANOVA(
  data = d,
  dv = .(AUC),
  wid = .(subject),
  within = .(att),
  between = .(expt),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subject" for ANOVA.

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
DFn
</th>
<th style="text-align:right;">
DFd
</th>
<th style="text-align:right;">
SSn
</th>
<th style="text-align:right;">
SSd
</th>
<th style="text-align:right;">
F
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
<th style="text-align:right;">
ges
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
(Intercept)
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
42
</td>
<td style="text-align:right;">
1.4253383
</td>
<td style="text-align:right;">
0.9185146
</td>
<td style="text-align:right;">
65.175018
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.5911536
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  expt
  </td>
  <td style="text-align:right;">
  2
  </td>
  <td style="text-align:right;">
  42
  </td>
  <td style="text-align:right;">
  0.1852453
  </td>
  <td style="text-align:right;">
  0.9185146
  </td>
  <td style="text-align:right;">
  4.235263
  </td>
  <td style="text-align:right;">
  0.0211077
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.1581914
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    att
    </td>
    <td style="text-align:right;">
    2
    </td>
    <td style="text-align:right;">
    84
    </td>
    <td style="text-align:right;">
    0.0087910
    </td>
    <td style="text-align:right;">
    0.0672603
    </td>
    <td style="text-align:right;">
    5.489460
    </td>
    <td style="text-align:right;">
    0.0057463
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.0088391
      </td>
      </tr>
      <tr>
      <td style="text-align:left;">
      expt:att
      </td>
      <td style="text-align:right;">
      4
      </td>
      <td style="text-align:right;">
      84
      </td>
      <td style="text-align:right;">
      0.0046113
      </td>
      <td style="text-align:right;">
      0.0672603
      </td>
      <td style="text-align:right;">
      1.439729
      </td>
      <td style="text-align:right;">
      0.2280611
      </td>
      <td style="text-align:left;">
      </td>
      <td style="text-align:right;">
      0.0046560
      </td>
      </tr>
      </tbody>
      </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
W
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.6189135
</td>
<td style="text-align:right;">
5.35e-05
</td>
<td style="text-align:left;">

- </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  4
  </td>
  <td style="text-align:left;">
  expt:att
  </td>
  <td style="text-align:right;">
  0.6189135
  </td>
  <td style="text-align:right;">
  5.35e-05
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    </tbody>
    </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
GGe
</th>
<th style="text-align:right;">
p\[GG\]
</th>
<th style="text-align:left;">
p\[GG\]\<.05
</th>
<th style="text-align:right;">
HFe
</th>
<th style="text-align:right;">
p\[HF\]
</th>
<th style="text-align:left;">
p\[HF\]\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.7240676
</td>
<td style="text-align:right;">
0.0126146
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7431201
  </td>
  <td style="text-align:right;">
  0.0119455
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    4
    </td>
    <td style="text-align:left;">
    expt:att
    </td>
    <td style="text-align:right;">
    0.7240676
    </td>
    <td style="text-align:right;">
    0.2407450
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.7431201
    </td>
    <td style="text-align:right;">
    0.2399288
    </td>
    <td style="text-align:left;">
    </td>
    </tr>
    </tbody>
    </table>

</td>
</tr>
</tbody>
</table>

## Task-relevant feature visibility: UCI

``` r
d <- data %>% filter(site=="0")
m_anova = ezANOVA(
  data = d,
  dv = .(AUC),
  wid = .(subject),
  within = .(att),
  between = .(expt),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subject" for ANOVA.

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
DFn
</th>
<th style="text-align:right;">
DFd
</th>
<th style="text-align:right;">
SSn
</th>
<th style="text-align:right;">
SSd
</th>
<th style="text-align:right;">
F
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
<th style="text-align:right;">
ges
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
(Intercept)
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
42
</td>
<td style="text-align:right;">
2.0805837
</td>
<td style="text-align:right;">
0.5315826
</td>
<td style="text-align:right;">
164.3855940
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7529555
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  expt
  </td>
  <td style="text-align:right;">
  2
  </td>
  <td style="text-align:right;">
  42
  </td>
  <td style="text-align:right;">
  0.1720091
  </td>
  <td style="text-align:right;">
  0.5315826
  </td>
  <td style="text-align:right;">
  6.7951637
  </td>
  <td style="text-align:right;">
  0.0027749
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.2012631
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    att
    </td>
    <td style="text-align:right;">
    2
    </td>
    <td style="text-align:right;">
    84
    </td>
    <td style="text-align:right;">
    0.0024095
    </td>
    <td style="text-align:right;">
    0.1510563
    </td>
    <td style="text-align:right;">
    0.6699493
    </td>
    <td style="text-align:right;">
    0.5144473
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.0035173
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    expt:att
    </td>
    <td style="text-align:right;">
    4
    </td>
    <td style="text-align:right;">
    84
    </td>
    <td style="text-align:right;">
    0.0516679
    </td>
    <td style="text-align:right;">
    0.1510563
    </td>
    <td style="text-align:right;">
    7.1829278
    </td>
    <td style="text-align:right;">
    0.0000504
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.0703629
      </td>
      </tr>
      </tbody>
      </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
W
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.591262
</td>
<td style="text-align:right;">
2.1e-05
</td>
<td style="text-align:left;">

- </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  4
  </td>
  <td style="text-align:left;">
  expt:att
  </td>
  <td style="text-align:right;">
  0.591262
  </td>
  <td style="text-align:right;">
  2.1e-05
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    </tbody>
    </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
GGe
</th>
<th style="text-align:right;">
p\[GG\]
</th>
<th style="text-align:left;">
p\[GG\]\<.05
</th>
<th style="text-align:right;">
HFe
</th>
<th style="text-align:right;">
p\[HF\]
</th>
<th style="text-align:left;">
p\[HF\]\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.7098552
</td>
<td style="text-align:right;">
0.4664280
</td>
<td style="text-align:left;">
</td>
<td style="text-align:right;">
0.7275398
</td>
<td style="text-align:right;">
0.4698634
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
4
</td>
<td style="text-align:left;">
expt:att
</td>
<td style="text-align:right;">
0.7098552
</td>
<td style="text-align:right;">
0.0004298
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7275398
  </td>
  <td style="text-align:right;">
  0.0003768
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    </tbody>
    </table>

</td>
</tr>
</tbody>
</table>

## Experiment 1: Task-relevant feature visibility

``` r
d1 <- data %>% filter(expt=="1")
m_anova = ezANOVA(
  data = d1,
  dv = .(AUC),
  wid = .(subject),
  within = .(att),
  between = .(site),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subject" for ANOVA.

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
DFn
</th>
<th style="text-align:right;">
DFd
</th>
<th style="text-align:right;">
SSn
</th>
<th style="text-align:right;">
SSd
</th>
<th style="text-align:right;">
F
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
<th style="text-align:right;">
ges
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
(Intercept)
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:right;">
1.1280732
</td>
<td style="text-align:right;">
0.4419566
</td>
<td style="text-align:right;">
71.4686654
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.6981226
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  site
  </td>
  <td style="text-align:right;">
  1
  </td>
  <td style="text-align:right;">
  28
  </td>
  <td style="text-align:right;">
  0.0066564
  </td>
  <td style="text-align:right;">
  0.4419566
  </td>
  <td style="text-align:right;">
  0.4217126
  </td>
  <td style="text-align:right;">
  0.5213757
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0134622
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  att
  </td>
  <td style="text-align:right;">
  2
  </td>
  <td style="text-align:right;">
  56
  </td>
  <td style="text-align:right;">
  0.0070946
  </td>
  <td style="text-align:right;">
  0.0458371
  </td>
  <td style="text-align:right;">
  4.3337963
  </td>
  <td style="text-align:right;">
  0.0177843
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.0143358
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    site:att
    </td>
    <td style="text-align:right;">
    2
    </td>
    <td style="text-align:right;">
    56
    </td>
    <td style="text-align:right;">
    0.0012310
    </td>
    <td style="text-align:right;">
    0.0458371
    </td>
    <td style="text-align:right;">
    0.7519681
    </td>
    <td style="text-align:right;">
    0.4761378
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.0025173
    </td>
    </tr>
    </tbody>
    </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
W
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.8358401
</td>
<td style="text-align:right;">
0.0888512
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
4
</td>
<td style="text-align:left;">
site:att
</td>
<td style="text-align:right;">
0.8358401
</td>
<td style="text-align:right;">
0.0888512
</td>
<td style="text-align:left;">
</td>
</tr>
</tbody>
</table>
</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
GGe
</th>
<th style="text-align:right;">
p\[GG\]
</th>
<th style="text-align:left;">
p\[GG\]\<.05
</th>
<th style="text-align:right;">
HFe
</th>
<th style="text-align:right;">
p\[HF\]
</th>
<th style="text-align:left;">
p\[HF\]\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.8589886
</td>
<td style="text-align:right;">
0.0233420
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.9097727
  </td>
  <td style="text-align:right;">
  0.0211616
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    4
    </td>
    <td style="text-align:left;">
    site:att
    </td>
    <td style="text-align:right;">
    0.8589886
    </td>
    <td style="text-align:right;">
    0.4580881
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.9097727
    </td>
    <td style="text-align:right;">
    0.4649149
    </td>
    <td style="text-align:left;">
    </td>
    </tr>
    </tbody>
    </table>

</td>
</tr>
</tbody>
</table>

## Experiment 3: Task-relevant feature visibility

``` r
d3 <- data %>% filter(expt=="3")
m_anova = ezANOVA(
  data = d3,
  dv = .(AUC),
  wid = .(subject),
  within = .(att),
  between = .(site),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subject" for ANOVA.

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
DFn
</th>
<th style="text-align:right;">
DFd
</th>
<th style="text-align:right;">
SSn
</th>
<th style="text-align:right;">
SSd
</th>
<th style="text-align:right;">
F
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
<th style="text-align:right;">
ges
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
(Intercept)
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:right;">
0.4788360
</td>
<td style="text-align:right;">
0.3942530
</td>
<td style="text-align:right;">
34.007122
</td>
<td style="text-align:right;">
0.0000029
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.5041413
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  site
  </td>
  <td style="text-align:right;">
  1
  </td>
  <td style="text-align:right;">
  28
  </td>
  <td style="text-align:right;">
  0.0426085
  </td>
  <td style="text-align:right;">
  0.3942530
  </td>
  <td style="text-align:right;">
  3.026073
  </td>
  <td style="text-align:right;">
  0.0929198
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0829641
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  att
  </td>
  <td style="text-align:right;">
  2
  </td>
  <td style="text-align:right;">
  56
  </td>
  <td style="text-align:right;">
  0.0349080
  </td>
  <td style="text-align:right;">
  0.0767162
  </td>
  <td style="text-align:right;">
  12.740763
  </td>
  <td style="text-align:right;">
  0.0000275
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.0690048
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    site:att
    </td>
    <td style="text-align:right;">
    2
    </td>
    <td style="text-align:right;">
    56
    </td>
    <td style="text-align:right;">
    0.0046292
    </td>
    <td style="text-align:right;">
    0.0767162
    </td>
    <td style="text-align:right;">
    1.689568
    </td>
    <td style="text-align:right;">
    0.1938726
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.0097334
    </td>
    </tr>
    </tbody>
    </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
W
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.3694011
</td>
<td style="text-align:right;">
1.4e-06
</td>
<td style="text-align:left;">

- </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  4
  </td>
  <td style="text-align:left;">
  site:att
  </td>
  <td style="text-align:right;">
  0.3694011
  </td>
  <td style="text-align:right;">
  1.4e-06
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    </tbody>
    </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
GGe
</th>
<th style="text-align:right;">
p\[GG\]
</th>
<th style="text-align:left;">
p\[GG\]\<.05
</th>
<th style="text-align:right;">
HFe
</th>
<th style="text-align:right;">
p\[HF\]
</th>
<th style="text-align:left;">
p\[HF\]\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.6132716
</td>
<td style="text-align:right;">
0.0005441
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.6269223
  </td>
  <td style="text-align:right;">
  0.0004893
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    4
    </td>
    <td style="text-align:left;">
    site:att
    </td>
    <td style="text-align:right;">
    0.6132716
    </td>
    <td style="text-align:right;">
    0.2039790
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.6269223
    </td>
    <td style="text-align:right;">
    0.2038129
    </td>
    <td style="text-align:left;">
    </td>
    </tr>
    </tbody>
    </table>

</td>
</tr>
</tbody>
</table>

## Experiment 4: Task-relevant feature visibility

``` r
d4 <- data %>% filter(expt=="4")
m_anova = ezANOVA(
  data = d4,
  dv = .(AUC),
  wid = .(subject),
  within = .(att),
  between = .(site),
  detailed = TRUE,
  )
```

    ## Warning: You have removed one or more Ss from the analysis. Refactoring
    ## "subject" for ANOVA.

``` r
knitr::kable(m_anova)
```

<table class="kable_wrapper">
<tbody>
<tr>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
DFn
</th>
<th style="text-align:right;">
DFd
</th>
<th style="text-align:right;">
SSn
</th>
<th style="text-align:right;">
SSd
</th>
<th style="text-align:right;">
F
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
<th style="text-align:right;">
ges
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
(Intercept)
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:right;">
2.1747548
</td>
<td style="text-align:right;">
0.6138876
</td>
<td style="text-align:right;">
99.192642
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7539698
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  site
  </td>
  <td style="text-align:right;">
  1
  </td>
  <td style="text-align:right;">
  28
  </td>
  <td style="text-align:right;">
  0.0322474
  </td>
  <td style="text-align:right;">
  0.6138876
  </td>
  <td style="text-align:right;">
  1.470836
  </td>
  <td style="text-align:right;">
  0.2353472
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0434661
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  att
  </td>
  <td style="text-align:right;">
  2
  </td>
  <td style="text-align:right;">
  56
  </td>
  <td style="text-align:right;">
  0.0101207
  </td>
  <td style="text-align:right;">
  0.0957633
  </td>
  <td style="text-align:right;">
  2.959163
  </td>
  <td style="text-align:right;">
  0.0600243
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0140610
  </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  site:att
  </td>
  <td style="text-align:right;">
  2
  </td>
  <td style="text-align:right;">
  56
  </td>
  <td style="text-align:right;">
  0.0094963
  </td>
  <td style="text-align:right;">
  0.0957633
  </td>
  <td style="text-align:right;">
  2.776600
  </td>
  <td style="text-align:right;">
  0.0708348
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0132049
  </td>
  </tr>
  </tbody>
  </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
W
</th>
<th style="text-align:right;">
p
</th>
<th style="text-align:left;">
p\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.2834904
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:left;">

- </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  4
  </td>
  <td style="text-align:left;">
  site:att
  </td>
  <td style="text-align:right;">
  0.2834904
  </td>
  <td style="text-align:right;">
  0
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    </tbody>
    </table>

</td>
<td>
<table>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
Effect
</th>
<th style="text-align:right;">
GGe
</th>
<th style="text-align:right;">
p\[GG\]
</th>
<th style="text-align:left;">
p\[GG\]\<.05
</th>
<th style="text-align:right;">
HFe
</th>
<th style="text-align:right;">
p\[HF\]
</th>
<th style="text-align:left;">
p\[HF\]\<.05
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
3
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.5825776
</td>
<td style="text-align:right;">
0.0895472
</td>
<td style="text-align:left;">
</td>
<td style="text-align:right;">
0.5923176
</td>
<td style="text-align:right;">
0.0887495
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
4
</td>
<td style="text-align:left;">
site:att
</td>
<td style="text-align:right;">
0.5825776
</td>
<td style="text-align:right;">
0.1002745
</td>
<td style="text-align:left;">
</td>
<td style="text-align:right;">
0.5923176
</td>
<td style="text-align:right;">
0.0995082
</td>
<td style="text-align:left;">
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
