## Description

<div><p>Inna is fed up with jokes about female logic. So she started using binary logic instead.</p><p>Inna has an array of <span class="tex-span"><i>n</i></span> elements <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>[1], <i>a</i><sub class="lower-index">1</sub>[2], ..., <i>a</i><sub class="lower-index">1</sub>[<i>n</i>]</span>. Girl likes to train in her binary logic, so she does an exercise consisting of <span class="tex-span"><i>n</i></span> stages: on the first stage Inna writes out all numbers from array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, on the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(<i>i</i> ≥ 2)</span> stage girl writes all elements of array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, which consists of <span class="tex-span"><i>n</i> - <i>i</i> + 1</span> integers; the <span class="tex-span"><i>k</i></span>-th integer of array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is defined as follows: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>[<i>k</i>] = <i>a</i><sub class="lower-index"><i>i</i> - 1</sub>[<i>k</i>]&nbsp;<i>AND</i>&nbsp;<i>a</i><sub class="lower-index"><i>i</i> - 1</sub>[<i>k</i> + 1]</span>. Here AND is bit-wise binary logical operation.</p><p>Dima decided to check Inna's skill. He asks Inna to change array, perform the exercise and say the sum of all <img align="middle" class="tex-formula" src="file://GjdtaAkZ.png" style="max-width: 100.0%;max-height: 100.0%;"> elements she wrote out during the current exercise.</p><p>Help Inna to answer the questions!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — size of array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and number of Dima's questions. Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>[1], <i>a</i><sub class="lower-index">1</sub>[2], ..., <i>a</i><sub class="lower-index">1</sub>[<i>n</i>]</span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — initial array elements.</p><p>Each of next <span class="tex-span"><i>m</i></span> lines contains two integers — Dima's question description. Each question consists of two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. For this question Inna should make <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>[<i>p</i><sub class="lower-index"><i>i</i></sub>]</span> equals <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, and then perform the exercise. Please, note that changes are saved from question to question.</p></div><div class="output-specification"><p>For each question print Inna's answer on a single line.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — size of array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and number of Dima's questions. Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>[1], <i>a</i><sub class="lower-index">1</sub>[2], ..., <i>a</i><sub class="lower-index">1</sub>[<i>n</i>]</span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — initial array elements.</p><p>Each of next <span class="tex-span"><i>m</i></span> lines contains two integers — Dima's question description. Each question consists of two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. For this question Inna should make <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>[<i>p</i><sub class="lower-index"><i>i</i></sub>]</span> equals <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, and then perform the exercise. Please, note that changes are saved from question to question.</p>

## Output

<p>For each question print Inna's answer on a single line.</p>





```input1
3 4
1 1 1
1 1
2 2
3 2
1 2

```




```output1
6
4
7
12

```


