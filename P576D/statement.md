## Description

<div><p>In the country there are exactly <span class="tex-span"><i>n</i></span> cities numbered with positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. In each city there is an airport is located.</p><p>Also, there is the only one airline, which makes <span class="tex-span"><i>m</i></span> flights. Unfortunately, to use them, you need to be a regular customer of this company, namely, you have the opportunity to enjoy flight <span class="tex-span"><i>i</i></span> from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> only if you have already made at least <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> flights before that.</p><p>Please note that flight <span class="tex-span"><i>i</i></span> flies exactly from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It can not be used to fly from city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. An interesting fact is that there may possibly be recreational flights with a beautiful view of the sky, which begin and end in the same city.</p><p>You need to get from city <span class="tex-span">1</span> to city <span class="tex-span"><i>n</i></span>. Unfortunately, you've never traveled by plane before. What minimum number of flights you have to perform in order to get to city <span class="tex-span"><i>n</i></span>?</p><p>Note that the same flight can be used multiple times.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 150</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 150</span>) — the number of cities in the country and the number of flights the company provides.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), representing flight number <span class="tex-span"><i>i</i></span> from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, accessible to only the clients who have made at least <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> flights. </p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes), if it is impossible to get from city <span class="tex-span">1</span> to city <span class="tex-span"><i>n</i></span> using the airways.</p><p>But if there is at least one way, print a single integer — the minimum number of flights you need to make to get to the destination point.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 150</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 150</span>) — the number of cities in the country and the number of flights the company provides.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), representing flight number <span class="tex-span"><i>i</i></span> from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, accessible to only the clients who have made at least <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> flights. </p>

## Output

<p>Print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes), if it is impossible to get from city <span class="tex-span">1</span> to city <span class="tex-span"><i>n</i></span> using the airways.</p><p>But if there is at least one way, print a single integer — the minimum number of flights you need to make to get to the destination point.</p>





```input1
3 2
1 2 0
2 3 1

```




```input2
2 1
1 2 100500

```




```input3
3 3
2 1 0
2 3 6
1 2 0

```




```output1
2

```




```output2
Impossible

```




```output3
8

```


