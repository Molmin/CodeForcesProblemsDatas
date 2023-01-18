## Description

<div><p>It's another Start[c]up, and that means there are T-shirts to order. In order to make sure T-shirts are shipped as soon as possible, we've decided that this year we're going to order all of the necessary T-shirts before the actual competition. The top <span class="tex-span"><i>C</i></span> contestants are going to be awarded T-shirts, but we obviously don't know which contestants that will be. The plan is to get the T-Shirt sizes of all contestants before the actual competition, and then order enough T-shirts so that no matter who is in the top <span class="tex-span"><i>C</i></span> we'll have T-shirts available in order to award them.</p><p>In order to get the T-shirt sizes of the contestants, we will send out a survey. The survey will allow contestants to either specify a single desired T-shirt size, or two adjacent T-shirt sizes. If a contestant specifies two sizes, it means that they can be awarded either size.</p><p>As you can probably tell, this plan could require ordering a lot of unnecessary T-shirts. We'd like your help to determine the minimum number of T-shirts we'll need to order to ensure that we'll be able to award T-shirts no matter the outcome of the competition.</p></div><div class="input-specification"><p>Input will begin with two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>C</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>C</i></span>), the number of T-shirt sizes and number of T-shirts to be awarded, respectively.</p><p>Following this is a line with <span class="tex-span">2·<i>N</i> - 1</span> integers, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> through <span class="tex-span"><i>s</i><sub class="lower-index">2·<i>N</i> - 1</sub></span> <span class="tex-span">(0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>. For odd <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> indicates the number of contestants desiring T-shirt size <span class="tex-span">((<i>i</i> + 1) / 2)</span>. For even <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> indicates the number of contestants okay receiving either of T-shirt sizes <span class="tex-span">(<i>i</i> / 2)</span> and <span class="tex-span">(<i>i</i> / 2 + 1)</span>. <span class="tex-span"><i>C</i></span> will not exceed the total number of contestants.</p></div><div class="output-specification"><p>Print the minimum number of T-shirts we need to buy.</p></div>

## Input

<p>Input will begin with two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>C</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>C</i></span>), the number of T-shirt sizes and number of T-shirts to be awarded, respectively.</p><p>Following this is a line with <span class="tex-span">2·<i>N</i> - 1</span> integers, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> through <span class="tex-span"><i>s</i><sub class="lower-index">2·<i>N</i> - 1</sub></span> <span class="tex-span">(0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>. For odd <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> indicates the number of contestants desiring T-shirt size <span class="tex-span">((<i>i</i> + 1) / 2)</span>. For even <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> indicates the number of contestants okay receiving either of T-shirt sizes <span class="tex-span">(<i>i</i> / 2)</span> and <span class="tex-span">(<i>i</i> / 2 + 1)</span>. <span class="tex-span"><i>C</i></span> will not exceed the total number of contestants.</p>

## Output

<p>Print the minimum number of T-shirts we need to buy.</p>





```input1
2 200
100 250 100

```




```input2
4 160
88 69 62 29 58 52 44

```




```output1
200

```




```output2
314

```



## Note

<p>In the first example, we can buy <span class="tex-span">100</span> of each size.</p>
