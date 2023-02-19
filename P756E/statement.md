## Description

<div><p>There are <span class="tex-span"><i>n</i></span> types of coins in Byteland. Conveniently, the denomination of the coin type <span class="tex-span"><i>k</i></span> divides the denomination of the coin type <span class="tex-span"><i>k</i> + 1</span>, the denomination of the coin type <span class="tex-span">1</span> equals <span class="tex-span">1</span> tugrick. The ratio of the denominations of coin types <span class="tex-span"><i>k</i> + 1</span> and <span class="tex-span"><i>k</i></span> equals <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>. It is known that for each <span class="tex-span"><i>x</i></span> there are at most <span class="tex-font-style-bf">20</span> coin types of denomination <span class="tex-span"><i>x</i></span>.</p><p>Byteasar has <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span> coins of type <span class="tex-span"><i>k</i></span> with him, and he needs to pay exactly <span class="tex-span"><i>m</i></span> tugricks. It is known that Byteasar never has more than <span class="tex-span">3·10<sup class="upper-index">5</sup></span> coins with him. Byteasar want to know how many ways there are to pay exactly <span class="tex-span"><i>m</i></span> tugricks. Two ways are different if there is an integer <span class="tex-span"><i>k</i></span> such that the amount of coins of type <span class="tex-span"><i>k</i></span> differs in these two ways. As all Byteland citizens, Byteasar wants to know the number of ways modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of coin types.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the ratios between the coin types denominations. It is guaranteed that for each <span class="tex-span"><i>x</i></span> there are at most <span class="tex-font-style-bf">20</span> coin types of denomination <span class="tex-span"><i>x</i></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— the number of coins of each type Byteasar has. It is guaranteed that the sum of these integers doesn't exceed <span class="tex-span">3·10<sup class="upper-index">5</sup></span>.</p><p>The fourth line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> &lt; 10<sup class="upper-index">10000</sup></span>)&nbsp;— the amount in tugricks Byteasar needs to pay.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the number of ways to pay exactly <span class="tex-span"><i>m</i></span> tugricks modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of coin types.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the ratios between the coin types denominations. It is guaranteed that for each <span class="tex-span"><i>x</i></span> there are at most <span class="tex-font-style-bf">20</span> coin types of denomination <span class="tex-span"><i>x</i></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— the number of coins of each type Byteasar has. It is guaranteed that the sum of these integers doesn't exceed <span class="tex-span">3·10<sup class="upper-index">5</sup></span>.</p><p>The fourth line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> &lt; 10<sup class="upper-index">10000</sup></span>)&nbsp;— the amount in tugricks Byteasar needs to pay.</p>

## Output

<p>Print single integer&nbsp;— the number of ways to pay exactly <span class="tex-span"><i>m</i></span> tugricks modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1

4
2

```




```input2
2
1
4 4
2

```




```input3
3
3 3
10 10 10
17

```




```output1
1

```




```output2
3

```




```output3
6

```



## Note

<p>In the first example Byteasar has <span class="tex-span">4</span> coins of denomination <span class="tex-span">1</span>, and he has to pay <span class="tex-span">2</span> tugricks. There is only one way.</p><p>In the second example Byteasar has <span class="tex-span">4</span> coins of each of two different types of denomination <span class="tex-span">1</span>, he has to pay <span class="tex-span">2</span> tugricks. There are <span class="tex-span">3</span> ways: pay one coin of the first type and one coin of the other, pay two coins of the first type, and pay two coins of the second type.</p><p>In the third example the denominations are equal to <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">9</span>.</p>
