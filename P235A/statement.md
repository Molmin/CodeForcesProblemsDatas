## Description

<div><p>Some days ago, I learned the concept of LCM (least common multiple). I've played with it for several times and I want to make a big number with it.</p><p>But I also don't want to use many numbers, so I'll choose three positive integers (they don't have to be distinct) which are not greater than <span class="tex-span"><i>n</i></span>. Can you help me to find the maximum possible least common multiple of these three integers?</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the <span class="tex-span"><i>n</i></span> mentioned in the statement.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible LCM of three not necessarily distinct positive integers that are not greater than <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the <span class="tex-span"><i>n</i></span> mentioned in the statement.</p>

## Output

<p>Print a single integer — the maximum possible LCM of three not necessarily distinct positive integers that are not greater than <span class="tex-span"><i>n</i></span>.</p>





```input1
9

```




```input2
7

```




```output1
504

```




```output2
210

```



## Note

<p>The least common multiple of some positive integers is the least positive integer which is multiple for each of them.</p><p>The result may become very large, 32-bit integer won't be enough. So using 64-bit integers is recommended.</p><p>For the last example, we can chose numbers <span class="tex-span">7</span>, <span class="tex-span">6</span>, <span class="tex-span">5</span> and the LCM of them is <span class="tex-span">7·6·5 = 210</span>. It is the maximum value we can get.</p>
