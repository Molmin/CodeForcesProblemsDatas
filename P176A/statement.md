## Description

<div><p>To get money for a new aeonic blaster, ranger Qwerty decided to engage in trade for a while. He wants to buy some number of items (or probably not to buy anything at all) on one of the planets, and then sell the bought items on another planet. Note that this operation is not repeated, that is, the buying and the selling are made only once. To carry out his plan, Qwerty is going to take a bank loan that covers all expenses and to return the loaned money at the end of the operation (the money is returned without the interest). At the same time, Querty wants to get as much profit as possible.</p><p>The system has <span class="tex-span"><i>n</i></span> planets in total. On each of them Qwerty can buy or sell items of <span class="tex-span"><i>m</i></span> types (such as food, medicine, weapons, alcohol, and so on). For each planet <span class="tex-span"><i>i</i></span> and each type of items <span class="tex-span"><i>j</i></span> Qwerty knows the following:</p><ul><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> — the cost of buying an item; </li><li> <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub></span> — the cost of selling an item; </li><li> <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> — the number of remaining items.</li></ul><p>It is not allowed to buy more than <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> items of type <span class="tex-span"><i>j</i></span> on planet <span class="tex-span"><i>i</i></span>, but it is allowed to sell any number of items of any kind.</p><p>Knowing that the hold of Qwerty's ship has room for no more than <span class="tex-span"><i>k</i></span> items, determine the maximum profit which Qwerty can get.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 100</span>) — the number of planets, the number of question types and the capacity of Qwerty's ship hold, correspondingly.</p><p>Then follow <span class="tex-span"><i>n</i></span> blocks describing each planet.</p><p>The first line of the <span class="tex-span"><i>i</i></span>-th block has the planet's name as a string with length from <span class="tex-span">1</span> to <span class="tex-span">10</span> Latin letters. The first letter of the name is uppercase, the rest are lowercase. Then in the <span class="tex-span"><i>i</i></span>-th block follow <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>j</i></span>-th of them contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>ij</i></sub> &lt; <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 100</span>) — the numbers that describe money operations with the <span class="tex-span"><i>j</i></span>-th item on the <span class="tex-span"><i>i</i></span>-th planet. The numbers in the lines are separated by spaces.</p><p>It is guaranteed that the names of all planets are different.</p></div><div class="output-specification"><p>Print a single number — the maximum profit Qwerty can get.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 100</span>) — the number of planets, the number of question types and the capacity of Qwerty's ship hold, correspondingly.</p><p>Then follow <span class="tex-span"><i>n</i></span> blocks describing each planet.</p><p>The first line of the <span class="tex-span"><i>i</i></span>-th block has the planet's name as a string with length from <span class="tex-span">1</span> to <span class="tex-span">10</span> Latin letters. The first letter of the name is uppercase, the rest are lowercase. Then in the <span class="tex-span"><i>i</i></span>-th block follow <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>j</i></span>-th of them contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>ij</i></sub> &lt; <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 100</span>) — the numbers that describe money operations with the <span class="tex-span"><i>j</i></span>-th item on the <span class="tex-span"><i>i</i></span>-th planet. The numbers in the lines are separated by spaces.</p><p>It is guaranteed that the names of all planets are different.</p>

## Output

<p>Print a single number — the maximum profit Qwerty can get.</p>





```input1
3 3 10
Venus
6 5 3
7 6 5
8 6 10
Earth
10 9 0
8 6 4
10 9 3
Mars
4 3 0
8 4 12
7 2 5

```




```output1
16
```



## Note

<p>In the first test case you should fly to planet <span class="tex-font-style-tt">Venus</span>, take a loan on 74 units of money and buy three items of the first type and 7 items of the third type (<span class="tex-span">3·6 + 7·8 = 74</span>). Then the ranger should fly to planet <span class="tex-font-style-tt">Earth</span> and sell there all the items he has bought. He gets <span class="tex-span">3·9 + 7·9 = 90</span> units of money for the items, he should give 74 of them for the loan. The resulting profit equals 16 units of money. We cannot get more profit in this case.</p>
