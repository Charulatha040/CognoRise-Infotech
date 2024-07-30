```python
import pandas as pd


file_path = 'cereals.csv'

# Read the CSV file with the correct parameters
dataset = pd.read_csv('cereals.csv', encoding='ISO-8859-1', on_bad_lines='skip')
pd.set_option('display.max_rows',None)

# Display the first few rows of the dataframe
dataset

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>mfr</th>
      <th>type</th>
      <th>calories</th>
      <th>protein</th>
      <th>fat</th>
      <th>sodium</th>
      <th>fiber</th>
      <th>carbo</th>
      <th>sugars</th>
      <th>potass</th>
      <th>vitamins</th>
      <th>shelf</th>
      <th>weight</th>
      <th>cups</th>
      <th>rating</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>N</td>
      <td>C</td>
      <td>70</td>
      <td>4</td>
      <td>1</td>
      <td>130</td>
      <td>10.0</td>
      <td>5.0</td>
      <td>6</td>
      <td>280</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.33</td>
      <td>68.402973</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>Q</td>
      <td>C</td>
      <td>120</td>
      <td>3</td>
      <td>5</td>
      <td>15</td>
      <td>2.0</td>
      <td>8.0</td>
      <td>8</td>
      <td>135</td>
      <td>0</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>33.983679</td>
    </tr>
    <tr>
      <th>2</th>
      <td>All-Bran</td>
      <td>K</td>
      <td>C</td>
      <td>70</td>
      <td>4</td>
      <td>1</td>
      <td>260</td>
      <td>9.0</td>
      <td>7.0</td>
      <td>5</td>
      <td>320</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.33</td>
      <td>59.425505</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>K</td>
      <td>C</td>
      <td>50</td>
      <td>4</td>
      <td>0</td>
      <td>140</td>
      <td>14.0</td>
      <td>8.0</td>
      <td>0</td>
      <td>330</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.50</td>
      <td>93.704912</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>R</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>2</td>
      <td>200</td>
      <td>1.0</td>
      <td>14.0</td>
      <td>8</td>
      <td>-1</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>34.384843</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>2</td>
      <td>180</td>
      <td>1.5</td>
      <td>10.5</td>
      <td>10</td>
      <td>70</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>29.509541</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>0</td>
      <td>125</td>
      <td>1.0</td>
      <td>11.0</td>
      <td>14</td>
      <td>30</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>33.174094</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>G</td>
      <td>C</td>
      <td>130</td>
      <td>3</td>
      <td>2</td>
      <td>210</td>
      <td>2.0</td>
      <td>18.0</td>
      <td>8</td>
      <td>100</td>
      <td>25</td>
      <td>3</td>
      <td>1.33</td>
      <td>0.75</td>
      <td>37.038562</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>R</td>
      <td>C</td>
      <td>90</td>
      <td>2</td>
      <td>1</td>
      <td>200</td>
      <td>4.0</td>
      <td>15.0</td>
      <td>6</td>
      <td>125</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.67</td>
      <td>49.120253</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>P</td>
      <td>C</td>
      <td>90</td>
      <td>3</td>
      <td>0</td>
      <td>210</td>
      <td>5.0</td>
      <td>13.0</td>
      <td>5</td>
      <td>190</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.67</td>
      <td>53.313813</td>
    </tr>
    <tr>
      <th>10</th>
      <td>Cap'n'Crunch</td>
      <td>Q</td>
      <td>C</td>
      <td>120</td>
      <td>1</td>
      <td>2</td>
      <td>220</td>
      <td>0.0</td>
      <td>12.0</td>
      <td>12</td>
      <td>35</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>18.042851</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Cheerios</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>6</td>
      <td>2</td>
      <td>290</td>
      <td>2.0</td>
      <td>17.0</td>
      <td>1</td>
      <td>105</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.25</td>
      <td>50.764999</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Cinnamon Toast Crunch</td>
      <td>G</td>
      <td>C</td>
      <td>120</td>
      <td>1</td>
      <td>3</td>
      <td>210</td>
      <td>0.0</td>
      <td>13.0</td>
      <td>9</td>
      <td>45</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>19.823573</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Clusters</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>3</td>
      <td>2</td>
      <td>140</td>
      <td>2.0</td>
      <td>13.0</td>
      <td>7</td>
      <td>105</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.50</td>
      <td>40.400208</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Cocoa Puffs</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>1</td>
      <td>180</td>
      <td>0.0</td>
      <td>12.0</td>
      <td>13</td>
      <td>55</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>22.736446</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Corn Chex</td>
      <td>R</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>0</td>
      <td>280</td>
      <td>0.0</td>
      <td>22.0</td>
      <td>3</td>
      <td>25</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>41.445019</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Corn Flakes</td>
      <td>K</td>
      <td>C</td>
      <td>100</td>
      <td>2</td>
      <td>0</td>
      <td>290</td>
      <td>1.0</td>
      <td>21.0</td>
      <td>2</td>
      <td>35</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>45.863324</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Corn Pops</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>0</td>
      <td>90</td>
      <td>1.0</td>
      <td>13.0</td>
      <td>12</td>
      <td>20</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>35.782791</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Count Chocula</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>1</td>
      <td>180</td>
      <td>0.0</td>
      <td>12.0</td>
      <td>13</td>
      <td>65</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>22.396513</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Cracklin' Oat Bran</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>3</td>
      <td>3</td>
      <td>140</td>
      <td>4.0</td>
      <td>10.0</td>
      <td>7</td>
      <td>160</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.50</td>
      <td>40.448772</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Cream of Wheat (Quick)</td>
      <td>N</td>
      <td>H</td>
      <td>100</td>
      <td>3</td>
      <td>0</td>
      <td>80</td>
      <td>1.0</td>
      <td>21.0</td>
      <td>0</td>
      <td>-1</td>
      <td>0</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>64.533816</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Crispix</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>0</td>
      <td>220</td>
      <td>1.0</td>
      <td>21.0</td>
      <td>3</td>
      <td>30</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>46.895644</td>
    </tr>
    <tr>
      <th>22</th>
      <td>Crispy Wheat &amp; Raisins</td>
      <td>G</td>
      <td>C</td>
      <td>100</td>
      <td>2</td>
      <td>1</td>
      <td>140</td>
      <td>2.0</td>
      <td>11.0</td>
      <td>10</td>
      <td>120</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>36.176196</td>
    </tr>
    <tr>
      <th>23</th>
      <td>Double Chex</td>
      <td>R</td>
      <td>C</td>
      <td>100</td>
      <td>2</td>
      <td>0</td>
      <td>190</td>
      <td>1.0</td>
      <td>18.0</td>
      <td>5</td>
      <td>80</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>44.330856</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Froot Loops</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>1</td>
      <td>125</td>
      <td>1.0</td>
      <td>11.0</td>
      <td>13</td>
      <td>30</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>32.207582</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Frosted Flakes</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>0</td>
      <td>200</td>
      <td>1.0</td>
      <td>14.0</td>
      <td>11</td>
      <td>25</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>31.435973</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Frosted Mini-Wheats</td>
      <td>K</td>
      <td>C</td>
      <td>100</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>3.0</td>
      <td>14.0</td>
      <td>7</td>
      <td>100</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>0.80</td>
      <td>58.345141</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Fruit &amp; Fibre Dates; Walnuts; and Oats</td>
      <td>P</td>
      <td>C</td>
      <td>120</td>
      <td>3</td>
      <td>2</td>
      <td>160</td>
      <td>5.0</td>
      <td>12.0</td>
      <td>10</td>
      <td>200</td>
      <td>25</td>
      <td>3</td>
      <td>1.25</td>
      <td>0.67</td>
      <td>40.917047</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Fruitful Bran</td>
      <td>K</td>
      <td>C</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>240</td>
      <td>5.0</td>
      <td>14.0</td>
      <td>12</td>
      <td>190</td>
      <td>25</td>
      <td>3</td>
      <td>1.33</td>
      <td>0.67</td>
      <td>41.015492</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Fruity Pebbles</td>
      <td>P</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>1</td>
      <td>135</td>
      <td>0.0</td>
      <td>13.0</td>
      <td>12</td>
      <td>25</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>28.025765</td>
    </tr>
    <tr>
      <th>30</th>
      <td>Golden Crisp</td>
      <td>P</td>
      <td>C</td>
      <td>100</td>
      <td>2</td>
      <td>0</td>
      <td>45</td>
      <td>0.0</td>
      <td>11.0</td>
      <td>15</td>
      <td>40</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.88</td>
      <td>35.252444</td>
    </tr>
    <tr>
      <th>31</th>
      <td>Golden Grahams</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>1</td>
      <td>280</td>
      <td>0.0</td>
      <td>15.0</td>
      <td>9</td>
      <td>45</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>23.804043</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Grape Nuts Flakes</td>
      <td>P</td>
      <td>C</td>
      <td>100</td>
      <td>3</td>
      <td>1</td>
      <td>140</td>
      <td>3.0</td>
      <td>15.0</td>
      <td>5</td>
      <td>85</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.88</td>
      <td>52.076897</td>
    </tr>
    <tr>
      <th>33</th>
      <td>Grape-Nuts</td>
      <td>P</td>
      <td>C</td>
      <td>110</td>
      <td>3</td>
      <td>0</td>
      <td>170</td>
      <td>3.0</td>
      <td>17.0</td>
      <td>3</td>
      <td>90</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.25</td>
      <td>53.371007</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Great Grains Pecan</td>
      <td>P</td>
      <td>C</td>
      <td>120</td>
      <td>3</td>
      <td>3</td>
      <td>75</td>
      <td>3.0</td>
      <td>13.0</td>
      <td>4</td>
      <td>100</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.33</td>
      <td>45.811716</td>
    </tr>
    <tr>
      <th>35</th>
      <td>Honey Graham Ohs</td>
      <td>Q</td>
      <td>C</td>
      <td>120</td>
      <td>1</td>
      <td>2</td>
      <td>220</td>
      <td>1.0</td>
      <td>12.0</td>
      <td>11</td>
      <td>45</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>21.871292</td>
    </tr>
    <tr>
      <th>36</th>
      <td>Honey Nut Cheerios</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>3</td>
      <td>1</td>
      <td>250</td>
      <td>1.5</td>
      <td>11.5</td>
      <td>10</td>
      <td>90</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>31.072217</td>
    </tr>
    <tr>
      <th>37</th>
      <td>Honey-comb</td>
      <td>P</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>0</td>
      <td>180</td>
      <td>0.0</td>
      <td>14.0</td>
      <td>11</td>
      <td>35</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.33</td>
      <td>28.742414</td>
    </tr>
    <tr>
      <th>38</th>
      <td>Just Right Crunchy  Nuggets</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>1</td>
      <td>170</td>
      <td>1.0</td>
      <td>17.0</td>
      <td>6</td>
      <td>60</td>
      <td>100</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>36.523683</td>
    </tr>
    <tr>
      <th>39</th>
      <td>Just Right Fruit &amp; Nut</td>
      <td>K</td>
      <td>C</td>
      <td>140</td>
      <td>3</td>
      <td>1</td>
      <td>170</td>
      <td>2.0</td>
      <td>20.0</td>
      <td>9</td>
      <td>95</td>
      <td>100</td>
      <td>3</td>
      <td>1.30</td>
      <td>0.75</td>
      <td>36.471512</td>
    </tr>
    <tr>
      <th>40</th>
      <td>Kix</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>1</td>
      <td>260</td>
      <td>0.0</td>
      <td>21.0</td>
      <td>3</td>
      <td>40</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.50</td>
      <td>39.241114</td>
    </tr>
    <tr>
      <th>41</th>
      <td>Life</td>
      <td>Q</td>
      <td>C</td>
      <td>100</td>
      <td>4</td>
      <td>2</td>
      <td>150</td>
      <td>2.0</td>
      <td>12.0</td>
      <td>6</td>
      <td>95</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>0.67</td>
      <td>45.328074</td>
    </tr>
    <tr>
      <th>42</th>
      <td>Lucky Charms</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>1</td>
      <td>180</td>
      <td>0.0</td>
      <td>12.0</td>
      <td>12</td>
      <td>55</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>26.734515</td>
    </tr>
    <tr>
      <th>43</th>
      <td>Maypo</td>
      <td>A</td>
      <td>H</td>
      <td>100</td>
      <td>4</td>
      <td>1</td>
      <td>0</td>
      <td>0.0</td>
      <td>16.0</td>
      <td>3</td>
      <td>95</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>54.850917</td>
    </tr>
    <tr>
      <th>44</th>
      <td>Muesli Raisins; Dates; &amp; Almonds</td>
      <td>R</td>
      <td>C</td>
      <td>150</td>
      <td>4</td>
      <td>3</td>
      <td>95</td>
      <td>3.0</td>
      <td>16.0</td>
      <td>11</td>
      <td>170</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>37.136863</td>
    </tr>
    <tr>
      <th>45</th>
      <td>Muesli Raisins; Peaches; &amp; Pecans</td>
      <td>R</td>
      <td>C</td>
      <td>150</td>
      <td>4</td>
      <td>3</td>
      <td>150</td>
      <td>3.0</td>
      <td>16.0</td>
      <td>11</td>
      <td>170</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>34.139765</td>
    </tr>
    <tr>
      <th>46</th>
      <td>Mueslix Crispy Blend</td>
      <td>K</td>
      <td>C</td>
      <td>160</td>
      <td>3</td>
      <td>2</td>
      <td>150</td>
      <td>3.0</td>
      <td>17.0</td>
      <td>13</td>
      <td>160</td>
      <td>25</td>
      <td>3</td>
      <td>1.50</td>
      <td>0.67</td>
      <td>30.313351</td>
    </tr>
    <tr>
      <th>47</th>
      <td>Multi-Grain Cheerios</td>
      <td>G</td>
      <td>C</td>
      <td>100</td>
      <td>2</td>
      <td>1</td>
      <td>220</td>
      <td>2.0</td>
      <td>15.0</td>
      <td>6</td>
      <td>90</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>40.105965</td>
    </tr>
    <tr>
      <th>48</th>
      <td>Nut&amp;Honey Crunch</td>
      <td>K</td>
      <td>C</td>
      <td>120</td>
      <td>2</td>
      <td>1</td>
      <td>190</td>
      <td>0.0</td>
      <td>15.0</td>
      <td>9</td>
      <td>40</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>0.67</td>
      <td>29.924285</td>
    </tr>
    <tr>
      <th>49</th>
      <td>Nutri-Grain Almond-Raisin</td>
      <td>K</td>
      <td>C</td>
      <td>140</td>
      <td>3</td>
      <td>2</td>
      <td>220</td>
      <td>3.0</td>
      <td>21.0</td>
      <td>7</td>
      <td>130</td>
      <td>25</td>
      <td>3</td>
      <td>1.33</td>
      <td>0.67</td>
      <td>40.692320</td>
    </tr>
    <tr>
      <th>50</th>
      <td>Nutri-grain Wheat</td>
      <td>K</td>
      <td>C</td>
      <td>90</td>
      <td>3</td>
      <td>0</td>
      <td>170</td>
      <td>3.0</td>
      <td>18.0</td>
      <td>2</td>
      <td>90</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>59.642837</td>
    </tr>
    <tr>
      <th>51</th>
      <td>Oatmeal Raisin Crisp</td>
      <td>G</td>
      <td>C</td>
      <td>130</td>
      <td>3</td>
      <td>2</td>
      <td>170</td>
      <td>1.5</td>
      <td>13.5</td>
      <td>10</td>
      <td>120</td>
      <td>25</td>
      <td>3</td>
      <td>1.25</td>
      <td>0.50</td>
      <td>30.450843</td>
    </tr>
    <tr>
      <th>52</th>
      <td>Post Nat. Raisin Bran</td>
      <td>P</td>
      <td>C</td>
      <td>120</td>
      <td>3</td>
      <td>1</td>
      <td>200</td>
      <td>6.0</td>
      <td>11.0</td>
      <td>14</td>
      <td>260</td>
      <td>25</td>
      <td>3</td>
      <td>1.33</td>
      <td>0.67</td>
      <td>37.840594</td>
    </tr>
    <tr>
      <th>53</th>
      <td>Product 19</td>
      <td>K</td>
      <td>C</td>
      <td>100</td>
      <td>3</td>
      <td>0</td>
      <td>320</td>
      <td>1.0</td>
      <td>20.0</td>
      <td>3</td>
      <td>45</td>
      <td>100</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>41.503540</td>
    </tr>
    <tr>
      <th>54</th>
      <td>Puffed Rice</td>
      <td>Q</td>
      <td>C</td>
      <td>50</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>0.0</td>
      <td>13.0</td>
      <td>0</td>
      <td>15</td>
      <td>0</td>
      <td>3</td>
      <td>0.50</td>
      <td>1.00</td>
      <td>60.756112</td>
    </tr>
    <tr>
      <th>55</th>
      <td>Puffed Wheat</td>
      <td>Q</td>
      <td>C</td>
      <td>50</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>1.0</td>
      <td>10.0</td>
      <td>0</td>
      <td>50</td>
      <td>0</td>
      <td>3</td>
      <td>0.50</td>
      <td>1.00</td>
      <td>63.005645</td>
    </tr>
    <tr>
      <th>56</th>
      <td>Quaker Oat Squares</td>
      <td>Q</td>
      <td>C</td>
      <td>100</td>
      <td>4</td>
      <td>1</td>
      <td>135</td>
      <td>2.0</td>
      <td>14.0</td>
      <td>6</td>
      <td>110</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.50</td>
      <td>49.511874</td>
    </tr>
    <tr>
      <th>57</th>
      <td>Quaker Oatmeal</td>
      <td>Q</td>
      <td>H</td>
      <td>100</td>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>2.7</td>
      <td>-1.0</td>
      <td>-1</td>
      <td>110</td>
      <td>0</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.67</td>
      <td>50.828392</td>
    </tr>
    <tr>
      <th>58</th>
      <td>Raisin Bran</td>
      <td>K</td>
      <td>C</td>
      <td>120</td>
      <td>3</td>
      <td>1</td>
      <td>210</td>
      <td>5.0</td>
      <td>14.0</td>
      <td>12</td>
      <td>240</td>
      <td>25</td>
      <td>2</td>
      <td>1.33</td>
      <td>0.75</td>
      <td>39.259197</td>
    </tr>
    <tr>
      <th>59</th>
      <td>Raisin Nut Bran</td>
      <td>G</td>
      <td>C</td>
      <td>100</td>
      <td>3</td>
      <td>2</td>
      <td>140</td>
      <td>2.5</td>
      <td>10.5</td>
      <td>8</td>
      <td>140</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.50</td>
      <td>39.703400</td>
    </tr>
    <tr>
      <th>60</th>
      <td>Raisin Squares</td>
      <td>K</td>
      <td>C</td>
      <td>90</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>2.0</td>
      <td>15.0</td>
      <td>6</td>
      <td>110</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.50</td>
      <td>55.333142</td>
    </tr>
    <tr>
      <th>61</th>
      <td>Rice Chex</td>
      <td>R</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>0</td>
      <td>240</td>
      <td>0.0</td>
      <td>23.0</td>
      <td>2</td>
      <td>30</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.13</td>
      <td>41.998933</td>
    </tr>
    <tr>
      <th>62</th>
      <td>Rice Krispies</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>0</td>
      <td>290</td>
      <td>0.0</td>
      <td>22.0</td>
      <td>3</td>
      <td>35</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>40.560159</td>
    </tr>
    <tr>
      <th>63</th>
      <td>Shredded Wheat</td>
      <td>N</td>
      <td>C</td>
      <td>80</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>3.0</td>
      <td>16.0</td>
      <td>0</td>
      <td>95</td>
      <td>0</td>
      <td>1</td>
      <td>0.83</td>
      <td>1.00</td>
      <td>68.235885</td>
    </tr>
    <tr>
      <th>64</th>
      <td>Shredded Wheat 'n'Bran</td>
      <td>N</td>
      <td>C</td>
      <td>90</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>4.0</td>
      <td>19.0</td>
      <td>0</td>
      <td>140</td>
      <td>0</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.67</td>
      <td>74.472949</td>
    </tr>
    <tr>
      <th>65</th>
      <td>Shredded Wheat spoon size</td>
      <td>N</td>
      <td>C</td>
      <td>90</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>3.0</td>
      <td>20.0</td>
      <td>0</td>
      <td>120</td>
      <td>0</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.67</td>
      <td>72.801787</td>
    </tr>
    <tr>
      <th>66</th>
      <td>Smacks</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>1</td>
      <td>70</td>
      <td>1.0</td>
      <td>9.0</td>
      <td>15</td>
      <td>40</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>31.230054</td>
    </tr>
    <tr>
      <th>67</th>
      <td>Special K</td>
      <td>K</td>
      <td>C</td>
      <td>110</td>
      <td>6</td>
      <td>0</td>
      <td>230</td>
      <td>1.0</td>
      <td>16.0</td>
      <td>3</td>
      <td>55</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>53.131324</td>
    </tr>
    <tr>
      <th>68</th>
      <td>Strawberry Fruit Wheats</td>
      <td>N</td>
      <td>C</td>
      <td>90</td>
      <td>2</td>
      <td>0</td>
      <td>15</td>
      <td>3.0</td>
      <td>15.0</td>
      <td>5</td>
      <td>90</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>59.363993</td>
    </tr>
    <tr>
      <th>69</th>
      <td>Total Corn Flakes</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>1</td>
      <td>200</td>
      <td>0.0</td>
      <td>21.0</td>
      <td>3</td>
      <td>35</td>
      <td>100</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>38.839746</td>
    </tr>
    <tr>
      <th>70</th>
      <td>Total Raisin Bran</td>
      <td>G</td>
      <td>C</td>
      <td>140</td>
      <td>3</td>
      <td>1</td>
      <td>190</td>
      <td>4.0</td>
      <td>15.0</td>
      <td>14</td>
      <td>230</td>
      <td>100</td>
      <td>3</td>
      <td>1.50</td>
      <td>1.00</td>
      <td>28.592785</td>
    </tr>
    <tr>
      <th>71</th>
      <td>Total Whole Grain</td>
      <td>G</td>
      <td>C</td>
      <td>100</td>
      <td>3</td>
      <td>1</td>
      <td>200</td>
      <td>3.0</td>
      <td>16.0</td>
      <td>3</td>
      <td>110</td>
      <td>100</td>
      <td>3</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>46.658844</td>
    </tr>
    <tr>
      <th>72</th>
      <td>Triples</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>1</td>
      <td>250</td>
      <td>0.0</td>
      <td>21.0</td>
      <td>3</td>
      <td>60</td>
      <td>25</td>
      <td>3</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>39.106174</td>
    </tr>
    <tr>
      <th>73</th>
      <td>Trix</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>1</td>
      <td>1</td>
      <td>140</td>
      <td>0.0</td>
      <td>13.0</td>
      <td>12</td>
      <td>25</td>
      <td>25</td>
      <td>2</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>27.753301</td>
    </tr>
    <tr>
      <th>74</th>
      <td>Wheat Chex</td>
      <td>R</td>
      <td>C</td>
      <td>100</td>
      <td>3</td>
      <td>1</td>
      <td>230</td>
      <td>3.0</td>
      <td>17.0</td>
      <td>3</td>
      <td>115</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.67</td>
      <td>49.787445</td>
    </tr>
    <tr>
      <th>75</th>
      <td>Wheaties</td>
      <td>G</td>
      <td>C</td>
      <td>100</td>
      <td>3</td>
      <td>1</td>
      <td>200</td>
      <td>3.0</td>
      <td>17.0</td>
      <td>3</td>
      <td>110</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>1.00</td>
      <td>51.592193</td>
    </tr>
    <tr>
      <th>76</th>
      <td>Wheaties Honey Gold</td>
      <td>G</td>
      <td>C</td>
      <td>110</td>
      <td>2</td>
      <td>1</td>
      <td>200</td>
      <td>1.0</td>
      <td>16.0</td>
      <td>8</td>
      <td>60</td>
      <td>25</td>
      <td>1</td>
      <td>1.00</td>
      <td>0.75</td>
      <td>36.187559</td>
    </tr>
  </tbody>
</table>
</div>




```python
print(dataset['name'])
```

    0                                  100% Bran
    1                          100% Natural Bran
    2                                   All-Bran
    3                  All-Bran with Extra Fiber
    4                             Almond Delight
    5                    Apple Cinnamon Cheerios
    6                                Apple Jacks
    7                                    Basic 4
    8                                  Bran Chex
    9                                Bran Flakes
    10                              Cap'n'Crunch
    11                                  Cheerios
    12                     Cinnamon Toast Crunch
    13                                  Clusters
    14                               Cocoa Puffs
    15                                 Corn Chex
    16                               Corn Flakes
    17                                 Corn Pops
    18                             Count Chocula
    19                        Cracklin' Oat Bran
    20                    Cream of Wheat (Quick)
    21                                   Crispix
    22                    Crispy Wheat & Raisins
    23                               Double Chex
    24                               Froot Loops
    25                            Frosted Flakes
    26                       Frosted Mini-Wheats
    27    Fruit & Fibre Dates; Walnuts; and Oats
    28                             Fruitful Bran
    29                            Fruity Pebbles
    30                              Golden Crisp
    31                            Golden Grahams
    32                         Grape Nuts Flakes
    33                                Grape-Nuts
    34                        Great Grains Pecan
    35                          Honey Graham Ohs
    36                        Honey Nut Cheerios
    37                                Honey-comb
    38               Just Right Crunchy  Nuggets
    39                    Just Right Fruit & Nut
    40                                       Kix
    41                                      Life
    42                              Lucky Charms
    43                                     Maypo
    44          Muesli Raisins; Dates; & Almonds
    45         Muesli Raisins; Peaches; & Pecans
    46                      Mueslix Crispy Blend
    47                      Multi-Grain Cheerios
    48                          Nut&Honey Crunch
    49                 Nutri-Grain Almond-Raisin
    50                         Nutri-grain Wheat
    51                      Oatmeal Raisin Crisp
    52                     Post Nat. Raisin Bran
    53                                Product 19
    54                               Puffed Rice
    55                              Puffed Wheat
    56                        Quaker Oat Squares
    57                            Quaker Oatmeal
    58                               Raisin Bran
    59                           Raisin Nut Bran
    60                            Raisin Squares
    61                                 Rice Chex
    62                             Rice Krispies
    63                            Shredded Wheat
    64                    Shredded Wheat 'n'Bran
    65                 Shredded Wheat spoon size
    66                                    Smacks
    67                                 Special K
    68                   Strawberry Fruit Wheats
    69                         Total Corn Flakes
    70                         Total Raisin Bran
    71                         Total Whole Grain
    72                                   Triples
    73                                      Trix
    74                                Wheat Chex
    75                                  Wheaties
    76                       Wheaties Honey Gold
    Name: name, dtype: object
    


```python
mfr_counts=dataset['mfr'].value_counts()
print(mfr_counts)
```

    mfr
    K    23
    G    22
    P     9
    R     8
    Q     8
    N     6
    A     1
    Name: count, dtype: int64
    


```python
max_protein_row = dataset.loc[dataset['protein'].idxmax()]        #Finding the maximum amount of protein 

product_with_max_protein = max_protein_row['name']

max_protein_value = max_protein_row['protein']

print(f"The product with the most protein is: {product_with_max_protein} with {max_protein_value} grams of protein.")

```

    The product with the most protein is: Cheerios with 6 grams of protein.
    


```python
max_fat_row = dataset.loc[dataset['fat'].idxmax()]            #Finding the maximum amount of fat

product_with_max_fat = max_fat_row['name']

max_fat_value = max_fat_row['fat']

print(f"The product with the most fat is: {product_with_max_fat} with {max_fat_value} grams of fat.")
```

    The product with the most fat is: 100% Natural Bran with 5 grams of fat.
    


```python
max_calories_row = dataset.loc[dataset['calories'].idxmax()]            #Finding the maximum amount of calories

product_with_max_calories = max_fat_row['name']

max_calories_value = max_calories_row['calories']

print(f"The product with the most calories is: {product_with_max_calories} with {max_calories_value} grams of calories.")
```

    The product with the most calories is: 100% Natural Bran with 160 grams of calories.
    


```python
max_sodium_row = dataset.loc[dataset['sodium'].idxmax()]            #Finding the maximum amount of  sodium

product_with_max_sodium = max_sodium_row['name']

max_sodium_value = max_sodium_row['sodium']

print(f"The product with the most sodium is: {product_with_max_sodium} with {max_sodium_value} grams of sodium.")
```

    The product with the most sodium is: Product 19 with 320 grams of sodium.
    


```python
max_fiber_row = dataset.loc[dataset['fiber'].idxmax()]            #Finding the maximum amount of fiber

product_with_max_fiber = max_fiber_row['name']

max_fiber_value = max_sodium_row['fiber']

print(f"The product with the most fiber is: {product_with_max_fiber} with {max_fiber_value} grams of fiber.")
```

    The product with the most fiber is: All-Bran with Extra Fiber with 1.0 grams of fiber.
    


```python
max_sugars_row = dataset.loc[dataset['sugars'].idxmax()]            #Finding the maximum amount of sugars

product_with_max_sugars = max_sugars_row['name']

max_sugars_value = max_sugars_row['sugars']

print(f"The product with the most sugars is: {product_with_max_sugars} with {max_sugars_value} grams of sugars.")
```

    The product with the most sugars is: Golden Crisp with 15 grams of sugars.
    


```python
max_carbo_row = dataset.loc[dataset['carbo'].idxmax()]            #Finding the maximum amount of carbohydrate

product_with_max_carbo = max_carbo_row['name']

max_carbo_value = max_carbo_row['carbo']

print(f"The product with the most carbo is: {product_with_max_carbo} with {max_carbo_value} grams of carbo.")
```

    The product with the most carbo is: Rice Chex with 23.0 grams of carbo.
    


```python
max_potass_row = dataset.loc[dataset['potass'].idxmax()]            #Finding the maximum amount of potassium

product_with_max_potass = max_potass_row['name']

max_potass_value = max_potass_row['potass']

print(f"The product with the most carbo is: {product_with_max_carbo} with {max_carbo_value} grams of carbo.")
```

    The product with the most carbo is: Rice Chex with 23.0 grams of carbo.
    


```python
max_vitamins_row = dataset.loc[dataset['vitamins'].idxmax()]            #Finding the maximum amount of vitamins

product_with_max_vitamins = max_vitamins_row['name']

max_vitamins_value = max_vitamins_row['carbo']

print(f"The product with the most vitamins is: {product_with_max_vitamins} with {max_vitamins_value} grams of vitamins.")
```

    The product with the most vitamins is: Just Right Crunchy  Nuggets with 17.0 grams of vitamins.
    


```python
max_vitamins_name = dataset.loc[dataset['vitamins'].idxmax()]

print("\nCereal with the highest vitamins content:\n", max_vitamins_name)
```

    
    Cereal with the highest vitamins content:
     name        Just Right Crunchy  Nuggets
    mfr                                   K
    type                                  C
    calories                            110
    protein                               2
    fat                                   1
    sodium                              170
    fiber                               1.0
    carbo                              17.0
    sugars                                6
    potass                               60
    vitamins                            100
    shelf                                 3
    weight                              1.0
    cups                                1.0
    rating                        36.523683
    Name: 38, dtype: object
    


```python

import matplotlib.pyplot as plt
import pandas as pd


file_path = 'cereals.csv'

# Read the CSV file with the correct parameters
datasets = pd.read_csv('cereals.csv', encoding='ISO-8859-1', on_bad_lines='skip')
pd.set_option('display.max_rows',None)

# Display the first few rows of the dataframe
datasets

# Find the cereal with the maximum vitamin content


# Plot the vitamin content
plt.figure(figsize=(15, 8))
plt.bar(datasets['name'], datasets['vitamins'], color='skyblue')
plt.xlabel('Cereal')
plt.ylabel('Vitamin Content')
plt.title('Vitamin Content in Cereals')
plt.xticks(rotation=90)  # Rotate cereal names for better readability
plt.grid(axis='y', linestyle='--', alpha=0.7)

plt.show()
```


    
![png](output_13_0.png)
    



```python

```


```python
max_calories_name = dataset.loc[dataset['calories'].idxmax()]

print("\nCereal with the highest calories content:\n", max_calories_name)
```

    
    Cereal with the highest calories content:
     name        Mueslix Crispy Blend
    mfr                            K
    type                           C
    calories                     160
    protein                        3
    fat                            2
    sodium                       150
    fiber                        3.0
    carbo                       17.0
    sugars                        13
    potass                       160
    vitamins                      25
    shelf                          3
    weight                       1.5
    cups                        0.67
    rating                 30.313351
    Name: 46, dtype: object
    


```python

import matplotlib.pyplot as plt
import pandas as pd


file_path = 'cereals.csv'

# Read the CSV file with the correct parameters
datasets = pd.read_csv('cereals.csv', encoding='ISO-8859-1', on_bad_lines='skip')
pd.set_option('display.max_rows',None)

# Display the first few rows of the dataframe
datasets

# Find the cereal with the maximum vitamin content


# Plot the vitamin content
plt.figure(figsize=(15, 18))
plt.barh(datasets['name'], datasets['potass'], color='darkblue')
plt.xlabel('Cereal')
plt.ylabel('potass Content')
plt.title('potass Content in Cereals')
plt.xticks(rotation=90)  # Rotate cereal names for better readability
plt.grid(axis='y', linestyle='--', alpha=0.7)

plt.show()
```


    
![png](output_16_0.png)
    



```python

```


```python
max_potass_name = dataset.loc[dataset['potass'].idxmax()]

print("\nCereal with the highest Potassium content:\n", max_potass_name)
```

    
    Cereal with the highest Potassium content:
     name        All-Bran with Extra Fiber
    mfr                                 K
    type                                C
    calories                           50
    protein                             4
    fat                                 0
    sodium                            140
    fiber                            14.0
    carbo                             8.0
    sugars                              0
    potass                            330
    vitamins                           25
    shelf                               3
    weight                            1.0
    cups                              0.5
    rating                      93.704912
    Name: 3, dtype: object
    


```python
plt.figure(figsize=(15, 8))
plt.scatter(datasets['name'], datasets['fat'], color='brown')
plt.xlabel('Cereal')
plt.ylabel('fat Content')
plt.title('fat Content in Cereals')
plt.xticks(rotation=90)  # Rotate cereal names for better readability
plt.grid(axis='y', linestyle='--', alpha=0.7)

plt.show()
```


```python
max_sugars_name = dataset.loc[dataset['sugars'].idxmax()]

print("\nCereal with the highest sugars content:\n", max_sugars_name)
```

    
    Cereal with the highest sugars content:
     name        Golden Crisp
    mfr                    P
    type                   C
    calories             100
    protein                2
    fat                    0
    sodium                45
    fiber                0.0
    carbo               11.0
    sugars                15
    potass                40
    vitamins              25
    shelf                  1
    weight               1.0
    cups                0.88
    rating         35.252444
    Name: 30, dtype: object
    


```python
plt.figure(figsize=(15, 10))
plt.bar(datasets['name'], datasets['sugars'], color='orange')
plt.xlabel('Cereal')
plt.ylabel('protein Content')
plt.title('protein Content in Cereals')
plt.xticks(rotation=90)  # Rotate cereal names for better readability
plt.grid(axis='y', linestyle='--', alpha=0.7)

plt.show()
```


    
![png](output_21_0.png)
    



```python
max_fat_name = dataset.loc[dataset['vitamins'].idxmax()]

print("\nCereal with the highest fat content:\n", max_fat_name)
```


```python
plt.figure(figsize=(15, 18))
plt.barh(datasets['name'], datasets['sugars'], color='red')
plt.xlabel('Cereal')
plt.ylabel('sugars Content')
plt.title('sugars Content in Cereals')
plt.xticks(rotation=90)  # Rotate cereal names for better readability
plt.grid(axis='y', linestyle='--', alpha=0.7)

plt.show()
```


    
![png](output_23_0.png)
    



```python
max_fiber_name = dataset.loc[dataset['fiber'].idxmax()]

print("\nCereal with the highest fiber content:\n", max_fiber_name)
```

    
    Cereal with the highest fiber content:
     name        All-Bran with Extra Fiber
    mfr                                 K
    type                                C
    calories                           50
    protein                             4
    fat                                 0
    sodium                            140
    fiber                            14.0
    carbo                             8.0
    sugars                              0
    potass                            330
    vitamins                           25
    shelf                               3
    weight                            1.0
    cups                              0.5
    rating                      93.704912
    Name: 3, dtype: object
    


```python
plt.figure(figsize=(15, 8))
plt.plot(datasets['name'], datasets['fiber'], color='black')
plt.xlabel('Cereal')
plt.ylabel('fiber Content')
plt.title('fiber Content in Cereals')
plt.xticks(rotation=90)  # Rotate cereal names for better readability
plt.grid(axis='y', linestyle='--', alpha=0.7)

plt.show()
```


    
![png](output_25_0.png)
    



```python
max_protein_name = dataset.loc[dataset['protein'].idxmax()]

print("\nCereal with the highest protein content:\n", max_protein_name)
```

    
    Cereal with the highest protein content:
     name         Cheerios
    mfr                 G
    type                C
    calories          110
    protein             6
    fat                 2
    sodium            290
    fiber             2.0
    carbo            17.0
    sugars              1
    potass            105
    vitamins           25
    shelf               1
    weight            1.0
    cups             1.25
    rating      50.764999
    Name: 11, dtype: object
    


```python
import pandas as pd
import matplotlib.pyplot as plt

# Load the cereals data from a CSV file
data = pd.read_csv('cereals.csv')

# Calculate the average rating for each brand
average_ratings = data.groupby('mfr')['rating'].mean()

# Plot the pie chart
plt.figure(figsize=(10, 7))
plt.pie(average_ratings, labels=average_ratings.index, autopct='%1.1f%%', startangle=140)
plt.title('Cereal Brands by Average Rating')
plt.axis('equal')  # Equal aspect ratio ensures that pie is drawn as a circle.
plt.show()

```


    
![png](output_27_0.png)
    



```python

```


```python
min_sugars_row = datasets.loc[datasets['sugars'].idxmin()]            #Finding the minimum amount of sugars

product_with_min_sugars = min_sugars_row['name']

min_sugars_value = min_sugars_row['sugars']

print(f"The product with the min sugars is: {product_with_min_sugars} with {min_sugars_value} grams of sugars.")
```

    The product with the min sugars is: Quaker Oatmeal with -1 grams of sugars.
    


```python
min_carbo_row = datasets.loc[datasets['carbo'].idxmin()]            #Finding the maximum amount of sugars

product_with_min_carbo = min_carbo_row['name']

min_carbo_value = min_carbo_row['carbo']

print(f"The product with the min carbo is: {product_with_min_carbo} with {min_carbo_value} grams of carbo.")
```

    The product with the min carbo is: Quaker Oatmeal with -1.0 grams of carbo.
    


```python
min_fat_row = datasets.loc[datasets['fat'].idxmin()]            #Finding the maximum amount of sugars

product_with_min_fat = min_fat_row['name']

min_fat_value = min_fat_row['fat']

print(f"The product with the least fat is: {product_with_min_fat} with {min_fat_value} grams of fat.")
```

    The product with the least fat is: All-Bran with Extra Fiber with 0 grams of fat.
    


```python
min_potass_row = datasets.loc[datasets['potass'].idxmin()]            #Finding the maximum amount of sugars

product_with_min_potass = min_potass_row['name']

min_potass_value = min_potass_row['potass']

print(f"The product with the least potass is: {product_with_min_potass} with {min_potass_value} grams of potass.")
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[15], line 1
    ----> 1 min_potass_row = datasets.loc[datasets['potass'].idxmin()]            #Finding the maximum amount of sugars
          3 product_with_min_potass = min_potass_row['name']
          5 min_potass_value = min_potass_row['potass']
    

    NameError: name 'datasets' is not defined



```python

```
