TWCF FOHO BigANOVA3
================
Karen Tian
2024-02-21

## ANOVA

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
174
</td>
<td style="text-align:right;">
6.9500680
</td>
<td style="text-align:right;">
3.0632190
</td>
<td style="text-align:right;">
394.784648
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.6631344
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
  174
  </td>
  <td style="text-align:right;">
  0.0000000
  </td>
  <td style="text-align:right;">
  3.0632190
  </td>
  <td style="text-align:right;">
  0.000000
  </td>
  <td style="text-align:right;">
  1.0000000
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0000000
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
  174
  </td>
  <td style="text-align:right;">
  0.6132600
  </td>
  <td style="text-align:right;">
  3.0632190
  </td>
  <td style="text-align:right;">
  17.417500
  </td>
  <td style="text-align:right;">
  0.0000001
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.1479937
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
    348
    </td>
    <td style="text-align:right;">
    0.0199068
    </td>
    <td style="text-align:right;">
    0.4673462
    </td>
    <td style="text-align:right;">
    7.411614
    </td>
    <td style="text-align:right;">
    0.0007044
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.0056068
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
      174
      </td>
      <td style="text-align:right;">
      0.0000000
      </td>
      <td style="text-align:right;">
      3.0632190
      </td>
      <td style="text-align:right;">
      0.000000
      </td>
      <td style="text-align:right;">
      1.0000000
      </td>
      <td style="text-align:left;">
      </td>
      <td style="text-align:right;">
      0.0000000
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
      348
      </td>
      <td style="text-align:right;">
      0.0000000
      </td>
      <td style="text-align:right;">
      0.4673462
      </td>
      <td style="text-align:right;">
      0.000000
      </td>
      <td style="text-align:right;">
      1.0000000
      </td>
      <td style="text-align:left;">
      </td>
      <td style="text-align:right;">
      0.0000000
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
      348
      </td>
      <td style="text-align:right;">
      0.0843397
      </td>
      <td style="text-align:right;">
      0.4673462
      </td>
      <td style="text-align:right;">
      15.700461
      </td>
      <td style="text-align:right;">
      0.0000000
      </td>
      <td style="text-align:left;">

      - </td>
        <td style="text-align:right;">
        0.0233311
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
        348
        </td>
        <td style="text-align:right;">
        0.0000000
        </td>
        <td style="text-align:right;">
        0.4673462
        </td>
        <td style="text-align:right;">
        0.000000
        </td>
        <td style="text-align:right;">
        1.0000000
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.0000000
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
0.5983593
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
  0.5983593
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
    0.5983593
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
      0.5983593
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
0.7134496
</td>
<td style="text-align:right;">
0.0026465
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7176882
  </td>
  <td style="text-align:right;">
  0.0025949
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
    0.7134496
    </td>
    <td style="text-align:right;">
    1.0000000
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.7176882
    </td>
    <td style="text-align:right;">
    1.0000000
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
    0.7134496
    </td>
    <td style="text-align:right;">
    0.0000000
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.7176882
      </td>
      <td style="text-align:right;">
      0.0000000
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
        0.7134496
        </td>
        <td style="text-align:right;">
        1.0000000
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.7176882
        </td>
        <td style="text-align:right;">
        1.0000000
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
