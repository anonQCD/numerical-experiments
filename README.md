# QCD Numerical Experiments 

This document includes further numerical experiments results of further comparison between QCD and smoothed approaches. We use `hqreg` (Yi and Huang'17) and `conquer` (Tan et al'22, He et al'23) packages for comparison. 

## Autocorrelation
Table 1. Average runtime and minimum RMSE for QCD, hqreg, and conquer when autocorrelation between features are 0.9. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
<table>
  <tr>
    <th> Dimension ($n=300$) </th>
    <th colspan="3"> Runtime (seconds) </th>
    <th colspan="3"> minimum RMSE </th>
  </tr>
  <tr>
    <th></th>
    <th>QCD </th>
    <th>hqreg</th>
    <th>conquer</th>
    <th>QCD</th>
    <th>hqreg</th>
    <th>conquer</th>
  </tr>
 <tr>
    <td>$p=100$</td>
    <td>16.83 (1.24)</td>
    <td>0.84 (0.12)</td>
    <td><b>0.28 (0.04)</b></td>
    <td><b>3.70 (0.35)</b></td>
    <td>3.72 (0.67)</td>
    <td>4.86 (0.86)</td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td>20.47 (1.97)</td>
    <td>4.82 (0.55)</td>
    <td><b>0.62 (0.15)</b></td>
    <td><b>3.63 (0.30)</b></td>
    <td>3.97 (0.52)</td>
    <td>4.91 (0.69)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td>20.47 (1.97)</td>
    <td>4.82 (0.55)</td>
    <td><b>0.62 (0.15)</b></td>
    <td><b>3.63 (0.30)</b></td>
    <td>3.97 (0.52)</td>
    <td>4.91 (0.69)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td>42.42 (3.90)</td>
    <td>7.77 (0.73)</td>
    <td><b>1.46 (0.30)</b></td>
    <td><b>3.60 (0.51)</b></td>
    <td>4.15 (0.75)</td>
    <td>5.05 (0.92)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td>53.36 (4.42)</td>
    <td>8.46 (0.73)</td>
    <td><b>2.20 (0.48)</b></td>
    <td><b>3.70 (0.22)</b></td>
    <td>4.58 (0.70)</td>
    <td>5.30 (0.88)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td>57.96 (4.39)</td>
    <td>9.79 (1.12)</td>
    <td><b>3.62 (0.54)</b></td>
    <td><b>3.68 (0.31)</b></td>
    <td>4.37 (0.51)</td>
    <td>5.33 (0.71)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td>62.84 (4.54)</td>
    <td>10.50 (1.12)</td>
    <td><b>4.65 (0.82)</b></td>
    <td><b>3.76 (0.34)</b></td>
    <td>4.52 (0.56)</td>
    <td>5.43 (0.70)</td>
  </tr>
</table>

## Signal
Table 2. Average runtime and minimum RMSE for QCD, hqreg, and conquer when signals of non-zero true $\beta$ are 0.7. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
<table>
  <tr>
    <th> Dimension ($n=300$) </th>
    <th colspan="3"> Runtime (seconds) </th>
    <th colspan="3"> minimum RMSE </th>
  </tr>
  <tr>
    <th></th>
    <th>QCD </th>
    <th>hqreg</th>
    <th>conquer</th>
    <th>QCD</th>
    <th>hqreg</th>
    <th>conquer</th>
  </tr>
 <tr>
    <td>$p=100$</td>
    <td>9.28 (1.51)</td>
    <td>0.58 (0.09)</td>
    <td><b>0.25 (0.03)</b></td>
    <td><b>7.63 (0.80)</b></td>
    <td>12.47 (1.20)</td>
    <td>12.50 (1.17)</td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td>8.64 (1.12)</td>
    <td>4.61 (0.51)</td>
    <td><b>0.60 (0.09)</b></td>
    <td><b>7.65 (0.75)</b></td>
    <td>12.41 (1.07)</td>
    <td>12.75 (1.04)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td>12.07 (2.09)</td>
    <td>5.15 (0.53)</td>
    <td><b>1.06 (0.08)</b></td>
    <td><b>7.29 (0.66)</b></td>
    <td>12.52 (1.31)</td>
    <td>12.87 (1.29)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td>13.28 (1.71)</td>
    <td>5.03 (0.46)</td>
    <td><b>1.58 (0.10)</b></td>
    <td><b>7.54 (0.69)</b></td>
    <td>12.97 (1.05)</td>
    <td>13.28 (1.09)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td>15.55 (1.40)</td>
    <td>5.60 (0.49)</td>
    <td><b>2.26 (0.24)</b></td>
    <td><b>7.53 (0.54)</b></td>
    <td>12.64 (1.07)</td>
    <td>12.83 (1.23)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td>18.43 (1.20)</td>
    <td>6.67 (0.42)</td>
    <td><b>3.58 (0.53)</b></td>
    <td><b>7.58 (0.52)</b></td>
    <td>12.03 (1.05)</td>
    <td>13.36 (0.97)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td>22.08 (1.53)</td>
    <td>7.78 (0.57)</td>
    <td><b>5.17 (0.62)</b></td>
    <td><b>7.56 (0.98)</b></td>
    <td>12.83 (2.12)</td>
    <td>13.08 (1.37)</td>
  </tr>
</table>

Table 3. Average runtime and minimum RMSE for QCD, hqreg, and conquer when signals of non-zero true $\beta$ are 0.6. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
<table>
  <tr>
    <th> Dimension ($n=300$) </th>
    <th colspan="3"> Runtime (seconds) </th>
    <th colspan="3"> minimum RMSE </th>
  </tr>
  <tr>
    <th></th>
    <th>QCD </th>
    <th>hqreg</th>
    <th>conquer</th>
    <th>QCD</th>
    <th>hqreg</th>
    <th>conquer</th>
  </tr>
 <tr>
    <td>$p=100$</td>
    <td><b>0.14 (0.02)</b></td>
    <td>0.57 (0.08)</td>
    <td>0.25 (0.03)</td>
    <td><b>11.9 (1.99)</b></td>
    <td>21.1 (2.63)</td>
    <td>21.2 (2.55)</td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td><b>0.48 (0.08)</b></td>
    <td>4.61 (0.52)</td>
    <td>0.60 (0.09)</td>
    <td><b>11.4 (2.77)</b></td>
    <td>21.8 (2.27)</td>
    <td>21.6 (2.18)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td><b>0.95 (0.30)</b></td>
    <td>5.16 (0.54)</td>
    <td>1.06 (0.08)</td>
    <td><b>11.6 (1.73)</b></td>
    <td>21.9 (2.66)</td>
    <td>22.0 (2.61)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td><b>1.23 (0.27)</b></td>
    <td>5.09 (0.46)</td>
    <td>1.56 (0.09)</td>
    <td><b>11.7 (2.34)</b></td>
    <td>22.8 (2.00)</td>
    <td>22.7 (2.09)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td><b>1.82 (0.23)</b></td>
    <td>5.53 (0.51)</td>
    <td>2.21 (0.23)</td>
    <td><b>11.1 (2.18)</b></td>
    <td>21.9 (2.05)</td>
    <td>22.1 (2.14)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td><b>3.42 (1.47)</b></td>
    <td>6.51 (0.36)</td>
    <td>3.51 (0.53)</td>
    <td><b>12.5 (2.62)</b></td>
    <td>23.0 (2.14)</td>
    <td>22.8 (2.20)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td><b>6.19 (3.20)</b></td>
    <td>7.26 (0.87)</td>
    <td>4.44 (0.59)</td>
    <td><b>11.5 (2.50)</b></td>
    <td>22.5 (2.12)</td>
    <td>22.4 (2.24)</td>
  </tr>
</table>

Table 4. Average runtime and minimum RMSE for QCD, hqreg, and conquer when signals of non-zero true $\beta$ are 0.5. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
<table>
  <tr>
    <th> Dimension ($n=300$) </th>
    <th colspan="3"> Runtime (seconds) </th>
    <th colspan="3"> minimum RMSE </th>
  </tr>
  <tr>
    <th></th>
    <th>QCD </th>
    <th>hqreg</th>
    <th>conquer</th>
    <th>QCD</th>
    <th>hqreg</th>
    <th>conquer</th>
  </tr>
 <tr>
    <td>$p=100$</td>
    <td><b>0.14 (0.02)</b></td>
        <td>0.57 (0.08)</td>
        <td>0.25 (0.03)</td>
        <td><b>23.6 (5.69)</b></td>
        <td>38.1 (5.36)</td>
        <td>27.5 (5.17)</td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td><b>0.48 (0.07)</b></td>
        <td>4.63 (0.49)</td>
        <td>0.60 (0.09)</td>
        <td><b>23.1 (8.40)</b></td>
        <td>39.9 (5.26)</td>
        <td>39.5 (4.68)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td><b>0.90 (0.14)</b></td>
        <td>5.19 (0.51)</td>
        <td>1.06 (0.08)</td>
        <td><b>25.0 (4.34)</b></td>
        <td>39.5 (4.60)</td>
        <td>39.3 (4.65)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td><b>1.16 (0.18)</b></td>
        <td>5.11 (0.42)</td>
        <td>1.55 (0.09)</td>
        <td><b>22.5 (7.98)</b></td>
        <td>41.2 (4.99)</td>
        <td>41.0 (4.46)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td><b>1.78 (0.23)</b></td>
        <td>5.63 (0.60)</td>
        <td>2.20 (0.23)</td>
        <td><b>20.7 (6.35)</b></td>
        <td>40.4 (6.41)</td>
        <td>39.9 (6.06)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td><b>2.83 (0.23)</b></td>
        <td>6.72 (0.47)</td>
        <td>3.58 (0.54)</td>
        <td><b>24.8 (8.98)</b></td>
        <td>41.9 (4.64)</td>
        <td>41.2 (4.16)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td><b>4.20 (0.75)</b></td>
        <td>8.03 (0.83)</td>
        <td>5.02 (0.58)</td>
        <td><b>22.5 (6.28)</b></td>
        <td>41.3 (4.76)</td>
        <td>40.9 (4.21)</td>
  </tr>
</table>


