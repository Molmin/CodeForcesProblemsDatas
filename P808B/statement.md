## Description

<div><p>It's been almost a week since Polycarp couldn't get rid of insomnia. And as you may already know, one week in Berland lasts <span class="tex-span"><i>k</i></span> days!</p><p>When Polycarp went to a doctor with his problem, the doctor asked him about his sleeping schedule (more specifically, the average amount of hours of sleep per week). Luckily, Polycarp kept records of sleep times for the last <span class="tex-span"><i>n</i></span> days. So now he has a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the sleep time on the <span class="tex-span"><i>i</i></span>-th day.</p><p>The number of records is so large that Polycarp is unable to calculate the average value by himself. Thus he is asking you to help him with the calculations. To get the average Polycarp is going to consider <span class="tex-span"><i>k</i></span> consecutive days as a week. So there will be <span class="tex-span"><i>n</i> - <i>k</i> + 1</span> weeks to take into consideration. For example, if <span class="tex-span"><i>k</i> = 2</span>, <span class="tex-span"><i>n</i> = 3</span> and <span class="tex-span"><i>a</i> = [3, 4, 7]</span>, then the result is <img align="middle" class="tex-formula" src="file://4NF4BKEB.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>You should write a program which will calculate average sleep times of Polycarp over all weeks.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Output average sleeping time over all weeks. </p><p>The answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. In particular, it is enough to output real number with at least 6 digits after the decimal point.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Output average sleeping time over all weeks. </p><p>The answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. In particular, it is enough to output real number with at least 6 digits after the decimal point.</p>





```input1
3 2
3 4 7

```




```input2
1 1
10

```




```input3
8 2
1 2 4 100000 123 456 789 1

```




```output1
9.0000000000

```




```output2
10.0000000000

```




```output3
28964.2857142857

```



## Note

<p>In the third example there are <span class="tex-span"><i>n</i> - <i>k</i> + 1 = 7</span> weeks, so the answer is sums of all weeks divided by 7.</p>
