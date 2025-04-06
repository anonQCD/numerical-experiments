# QCD Numerical Experiments 

# Section 1 - LP, QICD, QCD

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

Table 4. Average runtime and minimum RMSE for QCD, hqreg, and conquer when autocorrelation between features are 0.9. Here, standard normal error distriution is used. QCD is slower than conquer and hqreg, but has the lowest minimum RMSE. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
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


Table 5. Average runtime and minimum RMSE for QCD, hqreg, and conquer when the error distribution is centered skewed-t and $\tau=0.3$. Here, parameters for skewed-t are degrees of freedom 2 and skewing parameter $\gamma$ 4. QCD is faster than hqreg in higher dimensions but slower than conquer, but QCD has the lowest minimum RMSE. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
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
    <td>2.56 (0.62)</td>
    <td>1.28 (0.28)</td>
    <td><b>0.24 (0.06)</b></td>
    <td><b>8.97 (2.98)</b></td>
    <td>35.53 (9.82)</td>
    <td>36.83 (9.95)</td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td>4.35 (0.70)</td>
    <td>15.00 (2.20)</td>
    <td><b>1.36 (0.27)</b></td>
    <td><b>10.3 (5.69)</b></td>
    <td>34.4 (8.76)</td>
    <td>35.7 (8.95)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td>6.62 (1.65)</td>
    <td>24.32 (4.22)</td>
    <td><b>1.70 (0.53)</b></td>
    <td><b>12.3 (5.27)</b></td>
    <td>37.0 (19.12)</td>
    <td>37.9 (19.10)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td>8.86 (1.93)</td>
    <td>29.62 (5.23)</td>
    <td><b>2.50 (0.42)</b></td>
    <td><b>11.3 (5.6)</b></td>
    <td>39.7 (18.2)</td>
    <td>40.5 (18.6)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td>11.60 (2.83)</td>
    <td>36.49 (6.27)</td>
    <td><b>3.96 (0.64)</b></td>
    <td><b>11.9 (5.12)</b></td>
    <td>35.5 (16.4)</td>
    <td>36.8 (18.03)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td>16.72 (2.15)</td>
    <td>49.97 (8.36)</td>
    <td><b>3.96 (0.64)</b></td>
    <td><b>13.0 (4.72)</b></td>
    <td>31.5 (8.42)</td>
    <td>34.0 (9.32)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td>20.67 (1.75)</td>
    <td>59.16 (14.07)</td>
    <td><b>5.43 (0.71)</b></td>
    <td><b>13.9 (5.41)</b></td>
    <td>25.2 (4.87)</td>
    <td>27.9 (5.76)</td>
  </tr>
</table>

Table 6. Average runtime and minimum RMSE for QCD, hqreg, and conquer when the error distribution is centered skewed-t and $\tau=0.5$. Here, parameters for skewed-t are degrees of freedom 2 and skewing parameter $\gamma$ 4. QCD is faster than hqreg in higher dimensions but slower than conquer, but QCD has the lowest minimum RMSE. The results are averaged over 20 different seeds and the standard deviations are reported in parentheses.
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
    <td>3.07 (1.00)</td>
    <td>1.47 (0.29)</td>
    <td><b>0.28 (0.04)</b></td>
    <td><b>4.4 (2.37)</b></td>
    <td>13.7 (6.00)</td>
    <td>13.9 (5.84)</td>
  </tr>
  <tr>
    <td>$p=300$</td>
    <td>4.54 (0.83)</td>
    <td>18.73 (2.71)</td>
    <td><b>1.26 (0.34)</b></td>
    <td><b>4.76 (3.44)</b></td>
    <td>13.48 (6.37)</td>
    <td>13.66 (6.42)</td>
  </tr>
  <tr>
    <td>$p=500$</td>
    <td>6.16 (1.10)</td>
    <td>26.00 (5.90)</td>
    <td><b>1.47 (0.27)</b></td>
    <td><b>6.23 (3.74)</b></td>
    <td>15.54 (9.82)</td>
    <td>15.41 (9.70)</td>
  </tr>
  <tr>
    <td>$p=700$</td>
    <td>7.47 (1.83)</td>
    <td>33.39 (8.38)</td>
    <td><b>1.93 (0.43)</b></td>
    <td><b>6.18 (4.05)</b></td>
    <td>19.33 (15.56)</td>
    <td>19.55 (15.75)</td>
  </tr>
  <tr>
    <td>$p=1000$</td>
    <td>9.77 (2.28)</td>
    <td>31.68 (6.04)</td>
    <td><b>2.38 (0.52)</b></td>
    <td><b>6.73 (4.55)</b></td>
    <td>18.70 (14.47)</td>
    <td>18.65 (14.37)</td>
  </tr>
  <tr>
    <td>$p=1500$</td>
    <td>13.58 (2.80)</td>
    <td>42.50 (9.67)</td>
    <td><b>3.89 (0.77)</b></td>
    <td><b>6.49 (2.66)</b></td>
    <td>17.25 (7.10)</td>
    <td>17.33 (7.07)</td>
  </tr>
  <tr>
    <td>$p=2000$</td>
    <td>17.89 (1.85)</td>
    <td>46.48 (13.75)</td>
    <td><b>4.56 (1.03)</b></td>
    <td><b>8.22 (4.52)</b></td>
    <td>13.96 (5.87)</td>
    <td>13.88 (5.78)</td>
  </tr>
</table>






