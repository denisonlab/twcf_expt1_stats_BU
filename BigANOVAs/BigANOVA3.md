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
