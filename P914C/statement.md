## Description

<div><p>The Travelling Salesman spends a lot of time travelling so he tends to get bored. To pass time, he likes to perform operations on numbers. One such operation is to take a positive integer <span class="tex-span"><i>x</i></span> and reduce it to the number of bits set to <span class="tex-span">1</span> in the binary representation of <span class="tex-span"><i>x</i></span>. For example for number <span class="tex-span">13</span> it's true that <span class="tex-span">13<sub class="lower-index">10</sub> = 1101<sub class="lower-index">2</sub></span>, so it has <span class="tex-span">3</span> bits set and <span class="tex-span">13</span> will be reduced to <span class="tex-span">3</span> in one operation.</p><p>He calls a number <span class="tex-font-style-it">special</span> if the minimum number of operations to reduce it to <span class="tex-span">1</span> is <span class="tex-span"><i>k</i></span>.</p><p>He wants to find out how many special numbers exist which are not greater than <span class="tex-span"><i>n</i></span>. Please help the Travelling Salesman, as he is about to reach his destination!</p><p>Since the answer can be large, output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> &lt; 2<sup class="upper-index">1000</sup></span>).</p><p>The second line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 1000</span>).</p><p>Note that <span class="tex-span"><i>n</i></span> is given in its binary representation without any leading zeros.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of special numbers not greater than <span class="tex-span"><i>n</i></span>, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> &lt; 2<sup class="upper-index">1000</sup></span>).</p><p>The second line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 1000</span>).</p><p>Note that <span class="tex-span"><i>n</i></span> is given in its binary representation without any leading zeros.</p>

## Output

<p>Output a single integer&nbsp;— the number of special numbers not greater than <span class="tex-span"><i>n</i></span>, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
110
2

```




```input2
111111011
2

```




```output1
3

```




```output2
169

```



## Note

<p>In the first sample, the three special numbers are <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span>. They get reduced to <span class="tex-span">2</span> in one operation (since there are two set bits in each of <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span>) and then to <span class="tex-span">1</span> in one more operation (since there is only one set bit in <span class="tex-span">2</span>).</p>
