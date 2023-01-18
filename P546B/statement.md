## Description

<div><p>Colonel has <span class="tex-span"><i>n</i></span> badges. He wants to give one badge to every of his <span class="tex-span"><i>n</i></span> soldiers. Each badge has a <span class="tex-font-style-it">coolness factor</span>, which shows how much it's owner reached. Coolness factor can be increased by one for the cost of one coin. </p><p>For every pair of soldiers one of them should get a badge with strictly higher factor than the second one. Exact values of their factors aren't important, they just need to have distinct factors. </p><p>Colonel knows, which soldier is supposed to get which badge initially, but there is a problem. Some of badges may have the same factor of coolness. Help him and calculate how much money has to be paid for making all badges have different factors of coolness.</p></div><div class="input-specification"><p>First line of input consists of one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>).</p><p>Next line consists of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), which stand for coolness factor of each badge.</p></div><div class="output-specification"><p>Output single integer — minimum amount of coins the colonel has to pay.</p></div>

## Input

<p>First line of input consists of one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>).</p><p>Next line consists of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), which stand for coolness factor of each badge.</p>

## Output

<p>Output single integer — minimum amount of coins the colonel has to pay.</p>





```input1
4
1 3 1 4

```




```input2
5
1 2 3 2 5

```




```output1
1
```




```output2
2
```



## Note

<p>In first sample test we can increase factor of first badge by <span class="tex-span">1</span>.</p><p>In second sample test we can increase factors of the second and the third badge by <span class="tex-span">1</span>.</p>
