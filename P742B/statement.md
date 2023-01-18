## Description

<div><p><span class="tex-font-style-it">There are some beautiful girls in Arpa’s land as mentioned before.</span></p><p>Once Arpa came up with an obvious problem:</p><p>Given an array and a number <span class="tex-span"><i>x</i></span>, count the number of pairs of indices <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>) such that <img align="middle" class="tex-formula" src="file://ItrxtZNO.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://EOgfEZzb.png" style="max-width: 100.0%;max-height: 100.0%;"> is bitwise <span class="tex-font-style-tt">xor</span> operation (see notes for explanation).</p><center> <img class="tex-graphics" height="222px" src="file://IsKYVXyz.png" style="max-width: 100.0%;max-height: 100.0%;" width="210px"> </center><p>Immediately, Mehrdad discovered a terrible solution that nobody trusted. Now Arpa needs your help to implement the solution to that problem.</p></div><div class="input-specification"><p>First line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the array and the integer <span class="tex-span"><i>x</i></span>.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Print a single integer: the answer to the problem.</p></div>

## Input

<p>First line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the array and the integer <span class="tex-span"><i>x</i></span>.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the elements of the array.</p>

## Output

<p>Print a single integer: the answer to the problem.</p>





```input1
2 3
1 2

```




```input2
6 1
5 1 2 3 4 1

```




```output1
1
```




```output2
2
```



## Note

<p>In the first sample there is only one pair of <span class="tex-span"><i>i</i> = 1</span> and <span class="tex-span"><i>j</i> = 2</span>. <img align="middle" class="tex-formula" src="file://EEiICnoa.png" style="max-width: 100.0%;max-height: 100.0%;"> so the answer is <span class="tex-span">1</span>.</p><p>In the second sample the only two pairs are <span class="tex-span"><i>i</i> = 3</span>, <span class="tex-span"><i>j</i> = 4</span> (since <img align="middle" class="tex-formula" src="file://lqqvfHc6.png" style="max-width: 100.0%;max-height: 100.0%;">) and <span class="tex-span"><i>i</i> = 1</span>, <span class="tex-span"><i>j</i> = 5</span> (since <img align="middle" class="tex-formula" src="file://feENFf3t.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>A bitwise <span class="tex-font-style-tt">xor</span> takes two bit integers of equal length and performs the logical <span class="tex-font-style-tt">xor</span> operation on each pair of corresponding bits. The result in each position is <span class="tex-span">1</span> if only the first bit is <span class="tex-span">1</span> or only the second bit is <span class="tex-span">1</span>, but will be <span class="tex-span">0</span> if both are <span class="tex-span">0</span> or both are <span class="tex-span">1</span>. You can read more about bitwise <span class="tex-font-style-tt">xor</span> operation here: <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">https://en.wikipedia.org/wiki/Bitwise_operation#XOR</a>.</p>
