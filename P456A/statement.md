## Description

<div><p>One day Dima and Alex had an argument about the price and quality of laptops. Dima thinks that the more expensive a laptop is, the better it is. Alex disagrees. Alex thinks that there are two laptops, such that the price of the first laptop is less (strictly smaller) than the price of the second laptop but the quality of the first laptop is higher (strictly greater) than the quality of the second laptop.</p><p>Please, check the guess of Alex. You are given descriptions of <span class="tex-span"><i>n</i></span> laptops. Determine whether two described above laptops exist.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of laptops.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers each, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the price of the <span class="tex-span"><i>i</i></span>-th laptop, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number that represents the quality of the <span class="tex-span"><i>i</i></span>-th laptop (the larger the number is, the higher is the quality).</p><p>All <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct. All <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct. </p></div><div class="output-specification"><p>If Alex is correct, print "<span class="tex-font-style-tt">Happy Alex</span>", otherwise print "<span class="tex-font-style-tt">Poor Alex</span>" (without the quotes).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of laptops.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers each, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the price of the <span class="tex-span"><i>i</i></span>-th laptop, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number that represents the quality of the <span class="tex-span"><i>i</i></span>-th laptop (the larger the number is, the higher is the quality).</p><p>All <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct. All <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are distinct. </p>

## Output

<p>If Alex is correct, print "<span class="tex-font-style-tt">Happy Alex</span>", otherwise print "<span class="tex-font-style-tt">Poor Alex</span>" (without the quotes).</p>





```input1
2
1 2
2 1

```




```output1
Happy Alex

```


