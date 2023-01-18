## Description

<div><p>The good times at Heidi's library are over. Marmots finally got their internet connections and stopped coming to the library altogether. Not only that, but the bookstore has begun charging extortionate prices for some books. Namely, whereas in the previous versions each book could be bought for 1 CHF, now the price of book <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> CHF.</p></div><div class="input-specification"><p>The first line of input will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<img align="middle" class="tex-formula" src="file://3KGczmPV.png" style="max-width: 100.0%;max-height: 100.0%;">). The second line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) – the sequence of book requests. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) – the costs of the books.</p></div><div class="output-specification"><p>On a single line print the minimum cost of buying books at the store so as to satisfy all requests.</p></div>

## Input

<p>The first line of input will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<img align="middle" class="tex-formula" src="file://3KGczmPV.png" style="max-width: 100.0%;max-height: 100.0%;">). The second line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) – the sequence of book requests. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) – the costs of the books.</p>

## Output

<p>On a single line print the minimum cost of buying books at the store so as to satisfy all requests.</p>





```input1
4 80
1 2 2 1
1 1 1 1

```




```input2
4 1
1 2 2 1
1 1 1 1

```




```input3
4 2
1 2 3 1
1 1 1 1

```




```input4
7 2
1 2 3 1 1 1 2
1 10 1 0 0 0 0

```




```output1
2
```




```output2
3
```




```output3
3
```




```output4
13
```



## Note

<p>The first three sample cases are repeated, but the fourth one is new.</p><p>In the fourth test case, when buying book <span class="tex-span">3</span>, Heidi should discard either book <span class="tex-span">1</span> or <span class="tex-span">2</span>. Even though book <span class="tex-span">2</span> will be requested later than book <span class="tex-span">1</span>, she should keep it, because it is so expensive to buy again.</p>
