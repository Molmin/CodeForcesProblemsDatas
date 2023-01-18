## Description

<div><p>The Hedgehog likes to give presents to his friend, but no less he likes to receive them.</p><p>Having received another present today, the Hedgehog suddenly understood that he has no place to put it as there was no room left on the special shelf in the cupboard. He will have to choose another shelf, but which one should he choose, how large should it be?</p><p>In order to get to know this, the Hedgehog asks you to write him a program that will count the estimated number of presents that he will receive during the following <span class="tex-span"><i>N</i></span> days. Besides, he is guided by the principle: </p><ul> <li> on each holiday day the Hedgehog will necessarily receive a present, </li><li> he receives presents at least every <span class="tex-span"><i>K</i></span> days (i.e., if he received a present on the <span class="tex-span"><i>i</i></span>-th day, he will receive the next present no later than on the <span class="tex-span"><i>i</i> + <i>K</i></span>-th day). </li></ul> <p>For the given <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span>, as well as the list of holidays among the following <span class="tex-span"><i>N</i></span> days count the minimal number of presents that could be given to the Hedgehog. The number of today's day is zero, and you should regard today's present as already given (i.e., you shouldn't count it in the answer).</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 365</span>, <span class="tex-span">1 ≤ <i>K</i> ≤ <i>N</i></span>).</p><p>The second line contains a number <span class="tex-span"><i>C</i></span> which represents the number of holidays (<span class="tex-span">0 ≤ <i>C</i> ≤ <i>N</i></span>). Then in the same line follow <span class="tex-span"><i>C</i></span> numbers ranging from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span> which are the numbers of holiday days. The numbers are given in the increasing order, without repeating numbers among them.</p></div><div class="output-specification"><p>Print a single number — the minimal number of presents the Hedgehog will receive over the following <span class="tex-span"><i>N</i></span> days.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 365</span>, <span class="tex-span">1 ≤ <i>K</i> ≤ <i>N</i></span>).</p><p>The second line contains a number <span class="tex-span"><i>C</i></span> which represents the number of holidays (<span class="tex-span">0 ≤ <i>C</i> ≤ <i>N</i></span>). Then in the same line follow <span class="tex-span"><i>C</i></span> numbers ranging from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span> which are the numbers of holiday days. The numbers are given in the increasing order, without repeating numbers among them.</p>

## Output

<p>Print a single number — the minimal number of presents the Hedgehog will receive over the following <span class="tex-span"><i>N</i></span> days.</p>





```input1
5 2
1 3

```




```input2
10 1
3 6 7 8

```




```output1
3
```




```output2
10
```


