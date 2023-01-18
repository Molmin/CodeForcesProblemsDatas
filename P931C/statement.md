## Description

<div><p>Anya and Kirill are doing a physics laboratory work. In one of the tasks they have to measure some value <span class="tex-span"><i>n</i></span> times, and then compute the average value to lower the error.</p><p>Kirill has already made his measurements, and has got the following integer values: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span>. It is important that the values are close to each other, namely, the difference between the maximum value and the minimum value is <span class="tex-font-style-bf">at most <span class="tex-span">2</span></span>.</p><p>Anya does not want to make the measurements, however, she can't just copy the values from Kirill's work, because the error of each measurement is a random value, and this coincidence will be noted by the teacher. Anya wants to write such integer values <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>y</i><sub class="lower-index"><i>n</i></sub></span> in her work, that the following conditions are met:</p><ul> <li> the average value of <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> is equal to the average value of <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span>;</li><li> all Anya's measurements are in the same bounds as all Kirill's measurements, that is, the maximum value among Anya's values is not greater than the maximum value among Kirill's values, and the minimum value among Anya's values is not less than the minimum value among Kirill's values;</li><li> the number of equal measurements in Anya's work and Kirill's work is as small as possible among options with the previous conditions met. Formally, the teacher goes through all Anya's values one by one, if there is equal value in Kirill's work and it is not strike off yet, he strikes off this Anya's value and one of equal values in Kirill's work. The number of equal measurements is then the total number of <span class="tex-font-style-bf">strike off</span> values in Anya's work. </li></ul><p>Help Anya to write such a set of measurements that the conditions above are met.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the numeber of measurements made by Kirill.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 100 000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>) — the measurements made by Kirill. It is guaranteed that the difference between the maximum and minimum values among values <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> does not exceed <span class="tex-span">2</span>.</p></div><div class="output-specification"><p>In the first line print the minimum possible number of equal measurements.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> — the values Anya should write. You can print the integers in arbitrary order. Keep in mind that the minimum value among Anya's values should be not less that the minimum among Kirill's values, and the maximum among Anya's values should be not greater than the maximum among Kirill's values.</p><p>If there are multiple answers, print any of them. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the numeber of measurements made by Kirill.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 100 000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>) — the measurements made by Kirill. It is guaranteed that the difference between the maximum and minimum values among values <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> does not exceed <span class="tex-span">2</span>.</p>

## Output

<p>In the first line print the minimum possible number of equal measurements.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> — the values Anya should write. You can print the integers in arbitrary order. Keep in mind that the minimum value among Anya's values should be not less that the minimum among Kirill's values, and the maximum among Anya's values should be not greater than the maximum among Kirill's values.</p><p>If there are multiple answers, print any of them. </p>





```input1
6
-1 1 1 0 0 -1

```




```input2
3
100 100 101

```




```input3
7
-10 -9 -10 -8 -10 -9 -9

```




```output1
2
0 0 0 0 0 0 

```




```output2
3
101 100 100 

```




```output3
5
-10 -10 -9 -9 -9 -9 -9 

```



## Note

<p>In the first example Anya can write zeros as here measurements results. The average value is then equal to the average value of Kirill's values, and there are only two equal measurements.</p><p>In the second example Anya should write two values <span class="tex-span">100</span> and one value <span class="tex-span">101</span> (in any order), because it is the only possibility to make the average be the equal to the average of Kirill's values. Thus, all three measurements are equal.</p><p>In the third example the number of equal measurements is <span class="tex-span">5</span>.</p>
