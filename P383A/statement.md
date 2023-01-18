## Description

<div><p>Iahub helps his grandfather at the farm. Today he must milk the cows. There are <span class="tex-span"><i>n</i></span> cows sitting in a row, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Each cow is either facing to the left or facing to the right. When Iahub milks a cow, all the cows that see the current cow get scared and lose one unit of the quantity of milk that they can give. A cow facing left sees all the cows with lower indices than her index, and a cow facing right sees all the cows with higher indices than her index. A cow that got scared once can get scared again (and lose one more unit of milk). A cow that has been milked once cannot get scared and lose any more milk. You can assume that a cow never loses all the milk she can give (a cow gives an infinitely amount of milk).</p><p>Iahub can decide the order in which he milks the cows. But he must milk each cow exactly once. Iahub wants to lose as little milk as possible. Print the minimum amount of milk that is lost.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is <span class="tex-span">0</span> if the cow number <span class="tex-span"><i>i</i></span> is facing left, and <span class="tex-span">1</span> if it is facing right.</p></div><div class="output-specification"><p>Print a single integer, the minimum amount of lost milk.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200000)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is <span class="tex-span">0</span> if the cow number <span class="tex-span"><i>i</i></span> is facing left, and <span class="tex-span">1</span> if it is facing right.</p>

## Output

<p>Print a single integer, the minimum amount of lost milk.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4
0 0 1 0

```




```input2
5
1 0 1 0 1

```




```output1
1
```




```output2
3
```



## Note

<p>In the first sample Iahub milks the cows in the following order: cow <span class="tex-span">3</span>, cow <span class="tex-span">4</span>, cow <span class="tex-span">2</span>, cow <span class="tex-span">1</span>. When he milks cow <span class="tex-span">3</span>, cow <span class="tex-span">4</span> loses <span class="tex-span">1</span> unit of milk. After that, no more milk is lost.</p>
