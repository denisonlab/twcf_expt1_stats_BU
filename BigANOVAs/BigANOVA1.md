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
111
</td>
<td style="text-align:right;">
4.8747483
</td>
<td style="text-align:right;">
1.336936
</td>
<td style="text-align:right;">
404.7293755
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.7515843
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
  111
  </td>
  <td style="text-align:right;">
  0.0205653
  </td>
  <td style="text-align:right;">
  1.336936
  </td>
  <td style="text-align:right;">
  1.7074462
  </td>
  <td style="text-align:right;">
  0.1940179
  </td>
  <td style="text-align:left;">
  </td>
  <td style="text-align:right;">
  0.0126030
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
  111
  </td>
  <td style="text-align:right;">
  0.1963186
  </td>
  <td style="text-align:right;">
  1.336936
  </td>
  <td style="text-align:right;">
  16.2994891
  </td>
  <td style="text-align:right;">
  0.0000998
  </td>
  <td style="text-align:left;">

  - </td>
    <td style="text-align:right;">
    0.1086113
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
    111
    </td>
    <td style="text-align:right;">
    1.4932472
    </td>
    <td style="text-align:right;">
    1.336936
    </td>
    <td style="text-align:right;">
    123.9778906
    </td>
    <td style="text-align:right;">
    0.0000000
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.4810002
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
      222
      </td>
      <td style="text-align:right;">
      0.3024265
      </td>
      <td style="text-align:right;">
      0.274280
      </td>
      <td style="text-align:right;">
      122.3908087
      </td>
      <td style="text-align:right;">
      0.0000000
      </td>
      <td style="text-align:left;">

      - </td>
        <td style="text-align:right;">
        0.1580372
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
        111
        </td>
        <td style="text-align:right;">
        0.0526898
        </td>
        <td style="text-align:right;">
        1.336936
        </td>
        <td style="text-align:right;">
        4.3746034
        </td>
        <td style="text-align:right;">
        0.0387595
        </td>
        <td style="text-align:left;">

        - </td>
          <td style="text-align:right;">
          0.0316663
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
          111
          </td>
          <td style="text-align:right;">
          0.0123321
          </td>
          <td style="text-align:right;">
          1.336936
          </td>
          <td style="text-align:right;">
          1.0238782
          </td>
          <td style="text-align:right;">
          0.3138015
          </td>
          <td style="text-align:left;">
          </td>
          <td style="text-align:right;">
          0.0075958
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
          111
          </td>
          <td style="text-align:right;">
          0.0677974
          </td>
          <td style="text-align:right;">
          1.336936
          </td>
          <td style="text-align:right;">
          5.6289232
          </td>
          <td style="text-align:right;">
          0.0193869
          </td>
          <td style="text-align:left;">

          - </td>
            <td style="text-align:right;">
            0.0403793
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
            222
            </td>
            <td style="text-align:right;">
            0.0022628
            </td>
            <td style="text-align:right;">
            0.274280
            </td>
            <td style="text-align:right;">
            0.9157503
            </td>
            <td style="text-align:right;">
            0.4017226
            </td>
            <td style="text-align:left;">
            </td>
            <td style="text-align:right;">
            0.0014024
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
            222
            </td>
            <td style="text-align:right;">
            0.0008848
            </td>
            <td style="text-align:right;">
            0.274280
            </td>
            <td style="text-align:right;">
            0.3580753
            </td>
            <td style="text-align:right;">
            0.6994234
            </td>
            <td style="text-align:left;">
            </td>
            <td style="text-align:right;">
            0.0005488
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
            222
            </td>
            <td style="text-align:right;">
            0.0169413
            </td>
            <td style="text-align:right;">
            0.274280
            </td>
            <td style="text-align:right;">
            6.8560629
            </td>
            <td style="text-align:right;">
            0.0012906
            </td>
            <td style="text-align:left;">

            - </td>
              <td style="text-align:right;">
              0.0104052
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
              111
              </td>
              <td style="text-align:right;">
              0.0837813
              </td>
              <td style="text-align:right;">
              1.336936
              </td>
              <td style="text-align:right;">
              6.9559982
              </td>
              <td style="text-align:right;">
              0.0095521
              </td>
              <td style="text-align:left;">

              - </td>
                <td style="text-align:right;">
                0.0494286
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
                222
                </td>
                <td style="text-align:right;">
                0.0009288
                </td>
                <td style="text-align:right;">
                0.274280
                </td>
                <td style="text-align:right;">
                0.3758846
                </td>
                <td style="text-align:right;">
                0.6871178
                </td>
                <td style="text-align:left;">
                </td>
                <td style="text-align:right;">
                0.0005761
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
                222
                </td>
                <td style="text-align:right;">
                0.0004820
                </td>
                <td style="text-align:right;">
                0.274280
                </td>
                <td style="text-align:right;">
                0.1950753
                </td>
                <td style="text-align:right;">
                0.8229136
                </td>
                <td style="text-align:left;">
                </td>
                <td style="text-align:right;">
                0.0002991
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
                222
                </td>
                <td style="text-align:right;">
                0.0050848
                </td>
                <td style="text-align:right;">
                0.274280
                </td>
                <td style="text-align:right;">
                2.0578028
                </td>
                <td style="text-align:right;">
                0.1301639
                </td>
                <td style="text-align:left;">
                </td>
                <td style="text-align:right;">
                0.0031460
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
                222
                </td>
                <td style="text-align:right;">
                0.0062968
                </td>
                <td style="text-align:right;">
                0.274280
                </td>
                <td style="text-align:right;">
                2.5482716
                </td>
                <td style="text-align:right;">
                0.0805030
                </td>
                <td style="text-align:left;">
                </td>
                <td style="text-align:right;">
                0.0038929
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
0.804531
</td>
<td style="text-align:right;">
6.4e-06
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
  0.804531
  </td>
  <td style="text-align:right;">
  6.4e-06
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
    0.804531
    </td>
    <td style="text-align:right;">
    6.4e-06
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
      0.804531
      </td>
      <td style="text-align:right;">
      6.4e-06
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
        0.804531
        </td>
        <td style="text-align:right;">
        6.4e-06
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
          0.804531
          </td>
          <td style="text-align:right;">
          6.4e-06
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
            0.804531
            </td>
            <td style="text-align:right;">
            6.4e-06
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
              0.804531
              </td>
              <td style="text-align:right;">
              6.4e-06
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
0.8364918
</td>
<td style="text-align:right;">
0.0000000
</td>
<td style="text-align:left;">

- </td>
  <td style="text-align:right;">
  0.8477967
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
    0.8364918
    </td>
    <td style="text-align:right;">
    0.3868468
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.8477967
    </td>
    <td style="text-align:right;">
    0.3879857
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
    0.8364918
    </td>
    <td style="text-align:right;">
    0.6612616
    </td>
    <td style="text-align:left;">
    </td>
    <td style="text-align:right;">
    0.8477967
    </td>
    <td style="text-align:right;">
    0.6641437
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
    0.8364918
    </td>
    <td style="text-align:right;">
    0.0025186
    </td>
    <td style="text-align:left;">

    - </td>
      <td style="text-align:right;">
      0.8477967
      </td>
      <td style="text-align:right;">
      0.0024046
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
        0.8364918
        </td>
        <td style="text-align:right;">
        0.6494862
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.8477967
        </td>
        <td style="text-align:right;">
        0.6523239
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
        0.8364918
        </td>
        <td style="text-align:right;">
        0.7836361
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.8477967
        </td>
        <td style="text-align:right;">
        0.7866804
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
        0.8364918
        </td>
        <td style="text-align:right;">
        0.1387632
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.8477967
        </td>
        <td style="text-align:right;">
        0.1381708
        </td>
        <td style="text-align:left;">
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
        0.8364918
        </td>
        <td style="text-align:right;">
        0.0905779
        </td>
        <td style="text-align:left;">
        </td>
        <td style="text-align:right;">
        0.8477967
        </td>
        <td style="text-align:right;">
        0.0898508
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
