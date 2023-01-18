## Description

<div><p>Nick is attracted by everything unconventional. He doesn't like decimal number system any more, and he decided to study other number systems. A number system with base <span class="tex-span"><i>b</i></span> caught his attention. Before he starts studying it, he wants to write in his notepad all the numbers of length <span class="tex-span"><i>n</i></span> without leading zeros in this number system. Each page in Nick's notepad has enough space for <span class="tex-span"><i>c</i></span> numbers exactly. Nick writes every suitable number only once, starting with the first clean page and leaving no clean spaces. Nick never writes number <span class="tex-span">0</span> as he has unpleasant memories about zero divide.</p><p>Would you help Nick find out how many numbers will be written on the last page.</p></div><div class="input-specification"><p>The only input line contains three space-separated integers <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>b</i> &lt; 10<sup class="upper-index">10<sup class="upper-index">6</sup></sup></span>, <span class="tex-span">1 ≤ <i>n</i> &lt; 10<sup class="upper-index">10<sup class="upper-index">6</sup></sup></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>). You may consider that Nick has infinite patience, endless amount of paper and representations of digits as characters. The numbers doesn't contain leading zeros.</p></div><div class="output-specification"><p>In the only line output the amount of numbers written on the same page as the last number.</p></div>

## Input

<p>The only input line contains three space-separated integers <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>b</i> &lt; 10<sup class="upper-index">10<sup class="upper-index">6</sup></sup></span>, <span class="tex-span">1 ≤ <i>n</i> &lt; 10<sup class="upper-index">10<sup class="upper-index">6</sup></sup></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>). You may consider that Nick has infinite patience, endless amount of paper and representations of digits as characters. The numbers doesn't contain leading zeros.</p>

## Output

<p>In the only line output the amount of numbers written on the same page as the last number.</p>





```input1
2 3 3

```




```input2
2 3 4

```




```output1
1
```




```output2
4
```



## Note

<p>In both samples there are exactly <span class="tex-span">4</span> numbers of length <span class="tex-span">3</span> in binary number system. In the first sample Nick writes <span class="tex-span">3</span> numbers on the first page and <span class="tex-span">1</span> on the second page. In the second sample all the <span class="tex-span">4</span> numbers can be written on the first page.</p>
