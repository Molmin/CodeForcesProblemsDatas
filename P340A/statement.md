## Description

<div><p>Iahub and his friend Floyd have started painting a wall. Iahub is painting the wall red and Floyd is painting it pink. You can consider the wall being made of a very large number of bricks, numbered <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and so on. </p><p>Iahub has the following scheme of painting: he skips <span class="tex-span"><i>x</i> - 1</span> consecutive bricks, then he paints the <span class="tex-span"><i>x</i></span>-th one. That is, he'll paint bricks <span class="tex-span"><i>x</i></span>, <span class="tex-span">2·<i>x</i></span>, <span class="tex-span">3·<i>x</i></span> and so on red. Similarly, Floyd skips <span class="tex-span"><i>y</i> - 1</span> consecutive bricks, then he paints the <span class="tex-span"><i>y</i></span>-th one. Hence he'll paint bricks <span class="tex-span"><i>y</i></span>, <span class="tex-span">2·<i>y</i></span>, <span class="tex-span">3·<i>y</i></span> and so on pink.</p><p>After painting the wall all day, the boys observed that some bricks are painted both red and pink. Iahub has a lucky number <span class="tex-span"><i>a</i></span> and Floyd has a lucky number <span class="tex-span"><i>b</i></span>. Boys wonder how many bricks numbered no less than <span class="tex-span"><i>a</i></span> and no greater than <span class="tex-span"><i>b</i></span> are painted both red and pink. This is exactly your task: compute and print the answer to the question. </p></div><div class="input-specification"><p>The input will have a single line containing four integers in this order: <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>. (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 2·10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i> ≤ <i>b</i></span>).</p></div><div class="output-specification"><p>Output a single integer — the number of bricks numbered no less than <span class="tex-span"><i>a</i></span> and no greater than <span class="tex-span"><i>b</i></span> that are painted both red and pink.</p></div>

## Input

<p>The input will have a single line containing four integers in this order: <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>. (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 2·10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i> ≤ <i>b</i></span>).</p>

## Output

<p>Output a single integer — the number of bricks numbered no less than <span class="tex-span"><i>a</i></span> and no greater than <span class="tex-span"><i>b</i></span> that are painted both red and pink.</p>





```input1
2 3 6 18

```




```output1
3
```



## Note

<p>Let's look at the bricks from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>a</i> = 6, <i>b</i> = 18)</span>. The bricks colored in red are numbered 6, 8, 10, 12, 14, 16, 18. The bricks colored in pink are numbered 6, 9, 12, 15, 18. The bricks colored in both red and pink are numbered with 6, 12 and 18. </p>
