## Description

<div><p>Vasya has <span class="tex-span"><i>n</i></span> pairs of socks. In the morning of each day Vasya has to put on a pair of socks before he goes to school. When he comes home in the evening, Vasya takes off the used socks and throws them away. Every <span class="tex-span"><i>m</i></span>-th day (at days with numbers <span class="tex-span"><i>m</i>, 2<i>m</i>, 3<i>m</i>, ...</span>) mom buys a pair of socks to Vasya. She does it late in the evening, so that Vasya cannot put on a new pair of socks before the next day. How many consecutive days pass until Vasya runs out of socks?</p></div><div class="input-specification"><p>The single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;2 ≤ <i>m</i> ≤ 100)</span>, separated by a space.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;2 ≤ <i>m</i> ≤ 100)</span>, separated by a space.</p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
2 2

```




```input2
9 3

```




```output1
3

```




```output2
13

```



## Note

<p>In the first sample Vasya spends the first two days wearing the socks that he had initially. Then on day three he puts on the socks that were bought on day two.</p><p>In the second sample Vasya spends the first nine days wearing the socks that he had initially. Then he spends three days wearing the socks that were bought on the third, sixth and ninth days. Than he spends another day wearing the socks that were bought on the twelfth day.</p>
