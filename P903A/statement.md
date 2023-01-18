## Description

<div><p>Ivan's classes at the university have just finished, and now he wants to go to the local CFK cafe and eat some fried chicken.</p><p>CFK sells chicken chunks in small and large portions. A small portion contains <span class="tex-span">3</span> chunks; a large one — <span class="tex-span">7</span> chunks. Ivan wants to eat exactly <span class="tex-span"><i>x</i></span> chunks. Now he wonders whether he can buy exactly this amount of chicken.</p><p>Formally, Ivan wants to know if he can choose two non-negative integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> in such a way that <span class="tex-span"><i>a</i></span> small portions and <span class="tex-span"><i>b</i></span> large ones contain exactly <span class="tex-span"><i>x</i></span> chunks.</p><p>Help Ivan to answer this question for several values of <span class="tex-span"><i>x</i></span>!</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of testcases.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains one integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of chicken chunks Ivan wants to eat.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, in <span class="tex-span"><i>i</i></span>-th line output <span class="tex-font-style-tt">YES</span> if Ivan can buy exactly <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> chunks. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of testcases.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains one integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the number of chicken chunks Ivan wants to eat.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, in <span class="tex-span"><i>i</i></span>-th line output <span class="tex-font-style-tt">YES</span> if Ivan can buy exactly <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> chunks. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
2
6
5

```




```output1
YES
NO

```



## Note

<p>In the first example Ivan can buy two small portions.</p><p>In the second example Ivan cannot buy exactly <span class="tex-span">5</span> chunks, since one small portion is not enough, but two small portions or one large is too much.</p>
