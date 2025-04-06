# QCD Numerical Experiments 

# Section 1 - LP, QICD, QCD

## Nudge hyperparameter
Table 1. minimum RMSE of QCD when different nudge standard deviation values are used. There are no difference in minimum RMSE over different hyperparameter values. Same example data in the introduction of the main paper is used ($p = 1000, n = 300$). 

<table>
  <tr>
    <td>sd</td>
    <td>minimum RMSE </td>
  </tr>
  <tr>
    <td>0.01</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>1</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>3</td>
    <td>0.01</td>
  </tr>
  <tr>
    <td>6</td>
    <td>0.008 $\approx$ 0.01</td>
  </tr>
  <tr>
    <td>10</td>
    <td>0.0095 $\approx$ 0.01</td>
  </tr>
</table>




## Sparsity
Table 2. Average runtime and minimum RMSE for LP, QICD, and QCD when 10 non-zero true $\beta$ are used. QCD is faster than LP and QICD in high dimensions, and has the similar low minimum RMSE as other two. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
<table>
  <tr>
    <th> Dimension ($n=300$) </th>
    <th colspan="3"> Runtime (seconds) </th>
    <th colspan="3"> minimum RMSE </th>
  </tr>
  <tr>
    <th></th>
    <th>LP </th>
    <th>QICD</th>
    <th>QCD</th>
    <th>LP</th>
    <th>QICD</th>
    <th>QCD</th>
  </tr>
 <tr>
    <td>$p=100$</td>
<td><b>1.85 (0.03)</b></td>
    <td>12.90 (1.53)</td>
    <td>9.69 (0.42)</td>
    <td>1.60 (0.05)</td>
    <td>1.62 (0.06)</td>
    <td><b>1.60 (0.05)</b></td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td><b>16.24 (0.83)</b></td>
    <td>21.11 (4.17)</td>
    <td>29.16 (2.59)</td>
    <td>1.66 (0.12)</td>
    <td>1.69 (0.13)</td>
    <td><b>1.65 (0.12)</b></td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td>54.87 (2.57)</td>
    <td>33.03 (8.34)</td>
    <td><b>31.68 (2.14)</b></td>
    <td>1.73 (0.12)</td>
    <td>1.76 (0.13)</td>
    <td><b>1.72 (0.11)</b></td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td>112.78 (5.61)</td>
    <td>50.21 (12.77)</td>
    <td><b>29.66 (2.21)</b></td>
    <td>1.69 (0.17)</td>
    <td>1.75 (0.19)</td>
    <td><b>1.71 (0.15)</b></td>
  </tr>
  <tr>
    <td>$p=1000$</td>
     <td>253.86 (9.19)</td>
    <td>72.39 (21.51)</td>
    <td><b>29.13 (1.93)</b></td>
    <td>1.75 (0.10)</td>
    <td>1.79 (0.12)</td>
    <td><b>1.76 (0.11)</b></td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td>677.11 (30.64)</td>
    <td>91.09 (20.02)</td>
    <td><b>30.02 (1.92)</b></td>
    <td>1.81 (0.14)</td>
    <td>1.91 (0.24)</td>
    <td><b>1.84 (0.19)</b></td>
  </tr>
  <tr>
    <td>$p=2000$</td>
<td>1446.99 (80.47)</td>
    <td>133.63 (42.33)</td>
    <td><b>31.05 (1.31)</b></td>
    <td>1.85 (0.13)</td>
    <td>1.96 (0.21)</td>
    <td><b>1.88 (0.17)</b></td>
  </tr>
</table>


## Autocorrelation

Table 3. Average runtime and minimum RMSE for LP, QICD, and QCD when autocorrelation between features are 0.9. QCD is faster than LP and QICD in high dimensions, and has the similar low minimum RMSE as other two. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
<table>
  <tr>
    <th> Dimension ($n=300$) </th>
    <th colspan="3"> Runtime (seconds) </th>
    <th colspan="3"> minimum RMSE </th>
  </tr>
  <tr>
    <th></th>
    <th>LP </th>
    <th>QICD</th>
    <th>QCD</th>
    <th>LP</th>
    <th>QICD</th>
    <th>QCD</th>
  </tr>
 <tr>
    <td>$p=100$</td>
    <td><b>2.09 (0.37)</b></td>
    <td>12.94 (2.10)</td>
    <td>14.60 (4.59)</td>
    <td>3.67 (0.31)</td>
    <td>3.92 (0.66)</td>
    <td><b>3.70 (0.35)</b></td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td><b>15.00 (1.33)</b></td>
    <td>26.98 (6.20)</td>
    <td>20.94 (2.46)</td>
    <td>3.62 (0.29)</td>
    <td>3.77 (0.37)</td>
    <td><b>3.63 (0.30)</b></td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td>53.02 (4.91)</td>
    <td>40.76 (10.13)</td>
    <td><b>32.50 (4.10)</b></td>
    <td>3.70 (0.29)</td>
    <td>4.03 (0.57)</td>
    <td><b>3.74 (0.35)</b></td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td>116.67 (10.64)</td>
    <td>50.96 (10.05)</td>
    <td><b>40.15 (5.06)</b></td>
    <td>3.62 (0.57)</td>
    <td>3.78 (0.70)</td>
    <td><b>3.60 (0.51)</b></td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td>251.80 (9.33)</td>
    <td>66.38 (17.70)</td>
    <td><b>43.25 (4.45)</b></td>
    <td>3.71 (0.23)</td>
    <td>3.88 (0.27)</td>
    <td><b>3.70 (0.22)</b></td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td>722.96 (27.33)</td>
    <td>84.58 (29.43)</td>
    <td><b>44.95 (5.09)</b></td>
    <td>3.71 (0.26)</td>
    <td>3.97 (0.55)</td>
    <td><b>3.68 (0.31)</b></td>
  </tr>
  <tr>
    <td>$p=2000$</td>
<td>1511.64 (41.57)</td>
    <td>100.96 (25.83)</td>
    <td><b>48.28 (3.96)</b></td>
    <td>3.83 (0.35)</td>
    <td>4.07 (0.51)</td>
    <td><b>3.76 (0.34)</b></td>
  </tr>
</table>






# Section 2 - QCD, hqreg, conquer

## Autocorrelation
Table 4. Average runtime and minimum RMSE for QCD, hqreg, and conquer when autocorrelation between features are 0.9. QCD is slower than conquer and hqreg, but has the lowest RMSE. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
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
    <td>4.91 (0.70)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td>33.69 (4.22)</td>
    <td>6.98 (0.88)</td>
    <td><b>1.05 (0.24)</b></td>
    <td><b>3.74 (0.35)</b></td>
    <td>4.11 (0.57)</td>
    <td>5.03 (0.76)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td>42.42 (3.90)</td>
    <td>7.77 (0.73)</td>
    <td><b>1.46 (0.30)</b></td>
    <td><b>3.70 (0.50)</b></td>
    <td>4.25 (0.84)</td>
    <td>5.19 (0.89)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td>42.42 (3.90)</td>
    <td>7.77 (0.73)</td>
    <td><b>1.46 (0.30)</b></td>
    <td><b>3.60 (0.51)</b></td>
    <td>4.15 (0.75)</td>
    <td>5.05 (0.92)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td>53.36 (4.42)</td>
    <td>8.46 (0.73)</td>
    <td><b>2.20 (0.48)</b></td>
    <td><b>3.70 (0.22)</b></td>
    <td>4.58 (0.70)</td>
    <td>5.30 (0.88)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td>57.96 (4.39)</td>
    <td>9.79 (1.12)</td>
    <td><b>3.62 (0.54)</b></td>
    <td><b>3.68 (0.31)</b></td>
    <td>4.37 (0.51)</td>
    <td>5.33 (0.71)</td>
  </tr>
</table>

## Signal
Table 5. Average runtime and minimum RMSE for QCD, hqreg, and conquer when signals of non-zero true $\beta$ are 0.7. QCD is slower than conquer and hqreg, but has the lowest RMSE. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
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

Table 6. Average runtime and minimum RMSE for QCD, hqreg, and conquer when signals of non-zero true $\beta$ are 0.6. QCD is faster than conquer and hqreg, and has the lowest RMSE. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
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

Table 7. Average runtime and minimum RMSE for QCD, hqreg, and conquer when signals of non-zero true $\beta$ are 0.5. QCD is faster than conquer and hqreg, and has the lowest RMSE. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
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
    <td><b>35.0 (21.50)</b></td>
    <td>43.7 (7.72)</td>
    <td>42.2 (6.69)</td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td><b>0.48 (0.07)</b></td>
    <td>4.63 (0.49)</td>
    <td>0.60 (0.09)</td>
    <td><b>32.5 (21.55)</b></td>
    <td>46.0 (5.98)</td>
    <td>43.7 (5.22)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td><b>0.90 (0.14)</b></td>
    <td>5.19 (0.51)</td>
    <td>1.06 (0.08)</td>
    <td><b>39.5 (12.15)</b></td>
    <td>45.9 (8.46)</td>
    <td>43.9 (7.61)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td><b>1.16 (0.18)</b></td>
    <td>5.11 (0.42)</td>
    <td>1.55 (0.09)</td>
    <td><b>29.2 (19.23)</b></td>
    <td>48.0 (6.87)</td>
    <td>45.4 (5.63)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td><b>1.78 (0.23)</b></td>
    <td>5.63 (0.60)</td>
    <td>2.20 (0.23)</td>
    <td><b>26.1 (15.27)</b></td>
    <td>45.7 (6.62)</td>
    <td>43.4 (5.93)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td><b>2.83 (0.23)</b></td>
    <td>6.72 (0.47)</td>
    <td>3.58 (0.54)</td>
    <td><b>33.4 (17.82)</b></td>
    <td>47.6 (6.55)</td>
    <td>44.9 (5.79)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td><b>4.20 (0.75)</b></td>
    <td>8.03 (0.83)</td>
    <td>5.02 (0.58)</td>
    <td><b>28.1 (13.71)</b></td>
    <td>47.5 (6.95)</td>
    <td>44.8 (5.48)</td>
  </tr>
</table>

## Error distribution

Table 8. Average runtime and minimum RMSE for QCD, hqreg, and conquer when the error distribution is skewed-t with degrees of freedom 2 and skewing parameter $\gamma$ 4. QCD is faster than hqreg in higher dimensions but slower than conquer, but QCD has the lowest RMSE. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
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
    <td>4.44 (2.04)</td>
    <td>1.35 (0.08)</td>
    <td><b>0.24 (0.06)</b></td>
    <td><b>4.57 (1.30)</b></td>
    <td>14.85 (7.24)</td>
    <td>15.24 (7.02)</td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td>4.34 (0.88)</td>
    <td>15.18 (1.99)</td>
    <td><b>1.03 (0.29)</b></td>
    <td><b>5.15 (1.49)</b></td>
    <td>15.39 (5.13)</td>
    <td>15.79 (4.97)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td>5.49 (0.87)</td>
    <td>23.66 (4.77)</td>
    <td><b>1.45 (0.40)</b></td>
    <td><b>5.97 (2.86)</b></td>
    <td>14.92 (6.05)</td>
    <td>15.43 (6.07)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td>7.25 (1.70)</td>
    <td>30.39 (7.36)</td>
    <td><b>1.78 (0.30)</b></td>
    <td><b>5.28 (1.21)</b></td>
    <td>13.44 (4.66)</td>
    <td>13.93 (4.68)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td>9.12 (1.74)</td>
    <td>39.20 (9.14)</td>
    <td><b>2.73 (0.43)</b></td>
    <td><b>6.23 (1.80)</b></td>
    <td>13.30 (3.49)</td>
    <td>13.81 (3.62)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td>11.68 (1.97)</td>
    <td>54.62 (15.66)</td>
    <td><b>3.98 (0.65)</b></td>
    <td><b>6.66 (2.36)</b></td>
    <td>14.39 (4.13)</td>
    <td>14.75 (4.12)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td>14.29 (2.44)</td>
    <td>64.83 (15.72)</td>
    <td><b>5.29 (0.92)</b></td>
    <td><b>6.68 (2.43)</b></td>
    <td>14.53 (4.99)</td>
    <td>15.07 (5.07)</td>
  </tr>
</table>






