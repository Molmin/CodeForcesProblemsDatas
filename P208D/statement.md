## Description

<div><p>Vasya, like many others, likes to participate in a variety of sweepstakes and lotteries. Now he collects wrappings from a famous chocolate bar "Jupiter". According to the sweepstake rules, each wrapping has an integer written on it — the number of points that the participant adds to his score as he buys the bar. After a participant earns a certain number of points, he can come to the prize distribution center and exchange the points for prizes. When somebody takes a prize, the prize's cost is simply subtracted from the number of his points.</p><p>Vasya didn't only bought the bars, he also kept a record of how many points each wrapping cost. Also, he remembers that he always stucks to the greedy strategy — as soon as he could take at least one prize, he went to the prize distribution centre and exchanged the points for prizes. Moreover, if he could choose between multiple prizes, he chose the most expensive one. If after an exchange Vasya had enough points left to get at least one more prize, then he continued to exchange points.</p><p>The sweepstake has the following prizes (the prizes are sorted by increasing of their cost): </p><ul> <li> a mug (costs <span class="tex-span"><i>a</i></span> points), </li><li> a towel (costs <span class="tex-span"><i>b</i></span> points), </li><li> a bag (costs <span class="tex-span"><i>c</i></span> points), </li><li> a bicycle (costs <span class="tex-span"><i>d</i></span> points), </li><li> a car (costs <span class="tex-span"><i>e</i></span> points). </li></ul><p>Now Vasya wants to recollect what prizes he has received. You know sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the number of points Vasya got for the <span class="tex-span"><i>i</i></span>-th bar. The sequence of points is given in the chronological order. You also know numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>e</i></span>. Your task is to find, how many prizes Vasya received, what prizes they are and how many points he's got left after all operations are completed.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of chocolate bar wrappings that brought points to Vasya. The second line contains space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The third line contains 5 integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>e</i></span> (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> &lt; <i>c</i> &lt; <i>d</i> &lt; <i>e</i> ≤ 10<sup class="upper-index">9</sup></span>) — the prizes' costs.</p></div><div class="output-specification"><p>Print on the first line 5 integers, separated by a space — the number of mugs, towels, bags, bicycles and cars that Vasya has got, respectively. On the second line print a single integer — the number of points Vasya will have left after all operations of exchange are completed.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of chocolate bar wrappings that brought points to Vasya. The second line contains space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The third line contains 5 integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>e</i></span> (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> &lt; <i>c</i> &lt; <i>d</i> &lt; <i>e</i> ≤ 10<sup class="upper-index">9</sup></span>) — the prizes' costs.</p>

## Output

<p>Print on the first line 5 integers, separated by a space — the number of mugs, towels, bags, bicycles and cars that Vasya has got, respectively. On the second line print a single integer — the number of points Vasya will have left after all operations of exchange are completed.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3
3 10 4
2 4 10 15 20

```




```input2
4
10 4 39 2
3 5 10 11 12

```




```output1
1 1 1 0 0 
1

```




```output2
3 0 1 0 3 
0

```



## Note

<p>In the first sample Vasya gets <span class="tex-span">3</span> points after eating the first chocolate bar. Then he exchanges <span class="tex-span">2</span> points and gets a mug. Vasya wins a <span class="tex-font-style-bf">bag</span> after eating the second chocolate bar. Then he wins a <span class="tex-font-style-bf">towel</span> after eating the third chocolate bar. After all chocolate bars <span class="tex-span">3 - 2 + 10 - 10 + 4 - 4 = 1</span> points remains.</p>
