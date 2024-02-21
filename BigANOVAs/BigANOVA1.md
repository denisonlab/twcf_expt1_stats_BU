TWCF FOHO BigANOVA1
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
  between = .(site,stimulus,task),
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
230
</td>
<td style="text-align:right;">
9.7494966
</td>
<td style="text-align:right;">
3.0117232
</td>
<td style="text-align:right;">
744.5518955
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7314099
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
  230
  </td>
  <td style="text-align:right;">
  0.0000000
  </td>
  <td style="text-align:right;">
  3.0117232
  </td>
  <td style="text-align:right;">
  0.0000000
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
  stimulus
  </td>
  <td style="text-align:right;">
  1
  </td>
  <td style="text-align:right;">
  230
  </td>
  <td style="text-align:right;">
  0.3931323
  </td>
  <td style="text-align:right;">
  3.0117232
  </td>
  <td style="text-align:right;">
  30.0228201
  </td>
  <td style="text-align:right;">
  0.0000001
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.0989419
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    4
    </td>
    <td style="text-align:left;">
    task
    </td>
    <td style="text-align:right;">
    1
    </td>
    <td style="text-align:right;">
    230
    </td>
    <td style="text-align:right;">
    2.9907679
    </td>
    <td style="text-align:right;">
    3.0117232
    </td>
    <td style="text-align:right;">
    228.3996808
    </td>
    <td style="text-align:right;">
    0.0000000
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.4551464
      </td>
      </tr>
      <tr>
      <td style="text-align:left;">
      9
      </td>
      <td style="text-align:left;">
      att
      </td>
      <td style="text-align:right;">
      2
      </td>
      <td style="text-align:right;">
      460
      </td>
      <td style="text-align:right;">
      0.6048531
      </td>
      <td style="text-align:right;">
      0.5685111
      </td>
      <td style="text-align:right;">
      244.7027009
      </td>
      <td style="text-align:right;">
      0.0000000
      </td>
      <td style="text-align:left;">

      - </td>
        <td style="text-align:right;">
        0.1445258
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        5
        </td>
        <td style="text-align:left;">
        site:stimulus
        </td>
        <td style="text-align:right;">
        1
        </td>
        <td style="text-align:right;">
        230
        </td>
        <td style="text-align:right;">
        0.0000000
        </td>
        <td style="text-align:right;">
        3.0117232
        </td>
        <td style="text-align:right;">
        0.0000000
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
        site:task
        </td>
        <td style="text-align:right;">
        1
        </td>
        <td style="text-align:right;">
        230
        </td>
        <td style="text-align:right;">
        0.0000000
        </td>
        <td style="text-align:right;">
        3.0117232
        </td>
        <td style="text-align:right;">
        0.0000000
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
        stimulus:task
        </td>
        <td style="text-align:right;">
        1
        </td>
        <td style="text-align:right;">
        230
        </td>
        <td style="text-align:right;">
        0.1374290
        </td>
        <td style="text-align:right;">
        3.0117232
        </td>
        <td style="text-align:right;">
        10.4952110
        </td>
        <td style="text-align:right;">
        0.0013738
        </td>
        <td style="text-align:left;">

        - </td>
          <td style="text-align:right;">
          0.0369665
          </td>
          </tr>
          <tr>
          <td style="text-align:left;">
          10
          </td>
          <td style="text-align:left;">
          site:att
          </td>
          <td style="text-align:right;">
          2
          </td>
          <td style="text-align:right;">
          460
          </td>
          <td style="text-align:right;">
          0.0000000
          </td>
          <td style="text-align:right;">
          0.5685111
          </td>
          <td style="text-align:right;">
          0.0000000
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
          stimulus:att
          </td>
          <td style="text-align:right;">
          2
          </td>
          <td style="text-align:right;">
          460
          </td>
          <td style="text-align:right;">
          0.0017917
          </td>
          <td style="text-align:right;">
          0.5685111
          </td>
          <td style="text-align:right;">
          0.7248773
          </td>
          <td style="text-align:right;">
          0.4849365
          </td>
          <td style="text-align:left;">
          </td>
          <td style="text-align:right;">
          0.0005002
          </td>
          </tr>
          <tr>
          <td style="text-align:left;">
          12
          </td>
          <td style="text-align:left;">
          task:att
          </td>
          <td style="text-align:right;">
          2
          </td>
          <td style="text-align:right;">
          460
          </td>
          <td style="text-align:right;">
          0.0338750
          </td>
          <td style="text-align:right;">
          0.5685111
          </td>
          <td style="text-align:right;">
          13.7046600
          </td>
          <td style="text-align:right;">
          0.0000017
          </td>
          <td style="text-align:left;">

          - </td>
            <td style="text-align:right;">
            0.0093730
            </td>
            </tr>
            <tr>
            <td style="text-align:left;">
            8
            </td>
            <td style="text-align:left;">
            site:stimulus:task
            </td>
            <td style="text-align:right;">
            1
            </td>
            <td style="text-align:right;">
            230
            </td>
            <td style="text-align:right;">
            0.0000000
            </td>
            <td style="text-align:right;">
            3.0117232
            </td>
            <td style="text-align:right;">
            0.0000000
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
            13
            </td>
            <td style="text-align:left;">
            site:stimulus:att
            </td>
            <td style="text-align:right;">
            2
            </td>
            <td style="text-align:right;">
            460
            </td>
            <td style="text-align:right;">
            0.0000000
            </td>
            <td style="text-align:right;">
            0.5685111
            </td>
            <td style="text-align:right;">
            0.0000000
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
            site:task:att
            </td>
            <td style="text-align:right;">
            2
            </td>
            <td style="text-align:right;">
            460
            </td>
            <td style="text-align:right;">
            0.0000000
            </td>
            <td style="text-align:right;">
            0.5685111
            </td>
            <td style="text-align:right;">
            0.0000000
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
            stimulus:task:att
            </td>
            <td style="text-align:right;">
            2
            </td>
            <td style="text-align:right;">
            460
            </td>
            <td style="text-align:right;">
            0.0102349
            </td>
            <td style="text-align:right;">
            0.5685111
            </td>
            <td style="text-align:right;">
            4.1406927
            </td>
            <td style="text-align:right;">
            0.0165088
            </td>
            <td style="text-align:left;">

            - </td>
              <td style="text-align:right;">
              0.0028506
              </td>
              </tr>
              <tr>
              <td style="text-align:left;">
              16
              </td>
              <td style="text-align:left;">
              site:stimulus:task:att
              </td>
              <td style="text-align:right;">
              2
              </td>
              <td style="text-align:right;">
              460
              </td>
              <td style="text-align:right;">
              0.0000000
              </td>
              <td style="text-align:right;">
              0.5685111
              </td>
              <td style="text-align:right;">
              0.0000000
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
9
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.8032191
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:left;">

- </td>
  </tr>
  <tr>
  <td style="text-align:left;">
  10
  </td>
  <td style="text-align:left;">
  site:att
  </td>
  <td style="text-align:right;">
  0.8032191
  </td>
  <td style="text-align:right;">
  0
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    11
    </td>
    <td style="text-align:left;">
    stimulus:att
    </td>
    <td style="text-align:right;">
    0.8032191
    </td>
    <td style="text-align:right;">
    0
    </td>
    <td style="text-align:left;">

    - </td>
      </tr>
      <tr>
      <td style="text-align:left;">
      12
      </td>
      <td style="text-align:left;">
      task:att
      </td>
      <td style="text-align:right;">
      0.8032191
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
        site:stimulus:att
        </td>
        <td style="text-align:right;">
        0.8032191
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
          site:task:att
          </td>
          <td style="text-align:right;">
          0.8032191
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
            stimulus:task:att
            </td>
            <td style="text-align:right;">
            0.8032191
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
              site:stimulus:task:att
              </td>
              <td style="text-align:right;">
              0.8032191
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
9
</td>
<td style="text-align:left;">
att
</td>
<td style="text-align:right;">
0.8355748
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.8409703
  </td>
  <td style="text-align:right;">
  0.0000000
  </td>
  <td style="text-align:left;">

  - </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    10
    </td>
    <td style="text-align:left;">
    site:att
    </td>
    <td style="text-align:right;">
    0.8355748
    </td>
    <td style="text-align:right;">
    1.0000000
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.8409703
    </td>
    <td style="text-align:right;">
    1.0000000
    </td>
    <td style="text-align:left;">
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    11
    </td>
    <td style="text-align:left;">
    stimulus:att
    </td>
    <td style="text-align:right;">
    0.8355748
    </td>
    <td style="text-align:right;">
    0.4617995
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.8409703
    </td>
    <td style="text-align:right;">
    0.4626288
    </td>
    <td style="text-align:left;">
    </td>
    </tr>
    <tr>
    <td style="text-align:left;">
    12
    </td>
    <td style="text-align:left;">
    task:att
    </td>
    <td style="text-align:right;">
    0.8355748
    </td>
    <td style="text-align:right;">
    0.0000087
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.8409703
      </td>
      <td style="text-align:right;">
      0.0000083
      </td>
      <td style="text-align:left;">

      - </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        13
        </td>
        <td style="text-align:left;">
        site:stimulus:att
        </td>
        <td style="text-align:right;">
        0.8355748
        </td>
        <td style="text-align:right;">
        1.0000000
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.8409703
        </td>
        <td style="text-align:right;">
        1.0000000
        </td>
        <td style="text-align:left;">
        </td>
        </tr>
        <tr>
        <td style="text-align:left;">
        14
        </td>
        <td style="text-align:left;">
        site:task:att
        </td>
        <td style="text-align:right;">
        0.8355748
        </td>
        <td style="text-align:right;">
        1.0000000
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.8409703
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
        stimulus:task:att
        </td>
        <td style="text-align:right;">
        0.8355748
        </td>
        <td style="text-align:right;">
        0.0226540
        </td>
        <td style="text-align:left;">

        - </td>
          <td style="text-align:right;">
          0.8409703
          </td>
          <td style="text-align:right;">
          0.0224198
          </td>
          <td style="text-align:left;">

          - </td>
            </tr>
            <tr>
            <td style="text-align:left;">
            16
            </td>
            <td style="text-align:left;">
            site:stimulus:task:att
            </td>
            <td style="text-align:right;">
            0.8355748
            </td>
            <td style="text-align:right;">
            1.0000000
            </td>
            <td style="text-align:left;">
            </td>
            <td style="text-align:right;">
            0.8409703
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
