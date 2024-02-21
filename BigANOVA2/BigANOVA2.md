TWCF FOHO BigANOVA2
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
```

    ## Warning: The column supplied as the wid variable contains non-unique values
    ## across levels of the supplied between-Ss variables. Automatically fixing this
    ## by generating unique wid labels.

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
16.6453981
</td>
<td style="text-align:right;">
4.8243944
</td>
<td style="text-align:right;">
600.344631
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7109911
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
  4.8243944
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
  0.9273399
  </td>
  <td style="text-align:right;">
  4.8243944
  </td>
  <td style="text-align:right;">
  16.723047
  </td>
  <td style="text-align:right;">
  0.0000002
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.1205357
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
    0.2799216
    </td>
    <td style="text-align:right;">
    0.6910326
    </td>
    <td style="text-align:right;">
    70.483438
    </td>
    <td style="text-align:right;">
    0.0000000
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.0397274
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
      174
      </td>
      <td style="text-align:right;">
      0.1236145
      </td>
      <td style="text-align:right;">
      1.0544427
      </td>
      <td style="text-align:right;">
      20.398386
      </td>
      <td style="text-align:right;">
      0.0000116
      </td>
      <td style="text-align:left;">

      - </td>
        <td style="text-align:right;">
        0.0179418
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
        4.8243944
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
        0.6910326
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
        0.0253498
        </td>
        <td style="text-align:right;">
        0.6910326
        </td>
        <td style="text-align:right;">
        3.191507
        </td>
        <td style="text-align:right;">
        0.0135603
        </td>
        <td style="text-align:left;">

        - </td>
          <td style="text-align:right;">
          0.0037326
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
          174
          </td>
          <td style="text-align:right;">
          0.0000000
          </td>
          <td style="text-align:right;">
          1.0544427
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
          11
          </td>
          <td style="text-align:left;">
          expt:AUCMeasure
          </td>
          <td style="text-align:right;">
          2
          </td>
          <td style="text-align:right;">
          174
          </td>
          <td style="text-align:right;">
          2.5085996
          </td>
          <td style="text-align:right;">
          1.0544427
          </td>
          <td style="text-align:right;">
          206.979636
          </td>
          <td style="text-align:right;">
          0.0000000
          </td>
          <td style="text-align:left;">

          - </td>
            <td style="text-align:right;">
            0.2704764
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
            348
            </td>
            <td style="text-align:right;">
            0.1087506
            </td>
            <td style="text-align:right;">
            0.1962752
            </td>
            <td style="text-align:right;">
            96.408479
            </td>
            <td style="text-align:right;">
            0.0000000
            </td>
            <td style="text-align:left;">

            - </td>
              <td style="text-align:right;">
              0.0158185
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
              0.6910326
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
              12
              </td>
              <td style="text-align:left;">
              site:expt:AUCMeasure
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
              1.0544427
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
              14
              </td>
              <td style="text-align:left;">
              site:att:AUCMeasure
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
              0.1962752
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
              15
              </td>
              <td style="text-align:left;">
              expt:att:AUCMeasure
              </td>
              <td style="text-align:right;">
              4
              </td>
              <td style="text-align:right;">
              348
              </td>
              <td style="text-align:right;">
              0.0818022
              </td>
              <td style="text-align:right;">
              0.1962752
              </td>
              <td style="text-align:right;">
              36.259243
              </td>
              <td style="text-align:right;">
              0.0000000
              </td>
              <td style="text-align:left;">

              - </td>
                <td style="text-align:right;">
                0.0119455
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
                348
                </td>
                <td style="text-align:right;">
                0.0000000
                </td>
                <td style="text-align:right;">
                0.1962752
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
0.7442367
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
  0.7442367
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
    0.7442367
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
      0.7442367
      </td>
      <td style="text-align:right;">
      0
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
        0.6609935
        </td>
        <td style="text-align:right;">
        0
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
          0.6609935
          </td>
          <td style="text-align:right;">
          0
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
            0.6609935
            </td>
            <td style="text-align:right;">
            0
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
              0.6609935
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
0.7963284
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.8025034
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
    0.7963284
    </td>
    <td style="text-align:right;">
    1.0000000
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.8025034
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
    0.7963284
    </td>
    <td style="text-align:right;">
    0.0217111
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.8025034
      </td>
      <td style="text-align:right;">
      0.0214014
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
        0.7963284
        </td>
        <td style="text-align:right;">
        1.0000000
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.8025034
        </td>
        <td style="text-align:right;">
        1.0000000
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
        0.7468223
        </td>
        <td style="text-align:right;">
        0.0000000
        </td>
        <td style="text-align:left;">

        - </td>
          <td style="text-align:right;">
          0.7518210
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
            0.7468223
            </td>
            <td style="text-align:right;">
            1.0000000
            </td>
            <td style="text-align:left;">
            </td>
            <td style="text-align:right;">
            0.7518210
            </td>
            <td style="text-align:right;">
            1.0000000
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
            0.7468223
            </td>
            <td style="text-align:right;">
            0.0000000
            </td>
            <td style="text-align:left;">

            - </td>
              <td style="text-align:right;">
              0.7518210
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
                0.7468223
                </td>
                <td style="text-align:right;">
                1.0000000
                </td>
                <td style="text-align:left;">
                </td>
                <td style="text-align:right;">
                0.7518210
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
