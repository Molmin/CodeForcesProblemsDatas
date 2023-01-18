## Description

<div><p>On his trip to Luxor and Aswan, Sagheer went to a Nubian market to buy some souvenirs for his friends and relatives. The market has some strange rules. It contains <span class="tex-span"><i>n</i></span> different items numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th item has base cost <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> Egyptian pounds. If Sagheer buys <span class="tex-span"><i>k</i></span> items with indices <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span>, then the cost of item <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>j</i></sub></sub> + <i>x</i><sub class="lower-index"><i>j</i></sub>·<i>k</i></span> for <span class="tex-span">1 ≤ <i>j</i> ≤ <i>k</i></span>. In other words, the cost of an item is equal to its base cost in addition to its index multiplied by the factor <span class="tex-span"><i>k</i></span>.</p><p>Sagheer wants to buy as many souvenirs as possible without paying more than <span class="tex-span"><i>S</i></span> Egyptian pounds. Note that he cannot buy a souvenir more than once. If there are many ways to maximize the number of souvenirs, he will choose the way that will minimize the total cost. Can you help him with this task?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span> and <span class="tex-span">1 ≤ <i>S</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of souvenirs in the market and Sagheer's budget.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the base costs of the souvenirs.</p></div><div class="output-specification"><p>On a single line, print two integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>T</i></span>&nbsp;— the maximum number of souvenirs Sagheer can buy and the minimum total cost to buy these <span class="tex-span"><i>k</i></span> souvenirs.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span> and <span class="tex-span">1 ≤ <i>S</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of souvenirs in the market and Sagheer's budget.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the base costs of the souvenirs.</p>

## Output

<p>On a single line, print two integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>T</i></span>&nbsp;— the maximum number of souvenirs Sagheer can buy and the minimum total cost to buy these <span class="tex-span"><i>k</i></span> souvenirs.</p>





```input1
3 11
2 3 5

```




```input2
4 100
1 2 5 6

```




```input3
1 7
7

```




```output1
2 11

```




```output2
4 54

```




```output3
0 0

```



## Note

<p>In the first example, he cannot take the three items because they will cost him <span class="tex-span">[5, 9, 14]</span> with total cost <span class="tex-span">28</span>. If he decides to take only two items, then the costs will be <span class="tex-span">[4, 7, 11]</span>. So he can afford the first and second items.</p><p>In the second example, he can buy all items as they will cost him <span class="tex-span">[5, 10, 17, 22]</span>.</p><p>In the third example, there is only one souvenir in the market which will cost him <span class="tex-span">8</span> pounds, so he cannot buy it.</p>
