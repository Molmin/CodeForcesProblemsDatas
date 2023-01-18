## Description

<div><p>Ehab has an array <span class="tex-span"><i>a</i></span> of <span class="tex-span"><i>n</i></span> integers. He likes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise-xor operation</a> and he likes to bother Mahmoud so he came up with a problem. He gave Mahmoud <span class="tex-span"><i>q</i></span> queries. In each of them, he gave Mahmoud 2 integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>x</i></span>, and asked him to find the number of subsequences of the first <span class="tex-span"><i>l</i></span> elements of the array such that their bitwise-xor sum is <span class="tex-span"><i>x</i></span>. Can you help Mahmoud answer the queries?</p><p>A subsequence can contain elements that are not neighboring.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of elements in the array and the number of queries.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">20</sup>)</span>, the elements of the array.</p><p>The next <span class="tex-span"><i>q</i></span> lines, each contains integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> &lt; 2<sup class="upper-index">20</sup>)</span>, representing the queries.</p></div><div class="output-specification"><p>For each query, output its answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> in a newline.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of elements in the array and the number of queries.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">20</sup>)</span>, the elements of the array.</p><p>The next <span class="tex-span"><i>q</i></span> lines, each contains integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> &lt; 2<sup class="upper-index">20</sup>)</span>, representing the queries.</p>

## Output

<p>For each query, output its answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> in a newline.</p>





```input1
5 5
0 1 2 3 4
4 3
2 0
3 7
5 7
5 8

```




```input2
3 2
1 1 1
3 1
2 0

```




```output1
4
2
0
4
0

```




```output2
4
2

```



## Note

<p>The bitwise-xor sum of the empty set is 0 and the bitwise-xor sum of a set containing one element is that element itself.</p>
