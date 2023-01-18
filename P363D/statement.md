## Description

<div><p>A group of <span class="tex-span"><i>n</i></span> schoolboys decided to ride bikes. As nobody of them has a bike, the boys need to rent them.</p><p>The renting site offered them <span class="tex-span"><i>m</i></span> bikes. The renting price is different for different bikes, renting the <span class="tex-span"><i>j</i></span>-th bike costs <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> rubles.</p><p>In total, the boys' shared budget is <span class="tex-span"><i>a</i></span> rubles. Besides, each of them has his own personal money, the <span class="tex-span"><i>i</i></span>-th boy has <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> personal rubles. The shared budget can be spent on any schoolchildren arbitrarily, but each boy's personal money can be spent on renting only this boy's bike.</p><p>Each boy can rent <span class="tex-font-style-it">at most one bike</span>, one cannot give his bike to somebody else.</p><p>What maximum number of schoolboys will be able to ride bikes? What minimum sum of personal money will they have to spend in total to let as many schoolchildren ride bikes as possible?</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains the sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the amount of the <span class="tex-span"><i>i</i></span>-th boy's personal money. The third line contains the sequence of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> is the price for renting the <span class="tex-span"><i>j</i></span>-th bike.</p></div><div class="output-specification"><p>Print two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>s</i></span>, where <span class="tex-span"><i>r</i></span> is the maximum number of schoolboys that can rent a bike and <span class="tex-span"><i>s</i></span> is the minimum total personal money needed to rent <span class="tex-span"><i>r</i></span> bikes. If the schoolchildren cannot rent any bikes, then <span class="tex-span"><i>r</i> = <i>s</i> = 0</span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains the sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the amount of the <span class="tex-span"><i>i</i></span>-th boy's personal money. The third line contains the sequence of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> is the price for renting the <span class="tex-span"><i>j</i></span>-th bike.</p>

## Output

<p>Print two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>s</i></span>, where <span class="tex-span"><i>r</i></span> is the maximum number of schoolboys that can rent a bike and <span class="tex-span"><i>s</i></span> is the minimum total personal money needed to rent <span class="tex-span"><i>r</i></span> bikes. If the schoolchildren cannot rent any bikes, then <span class="tex-span"><i>r</i> = <i>s</i> = 0</span>.</p>





```input1
2 2 10
5 5
7 6

```




```input2
4 5 2
8 1 1 2
6 3 7 5 2

```




```output1
2 3

```




```output2
3 8

```



## Note

<p>In the first sample both schoolchildren can rent a bike. For instance, they can split the shared budget in half (5 rubles each). In this case one of them will have to pay 1 ruble from the personal money and the other one will have to pay 2 rubles from the personal money. In total, they spend 3 rubles of their personal money. This way of distribution of money minimizes the amount of spent personal money.</p>
