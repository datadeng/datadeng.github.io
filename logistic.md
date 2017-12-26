
### 原始数据展示


```python
#### 美国入学申请的录取记录表，admit – 是否录取，1代表录取，0代表否定；gpa – gpa成绩，gre – 绩点
import pandas

admissions = pandas.read_csv('/Users/MichaelDeng/Desktop/admissions.csv')

admissions
```




<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>admit</th>
      <th>gre</th>
      <th>gpa</th>
      <th>prestige</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>380.0</td>
      <td>3.61</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>660.0</td>
      <td>3.67</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1</td>
      <td>800.0</td>
      <td>4.00</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1</td>
      <td>640.0</td>
      <td>3.19</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>0</td>
      <td>520.0</td>
      <td>2.93</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1</td>
      <td>760.0</td>
      <td>3.00</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1</td>
      <td>560.0</td>
      <td>2.98</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>7</th>
      <td>0</td>
      <td>400.0</td>
      <td>3.08</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1</td>
      <td>540.0</td>
      <td>3.39</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>9</th>
      <td>0</td>
      <td>700.0</td>
      <td>3.92</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>10</th>
      <td>0</td>
      <td>800.0</td>
      <td>4.00</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>11</th>
      <td>0</td>
      <td>440.0</td>
      <td>3.22</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1</td>
      <td>760.0</td>
      <td>4.00</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>13</th>
      <td>0</td>
      <td>700.0</td>
      <td>3.08</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1</td>
      <td>700.0</td>
      <td>4.00</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>15</th>
      <td>0</td>
      <td>480.0</td>
      <td>3.44</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>16</th>
      <td>0</td>
      <td>780.0</td>
      <td>3.87</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>17</th>
      <td>0</td>
      <td>360.0</td>
      <td>2.56</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>18</th>
      <td>0</td>
      <td>800.0</td>
      <td>3.75</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>19</th>
      <td>1</td>
      <td>540.0</td>
      <td>3.81</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>20</th>
      <td>0</td>
      <td>500.0</td>
      <td>3.17</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1</td>
      <td>660.0</td>
      <td>3.63</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>22</th>
      <td>0</td>
      <td>600.0</td>
      <td>2.82</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>23</th>
      <td>0</td>
      <td>680.0</td>
      <td>3.19</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1</td>
      <td>760.0</td>
      <td>3.35</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>25</th>
      <td>1</td>
      <td>800.0</td>
      <td>3.66</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>26</th>
      <td>1</td>
      <td>620.0</td>
      <td>3.61</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1</td>
      <td>520.0</td>
      <td>3.74</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1</td>
      <td>780.0</td>
      <td>3.22</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>29</th>
      <td>0</td>
      <td>520.0</td>
      <td>3.29</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>370</th>
      <td>1</td>
      <td>540.0</td>
      <td>3.77</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>371</th>
      <td>1</td>
      <td>680.0</td>
      <td>3.76</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>372</th>
      <td>1</td>
      <td>680.0</td>
      <td>2.42</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>373</th>
      <td>1</td>
      <td>620.0</td>
      <td>3.37</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>374</th>
      <td>0</td>
      <td>560.0</td>
      <td>3.78</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>375</th>
      <td>0</td>
      <td>560.0</td>
      <td>3.49</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>376</th>
      <td>0</td>
      <td>620.0</td>
      <td>3.63</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>377</th>
      <td>1</td>
      <td>800.0</td>
      <td>4.00</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>378</th>
      <td>0</td>
      <td>640.0</td>
      <td>3.12</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>379</th>
      <td>0</td>
      <td>540.0</td>
      <td>2.70</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>380</th>
      <td>0</td>
      <td>700.0</td>
      <td>3.65</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>381</th>
      <td>1</td>
      <td>540.0</td>
      <td>3.49</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>382</th>
      <td>0</td>
      <td>540.0</td>
      <td>3.51</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>383</th>
      <td>0</td>
      <td>660.0</td>
      <td>4.00</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>384</th>
      <td>1</td>
      <td>480.0</td>
      <td>2.62</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>385</th>
      <td>0</td>
      <td>420.0</td>
      <td>3.02</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>386</th>
      <td>1</td>
      <td>740.0</td>
      <td>3.86</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>387</th>
      <td>0</td>
      <td>580.0</td>
      <td>3.36</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>388</th>
      <td>0</td>
      <td>640.0</td>
      <td>3.17</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>389</th>
      <td>0</td>
      <td>640.0</td>
      <td>3.51</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>390</th>
      <td>1</td>
      <td>800.0</td>
      <td>3.05</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>391</th>
      <td>1</td>
      <td>660.0</td>
      <td>3.88</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>392</th>
      <td>1</td>
      <td>600.0</td>
      <td>3.38</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>393</th>
      <td>1</td>
      <td>620.0</td>
      <td>3.75</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>394</th>
      <td>1</td>
      <td>460.0</td>
      <td>3.99</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>395</th>
      <td>0</td>
      <td>620.0</td>
      <td>4.00</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>396</th>
      <td>0</td>
      <td>560.0</td>
      <td>3.04</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>397</th>
      <td>0</td>
      <td>460.0</td>
      <td>2.63</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>398</th>
      <td>0</td>
      <td>700.0</td>
      <td>3.65</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>399</th>
      <td>0</td>
      <td>600.0</td>
      <td>3.89</td>
      <td>3.0</td>
    </tr>
  </tbody>
</table>
<p>400 rows × 4 columns</p>
</div>




```python
admissions = admissions.dropna()
admissions
```




<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>admit</th>
      <th>gre</th>
      <th>gpa</th>
      <th>prestige</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>380.0</td>
      <td>3.61</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>660.0</td>
      <td>3.67</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1</td>
      <td>800.0</td>
      <td>4.00</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1</td>
      <td>640.0</td>
      <td>3.19</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>0</td>
      <td>520.0</td>
      <td>2.93</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1</td>
      <td>760.0</td>
      <td>3.00</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1</td>
      <td>560.0</td>
      <td>2.98</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>7</th>
      <td>0</td>
      <td>400.0</td>
      <td>3.08</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1</td>
      <td>540.0</td>
      <td>3.39</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>9</th>
      <td>0</td>
      <td>700.0</td>
      <td>3.92</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>10</th>
      <td>0</td>
      <td>800.0</td>
      <td>4.00</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>11</th>
      <td>0</td>
      <td>440.0</td>
      <td>3.22</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1</td>
      <td>760.0</td>
      <td>4.00</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>13</th>
      <td>0</td>
      <td>700.0</td>
      <td>3.08</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1</td>
      <td>700.0</td>
      <td>4.00</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>15</th>
      <td>0</td>
      <td>480.0</td>
      <td>3.44</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>16</th>
      <td>0</td>
      <td>780.0</td>
      <td>3.87</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>17</th>
      <td>0</td>
      <td>360.0</td>
      <td>2.56</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>18</th>
      <td>0</td>
      <td>800.0</td>
      <td>3.75</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>19</th>
      <td>1</td>
      <td>540.0</td>
      <td>3.81</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>20</th>
      <td>0</td>
      <td>500.0</td>
      <td>3.17</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1</td>
      <td>660.0</td>
      <td>3.63</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>22</th>
      <td>0</td>
      <td>600.0</td>
      <td>2.82</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>23</th>
      <td>0</td>
      <td>680.0</td>
      <td>3.19</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1</td>
      <td>760.0</td>
      <td>3.35</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>25</th>
      <td>1</td>
      <td>800.0</td>
      <td>3.66</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>26</th>
      <td>1</td>
      <td>620.0</td>
      <td>3.61</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1</td>
      <td>520.0</td>
      <td>3.74</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1</td>
      <td>780.0</td>
      <td>3.22</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>29</th>
      <td>0</td>
      <td>520.0</td>
      <td>3.29</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>370</th>
      <td>1</td>
      <td>540.0</td>
      <td>3.77</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>371</th>
      <td>1</td>
      <td>680.0</td>
      <td>3.76</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>372</th>
      <td>1</td>
      <td>680.0</td>
      <td>2.42</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>373</th>
      <td>1</td>
      <td>620.0</td>
      <td>3.37</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>374</th>
      <td>0</td>
      <td>560.0</td>
      <td>3.78</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>375</th>
      <td>0</td>
      <td>560.0</td>
      <td>3.49</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>376</th>
      <td>0</td>
      <td>620.0</td>
      <td>3.63</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>377</th>
      <td>1</td>
      <td>800.0</td>
      <td>4.00</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>378</th>
      <td>0</td>
      <td>640.0</td>
      <td>3.12</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>379</th>
      <td>0</td>
      <td>540.0</td>
      <td>2.70</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>380</th>
      <td>0</td>
      <td>700.0</td>
      <td>3.65</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>381</th>
      <td>1</td>
      <td>540.0</td>
      <td>3.49</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>382</th>
      <td>0</td>
      <td>540.0</td>
      <td>3.51</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>383</th>
      <td>0</td>
      <td>660.0</td>
      <td>4.00</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>384</th>
      <td>1</td>
      <td>480.0</td>
      <td>2.62</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>385</th>
      <td>0</td>
      <td>420.0</td>
      <td>3.02</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>386</th>
      <td>1</td>
      <td>740.0</td>
      <td>3.86</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>387</th>
      <td>0</td>
      <td>580.0</td>
      <td>3.36</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>388</th>
      <td>0</td>
      <td>640.0</td>
      <td>3.17</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>389</th>
      <td>0</td>
      <td>640.0</td>
      <td>3.51</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>390</th>
      <td>1</td>
      <td>800.0</td>
      <td>3.05</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>391</th>
      <td>1</td>
      <td>660.0</td>
      <td>3.88</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>392</th>
      <td>1</td>
      <td>600.0</td>
      <td>3.38</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>393</th>
      <td>1</td>
      <td>620.0</td>
      <td>3.75</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>394</th>
      <td>1</td>
      <td>460.0</td>
      <td>3.99</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>395</th>
      <td>0</td>
      <td>620.0</td>
      <td>4.00</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>396</th>
      <td>0</td>
      <td>560.0</td>
      <td>3.04</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>397</th>
      <td>0</td>
      <td>460.0</td>
      <td>2.63</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>398</th>
      <td>0</td>
      <td>700.0</td>
      <td>3.65</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>399</th>
      <td>0</td>
      <td>600.0</td>
      <td>3.89</td>
      <td>3.0</td>
    </tr>
  </tbody>
</table>
<p>397 rows × 4 columns</p>
</div>




```python
admissions.describe()
```




<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>admit</th>
      <th>gre</th>
      <th>gpa</th>
      <th>prestige</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>397.000000</td>
      <td>397.000000</td>
      <td>397.000000</td>
      <td>397.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>0.317380</td>
      <td>587.858942</td>
      <td>3.392242</td>
      <td>2.488665</td>
    </tr>
    <tr>
      <th>std</th>
      <td>0.466044</td>
      <td>115.717787</td>
      <td>0.380208</td>
      <td>0.947083</td>
    </tr>
    <tr>
      <th>min</th>
      <td>0.000000</td>
      <td>220.000000</td>
      <td>2.260000</td>
      <td>1.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>0.000000</td>
      <td>520.000000</td>
      <td>3.130000</td>
      <td>2.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>0.000000</td>
      <td>580.000000</td>
      <td>3.400000</td>
      <td>2.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>1.000000</td>
      <td>660.000000</td>
      <td>3.670000</td>
      <td>3.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>1.000000</td>
      <td>800.000000</td>
      <td>4.000000</td>
      <td>4.000000</td>
    </tr>
  </tbody>
</table>
</div>



### 线性回归来进行预测


```python
from sklearn.linear_model import LinearRegression

import matplotlib.pyplot as plt

model = LinearRegression()

####训练模型

model.fit(admissions[['gre', 'gpa']], admissions["admit"])

admit_prediction = model.predict(admissions[['gre', 'gpa']])

plt.xlabel('gpa')

plt.ylabel('admit_prediction')

plt.scatter(admissions["gpa"], admit_prediction)

plt.show()
```

    /Users/MichaelDeng/workspaces/env1/lib/python2.7/site-packages/scipy/linalg/basic.py:1018: RuntimeWarning: internal gelsd driver lwork query error, required iwork dimension not returned. This is likely the result of LAPACK bug 0038, fixed in LAPACK 3.2.2 (released July 21, 2010). Falling back to 'gelss' driver.
      warnings.warn(mesg, RuntimeWarning)



![png](output_5_1.png)


### logistic回归函数


```python
import numpy as np

def logit(x):
    
    return np.exp(x) / (1 + np.exp(x)) 

#### 在-6到6之间等差产生50个数

t = np.linspace(-6,6,50, dtype=float)

ylogit = logit(t)

#### 作图

plt.plot(t, ylogit, label="logistic")

plt.ylabel("Probability")

plt.xlabel("t")

plt.title("Logistic Function")

plt.show()
```


![png](output_7_0.png)


### logistic回归预测


```python
from sklearn.linear_model import LogisticRegression

#### 对数据集进行随机重排序
admissions = admissions.loc[np.random.permutation(admissions.index)]

#### 将随机排序后的前700条数据作为训练集，后面的作为测试集
num_train = 300
data_train = admissions[:num_train]
data_test = admissions[num_train:]

logistic_model = LogisticRegression()
logistic_model.fit(data_train[['gpa', 'gre']], data_train['admit'])

#### 进行测试
fitted_test = logistic_model.predict_proba(data_test[['gpa', 'gre']])[:, 1] #因为predict_proba返回的是一个两列的矩阵，矩阵的每一行代表的是对一个事件的预测结果，第一列代表该事件不会发生的概率，第二列代表的是该事件会发生的概率。而这里需要的是第二列的数据
plt.scatter(data_test['gre'], fitted_test)
plt.xlabel('gre')
plt.ylabel('probability ')
plt.show()
```


![png](output_9_0.png)


### 模型评估

#### 准确率


```python
#### predict()函数会自动把阀值设置为0.5

predicted = logistic_model.predict(data_train[['gpa','gre']])

#### 计算在训练集中正确预测的准确率

accuracy_train = (predicted == data_train['admit']).mean()

#### 计算在测试集中正确预测的准确率

predicted = logistic_model.predict(data_test[['gpa','gre']])

accuracy_test = (predicted == data_test['admit']).mean()
```


```python
accuracy_train,accuracy_test
```




    (0.69333333333333336, 0.64948453608247425)



#### ROC曲线


```python
from sklearn.metrics import roc_curve, roc_auc_score

train_probs = logistic_model.predict_proba(data_train[['gpa', 'gre']])[:,1]

test_probs = logistic_model.predict_proba(data_test[['gpa', 'gre']])[:,1]

#### 计算AUC

auc_train = roc_auc_score(data_train["admit"], train_probs)

auc_test = roc_auc_score(data_test["admit"], test_probs)

print('Auc_train: {}'.format(auc_train))

print('Auc_test: {}'.format(auc_test))

#### 计算ROC曲线

roc_train = roc_curve(data_train["admit"], train_probs)

roc_test = roc_curve(data_test["admit"], test_probs)

#### 作图

plt.plot(roc_train[0], roc_train[1])

plt.plot(roc_test[0], roc_test[1])

plt.show()
```

    Auc_train: 0.585310409699
    Auc_test: 0.642390289449



![png](output_15_1.png)



```python

```
