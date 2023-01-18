## Description

<div><p>To confuse the opponents, the Galactic Empire represents fractions in an unusual format. The fractions are represented as two sets of integers. The product of numbers from the first set gives the fraction numerator, the product of numbers from the second set gives the fraction denominator. However, it turned out that the programs that work with fractions in this representations aren't complete, they lack supporting the operation of reducing fractions. Implement this operation and the Empire won't forget you.</p></div><div class="input-specification"><p>The first input line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) that show how many numbers the first set (the numerator) and the second set (the denominator) contain, correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the numbers that are multiplied to produce the numerator.</p><p>The third line contains <span class="tex-span"><i>m</i></span> space-separated integers: <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the numbers that are multiplied to produce the denominator.</p></div><div class="output-specification"><p>Print the answer to the problem in the form, similar to the form of the input data. The number of values in the sets you print <span class="tex-span"><i>n</i><sub class="lower-index"><i>out</i></sub>, <i>m</i><sub class="lower-index"><i>out</i></sub></span> must satisfy the inequality <span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>out</i></sub>, <i>m</i><sub class="lower-index"><i>out</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, and the actual values in the sets <span class="tex-span"><i>a</i><sub class="lower-index"><i>out</i>, <i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>out</i>, <i>i</i></sub></span> must satisfy the inequality <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>out</i>, <i>i</i></sub>, <i>b</i><sub class="lower-index"><i>out</i>, <i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>. </p><p>Separate the values in the lines by spaces. The printed fraction must be reduced, that is, there mustn't be such integer <span class="tex-span"><i>x</i></span> (<span class="tex-span"><i>x</i> &gt; 1</span>), that the numerator and the denominator of the printed fraction are divisible by <span class="tex-span"><i>x</i></span>. If there are several matching answers, print any of them.</p></div>

## Input

<p>The first input line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) that show how many numbers the first set (the numerator) and the second set (the denominator) contain, correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the numbers that are multiplied to produce the numerator.</p><p>The third line contains <span class="tex-span"><i>m</i></span> space-separated integers: <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the numbers that are multiplied to produce the denominator.</p>

## Output

<p>Print the answer to the problem in the form, similar to the form of the input data. The number of values in the sets you print <span class="tex-span"><i>n</i><sub class="lower-index"><i>out</i></sub>, <i>m</i><sub class="lower-index"><i>out</i></sub></span> must satisfy the inequality <span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>out</i></sub>, <i>m</i><sub class="lower-index"><i>out</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, and the actual values in the sets <span class="tex-span"><i>a</i><sub class="lower-index"><i>out</i>, <i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>out</i>, <i>i</i></sub></span> must satisfy the inequality <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>out</i>, <i>i</i></sub>, <i>b</i><sub class="lower-index"><i>out</i>, <i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>. </p><p>Separate the values in the lines by spaces. The printed fraction must be reduced, that is, there mustn't be such integer <span class="tex-span"><i>x</i></span> (<span class="tex-span"><i>x</i> &gt; 1</span>), that the numerator and the denominator of the printed fraction are divisible by <span class="tex-span"><i>x</i></span>. If there are several matching answers, print any of them.</p>





```input1
3 2
100 5 2
50 10

```




```input2
4 3
2 5 10 20
100 1 3

```




```output1
2 3
2 1
1 1 1

```




```output2
1 1
20
3

```



## Note

<p>In the first test sample the numerator equals 1000, the denominator equals 500. If we reduce fraction 1000/500 by the greatest common divisor of the numerator and the denominator (by 500), we obtain fraction 2/1.</p><p>In the second test sample the numerator equals 2000, the denominator equals 300. If we reduce fraction 2000/300 by the greatest common divisor of the numerator and the denominator (by 100), we obtain fraction 20/3.</p>
