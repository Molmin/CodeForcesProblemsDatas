## Description

<div><p>Vasya came up with his own weather forecasting method. He knows the information about the average air temperature for each of the last <span class="tex-span"><i>n</i></span> days. Assume that the average air temperature for each day is integral.</p><p>Vasya believes that if the average temperatures over the last <span class="tex-span"><i>n</i></span> days form an arithmetic progression, where the first term equals to the average temperature on the first day, the second term equals to the average temperature on the second day and so on, then the average temperature of the next <span class="tex-span">(<i>n</i> + 1)</span>-th day will be equal to the next term of the arithmetic progression. Otherwise, according to Vasya's method, the temperature of the <span class="tex-span">(<i>n</i> + 1)</span>-th day will be equal to the temperature of the <span class="tex-span"><i>n</i></span>-th day.</p><p>Your task is to help Vasya predict the average temperature for tomorrow, i. e. for the <span class="tex-span">(<i>n</i> + 1)</span>-th day.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the number of days for which the average air temperature is known.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">( - 1000 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>&nbsp;— where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the average temperature in the <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>Print the average air temperature in the <span class="tex-span">(<i>n</i> + 1)</span>-th day, which Vasya predicts according to his method. Note that the absolute value of the predicted temperature can exceed <span class="tex-span">1000</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the number of days for which the average air temperature is known.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">( - 1000 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>&nbsp;— where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the average temperature in the <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>Print the average air temperature in the <span class="tex-span">(<i>n</i> + 1)</span>-th day, which Vasya predicts according to his method. Note that the absolute value of the predicted temperature can exceed <span class="tex-span">1000</span>.</p>





```input1
5
10 5 0 -5 -10

```




```input2
4
1 1 1 1

```




```input3
3
5 1 -5

```




```input4
2
900 1000

```




```output1
-15

```




```output2
1

```




```output3
-5

```




```output4
1100

```



## Note

<p>In the first example the sequence of the average temperatures is an arithmetic progression where the first term is <span class="tex-span">10</span> and each following terms decreases by <span class="tex-span">5</span>. So the predicted average temperature for the sixth day is <span class="tex-span"> - 10 - 5 =  - 15</span>.</p><p>In the second example the sequence of the average temperatures is an arithmetic progression where the first term is <span class="tex-span">1</span> and each following terms equals to the previous one. So the predicted average temperature in the fifth day is <span class="tex-span">1</span>.</p><p>In the third example the average temperatures do not form an arithmetic progression, so the average temperature of the fourth day equals to the temperature of the third day and equals to <span class="tex-span"> - 5</span>.</p><p>In the fourth example the sequence of the average temperatures is an arithmetic progression where the first term is <span class="tex-span">900</span> and each the following terms increase by <span class="tex-span">100</span>. So predicted average temperature in the third day is <span class="tex-span">1000 + 100 = 1100</span>.</p>
