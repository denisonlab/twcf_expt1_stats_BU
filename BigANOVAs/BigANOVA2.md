TWCF FOHO BigANOVAs
================
Karen Tian
2024-02-21

## ANOVA

``` r
m_anova = ezANOVA(
  data = data,
  dv = .(AUC),
  wid = .(subject),
  within = .(att,AUCMeasure),
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
8.3226990
</td>
<td style="text-align:right;">
2.2001829
</td>
<td style="text-align:right;">
317.7493583
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7278910
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
  0.0491329
  </td>
  <td style="text-align:right;">
  2.2001829
  </td>
  <td style="text-align:right;">
  1.8758258
  </td>
  <td style="text-align:right;">
  0.1744597
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0155463
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
  0.4636700
  </td>
  <td style="text-align:right;">
  2.2001829
  </td>
  <td style="text-align:right;">
  8.8511450
  </td>
  <td style="text-align:right;">
  0.0003250
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.1296993
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
    0.1399608
    </td>
    <td style="text-align:right;">
    0.3261065
    </td>
    <td style="text-align:right;">
    36.0517345
    </td>
    <td style="text-align:right;">
    0.0000000
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.0430483
      </td>
      </tr>
      <tr>
      <td style="text-align:left;">
      9
      </td>
      <td style="text-align:left;">
      AUCMeasure
      </td>
      <td style="text-align:right;">
      1
      </td>
      <td style="text-align:right;">
      84
      </td>
      <td style="text-align:right;">
      0.0618073
      </td>
      <td style="text-align:right;">
      0.4910878
      </td>
      <td style="text-align:right;">
      10.5720619
      </td>
      <td style="text-align:right;">
      0.0016534
      </td>
      <td style="text-align:left;">

      - </td>
        <td style="text-align:right;">
        0.0194785
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
        0.1628814
        </td>
        <td style="text-align:right;">
        2.2001829
        </td>
        <td style="text-align:right;">
        3.1092952
        </td>
        <td style="text-align:right;">
        0.0498077
        </td>
        <td style="text-align:left;">

        - </td>
          <td style="text-align:right;">
          0.0497473
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
          0.0017033
          </td>
          <td style="text-align:right;">
          0.3261065
          </td>
          <td style="text-align:right;">
          0.4387360
          </td>
          <td style="text-align:right;">
          0.6455877
          </td>
          <td style="text-align:left;">
          </td>
          <td style="text-align:right;">
          0.0005471
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
          0.0126749
          </td>
          <td style="text-align:right;">
          0.3261065
          </td>
          <td style="text-align:right;">
          1.6324313
          </td>
          <td style="text-align:right;">
          0.1683583
          </td>
          <td style="text-align:left;">
          </td>
          <td style="text-align:right;">
          0.0040573
          </td>
          </tr>
          <tr>
          <td style="text-align:left;">
          10
          </td>
          <td style="text-align:left;">
          site:AUCMeasure
          </td>
          <td style="text-align:right;">
          1
          </td>
          <td style="text-align:right;">
          84
          </td>
          <td style="text-align:right;">
          0.0007230
          </td>
          <td style="text-align:right;">
          0.4910878
          </td>
          <td style="text-align:right;">
          0.1236642
          </td>
          <td style="text-align:right;">
          0.7259744
          </td>
          <td style="text-align:left;">
          </td>
          <td style="text-align:right;">
          0.0002323
          </td>
          </tr>
          <tr>
          <td style="text-align:left;">
          11
          </td>
          <td style="text-align:left;">
          expt:AUCMeasure
          </td>
          <td style="text-align:right;">
          2
          </td>
          <td style="text-align:right;">
          84
          </td>
          <td style="text-align:right;">
          1.2542998
          </td>
          <td style="text-align:right;">
          0.4910878
          </td>
          <td style="text-align:right;">
          107.2732686
          </td>
          <td style="text-align:right;">
          0.0000000
          </td>
          <td style="text-align:left;">

          - </td>
            <td style="text-align:right;">
            0.2873149
            </td>
            </tr>
            <tr>
            <td style="text-align:left;">
            13
            </td>
            <td style="text-align:left;">
            att:AUCMeasure
            </td>
            <td style="text-align:right;">
            2
            </td>
            <td style="text-align:right;">
            168
            </td>
            <td style="text-align:right;">
            0.0543753
            </td>
            <td style="text-align:right;">
            0.0939150
            </td>
            <td style="text-align:right;">
            48.6346765
            </td>
            <td style="text-align:right;">
            0.0000000
            </td>
            <td style="text-align:left;">

            - </td>
              <td style="text-align:right;">
              0.0171766
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
              0.0177065
              </td>
              <td style="text-align:right;">
              0.3261065
              </td>
              <td style="text-align:right;">
              2.2804605
              </td>
              <td style="text-align:right;">
              0.0627372
              </td>
              <td style="text-align:left;">
              </td>
              <td style="text-align:right;">
              0.0056588
              </td>
              </tr>
              <tr>
              <td style="text-align:left;">
              12
              </td>
              <td style="text-align:left;">
              site:expt:AUCMeasure
              </td>
              <td style="text-align:right;">
              2
              </td>
              <td style="text-align:right;">
              84
              </td>
              <td style="text-align:right;">
              0.0354106
              </td>
              <td style="text-align:right;">
              0.4910878
              </td>
              <td style="text-align:right;">
              3.0284703
              </td>
              <td style="text-align:right;">
              0.0537042
              </td>
              <td style="text-align:left;">
              </td>
              <td style="text-align:right;">
              0.0112532
              </td>
              </tr>
              <tr>
              <td style="text-align:left;">
              14
              </td>
              <td style="text-align:left;">
              site:att:AUCMeasure
              </td>
              <td style="text-align:right;">
              2
              </td>
              <td style="text-align:right;">
              168
              </td>
              <td style="text-align:right;">
              0.0011781
              </td>
              <td style="text-align:right;">
              0.0939150
              </td>
              <td style="text-align:right;">
              1.0537378
              </td>
              <td style="text-align:right;">
              0.3509248
              </td>
              <td style="text-align:left;">
              </td>
              <td style="text-align:right;">
              0.0003785
              </td>
              </tr>
              <tr>
              <td style="text-align:left;">
              15
              </td>
              <td style="text-align:left;">
              expt:att:AUCMeasure
              </td>
              <td style="text-align:right;">
              4
              </td>
              <td style="text-align:right;">
              168
              </td>
              <td style="text-align:right;">
              0.0409011
              </td>
              <td style="text-align:right;">
              0.0939150
              </td>
              <td style="text-align:right;">
              18.2915088
              </td>
              <td style="text-align:right;">
              0.0000000
              </td>
              <td style="text-align:left;">

              - </td>
                <td style="text-align:right;">
                0.0129754
                </td>
                </tr>
                <tr>
                <td style="text-align:left;">
                16
                </td>
                <td style="text-align:left;">
                site:expt:att:AUCMeasure
                </td>
                <td style="text-align:right;">
                4
                </td>
                <td style="text-align:right;">
                168
                </td>
                <td style="text-align:right;">
                0.0030445
                </td>
                <td style="text-align:right;">
                0.0939150
                </td>
                <td style="text-align:right;">
                1.3615617
                </td>
                <td style="text-align:right;">
                0.2494276
                </td>
                <td style="text-align:left;">
                </td>
                <td style="text-align:right;">
                0.0009776
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
0.7433823
</td>
<td style="text-align:right;">
4.5e-06
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
  0.7433823
  </td>
  <td style="text-align:right;">
  4.5e-06
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
    0.7433823
    </td>
    <td style="text-align:right;">
    4.5e-06
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
      0.7433823
      </td>
      <td style="text-align:right;">
      4.5e-06
      </td>
      <td style="text-align:left;">

      - </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        13
        </td>
        <td style="text-align:left;">
        att:AUCMeasure
        </td>
        <td style="text-align:right;">
        0.6733233
        </td>
        <td style="text-align:right;">
        1.0e-07
        </td>
        <td style="text-align:left;">

        - </td>
          </tr>
          <tr>
          <td style="text-align:left;">
          14
          </td>
          <td style="text-align:left;">
          site:att:AUCMeasure
          </td>
          <td style="text-align:right;">
          0.6733233
          </td>
          <td style="text-align:right;">
          1.0e-07
          </td>
          <td style="text-align:left;">

          - </td>
            </tr>
            <tr>
            <td style="text-align:left;">
            15
            </td>
            <td style="text-align:left;">
            expt:att:AUCMeasure
            </td>
            <td style="text-align:right;">
            0.6733233
            </td>
            <td style="text-align:right;">
            1.0e-07
            </td>
            <td style="text-align:left;">

            - </td>
              </tr>
              <tr>
              <td style="text-align:left;">
              16
              </td>
              <td style="text-align:left;">
              site:expt:att:AUCMeasure
              </td>
              <td style="text-align:right;">
              0.6733233
              </td>
              <td style="text-align:right;">
              1.0e-07
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
0.7957870
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.8086782
  </td>
  <td style="text-align:right;">
  0.0000000
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
    0.7957870
    </td>
    <td style="text-align:right;">
    0.6003589
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.8086782
    </td>
    <td style="text-align:right;">
    0.6035348
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
    0.7957870
    </td>
    <td style="text-align:right;">
    0.1820569
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.8086782
    </td>
    <td style="text-align:right;">
    0.1811764
    </td>
    <td style="text-align:left;">
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
    0.7957870
    </td>
    <td style="text-align:right;">
    0.0784659
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.8086782
    </td>
    <td style="text-align:right;">
    0.0773608
    </td>
    <td style="text-align:left;">
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    13
    </td>
    <td style="text-align:left;">
    att:AUCMeasure
    </td>
    <td style="text-align:right;">
    0.7537631
    </td>
    <td style="text-align:right;">
    0.0000000
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.7645530
      </td>
      <td style="text-align:right;">
      0.0000000
      </td>
      <td style="text-align:left;">

      - </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        14
        </td>
        <td style="text-align:left;">
        site:att:AUCMeasure
        </td>
        <td style="text-align:right;">
        0.7537631
        </td>
        <td style="text-align:right;">
        0.3350071
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.7645530
        </td>
        <td style="text-align:right;">
        0.3358667
        </td>
        <td style="text-align:left;">
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        15
        </td>
        <td style="text-align:left;">
        expt:att:AUCMeasure
        </td>
        <td style="text-align:right;">
        0.7537631
        </td>
        <td style="text-align:right;">
        0.0000000
        </td>
        <td style="text-align:left;">

        - </td>
          <td style="text-align:right;">
          0.7645530
          </td>
          <td style="text-align:right;">
          0.0000000
          </td>
          <td style="text-align:left;">

          - </td>
            </tr>
            <tr>
            <td style="text-align:left;">
            16
            </td>
            <td style="text-align:left;">
            site:expt:att:AUCMeasure
            </td>
            <td style="text-align:right;">
            0.7537631
            </td>
            <td style="text-align:right;">
            0.2575259
            </td>
            <td style="text-align:left;">
            </td>
            <td style="text-align:right;">
            0.7645530
            </td>
            <td style="text-align:right;">
            0.2572183
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
