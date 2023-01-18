## Description

<div><p>Students love to celebrate their holidays. Especially if the holiday is the day of the end of exams!</p><p>Despite the fact that Igor K., unlike his groupmates, failed to pass a programming test, he decided to invite them to go to a cafe so that each of them could drink a bottle of... fresh cow milk. Having entered the cafe, the <span class="tex-span"><i>m</i></span> friends found <span class="tex-span"><i>n</i></span> different kinds of milk on the menu, that's why they ordered <span class="tex-span"><i>n</i></span> bottles — one bottle of each kind. We know that the volume of milk in each bottle equals <span class="tex-span"><i>w</i></span>.</p><p>When the bottles were brought in, they decided to pour all the milk evenly among the <span class="tex-span"><i>m</i></span> cups, so that each got a cup. As a punishment for not passing the test Igor was appointed the person to pour the milk. He protested that he was afraid to mix something up and suggested to distribute the drink so that the milk from each bottle was in no more than two different cups. His friends agreed but they suddenly faced the following problem — and what is actually the way to do it?</p><p>Help them and write the program that will help to distribute the milk among the cups and drink it as quickly as possible!</p><p>Note that due to Igor K.'s perfectly accurate eye and unswerving hands, he can pour any fractional amount of milk from any bottle to any cup.</p></div><div class="input-specification"><p>The only input data file contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">100 ≤ <i>w</i> ≤ 1000</span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 50</span>), where <span class="tex-span"><i>n</i></span> stands for the number of ordered bottles, <span class="tex-span"><i>w</i></span> stands for the volume of each of them and <span class="tex-span"><i>m</i></span> stands for the number of friends in the company.</p></div><div class="output-specification"><p>Print on the first line "<span class="tex-font-style-tt">YES</span>" if it is possible to pour the milk so that the milk from each bottle was in no more than two different cups. If there's no solution, print "<span class="tex-font-style-tt">NO</span>".</p><p>If there is a solution, then print <span class="tex-span"><i>m</i></span> more lines, where the <span class="tex-span"><i>i</i></span>-th of them describes the content of the <span class="tex-span"><i>i</i></span>-th student's cup. The line should consist of one or more pairs that would look like "<span class="tex-span"><i>b</i></span> <span class="tex-span"><i>v</i></span>". Each such pair means that <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>v</i> &gt; 0</span>) units of milk were poured into the <span class="tex-span"><i>i</i></span>-th cup from bottle <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>n</i></span>). All numbers <span class="tex-span"><i>b</i></span> on each line should be different.</p><p>If there are several variants to solve the problem, print any of them. Print the real numbers with no less than 6 digits after the decimal point.</p></div>

## Input

<p>The only input data file contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">100 ≤ <i>w</i> ≤ 1000</span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 50</span>), where <span class="tex-span"><i>n</i></span> stands for the number of ordered bottles, <span class="tex-span"><i>w</i></span> stands for the volume of each of them and <span class="tex-span"><i>m</i></span> stands for the number of friends in the company.</p>

## Output

<p>Print on the first line "<span class="tex-font-style-tt">YES</span>" if it is possible to pour the milk so that the milk from each bottle was in no more than two different cups. If there's no solution, print "<span class="tex-font-style-tt">NO</span>".</p><p>If there is a solution, then print <span class="tex-span"><i>m</i></span> more lines, where the <span class="tex-span"><i>i</i></span>-th of them describes the content of the <span class="tex-span"><i>i</i></span>-th student's cup. The line should consist of one or more pairs that would look like "<span class="tex-span"><i>b</i></span> <span class="tex-span"><i>v</i></span>". Each such pair means that <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>v</i> &gt; 0</span>) units of milk were poured into the <span class="tex-span"><i>i</i></span>-th cup from bottle <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>n</i></span>). All numbers <span class="tex-span"><i>b</i></span> on each line should be different.</p><p>If there are several variants to solve the problem, print any of them. Print the real numbers with no less than 6 digits after the decimal point.</p>





```input1
2 500 3

```




```input2
4 100 5

```




```input3
4 100 7

```




```input4
5 500 2

```




```output1
YES
1 333.333333
2 333.333333
2 166.666667 1 166.666667

```




```output2
YES
3 20.000000 4 60.000000
1 80.000000
4 40.000000 2 40.000000
3 80.000000
2 60.000000 1 20.000000

```




```output3
NO

```




```output4
YES
4 250.000000 5 500.000000 2 500.000000
3 500.000000 1 500.000000 4 250.000000

```


