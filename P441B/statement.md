## Description

<div><p>Valera loves his garden, where <span class="tex-span"><i>n</i></span> fruit trees grow.</p><p>This year he will enjoy a great harvest! On the <span class="tex-span"><i>i</i></span>-th tree <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> fruit grow, they will ripen on a day number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Unfortunately, the fruit on the tree get withered, so they can only be collected on day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + 1</span> (all fruits that are not collected in these two days, become unfit to eat).</p><p>Valera is not very fast, but there are some positive points. Valera is ready to work every day. In one day, Valera can collect no more than <span class="tex-span"><i>v</i></span> fruits. The fruits may be either from the same tree, or from different ones. What is the maximum amount of fruit Valera can collect for all time, if he operates optimally well?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>v</i> ≤ 3000)</span> — the number of fruit trees in the garden and the number of fruits that Valera can collect in a day. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of trees in the garden. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 3000)</span> — the day the fruits ripen on the <span class="tex-span"><i>i</i></span>-th tree and the number of fruits on the <span class="tex-span"><i>i</i></span>-th tree.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of fruit that Valera can collect. </p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>v</i> ≤ 3000)</span> — the number of fruit trees in the garden and the number of fruits that Valera can collect in a day. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of trees in the garden. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 3000)</span> — the day the fruits ripen on the <span class="tex-span"><i>i</i></span>-th tree and the number of fruits on the <span class="tex-span"><i>i</i></span>-th tree.</p>

## Output

<p>Print a single integer — the maximum number of fruit that Valera can collect. </p>





```input1
2 3
1 5
2 3

```




```input2
5 10
3 20
2 20
1 20
4 20
5 20

```




```output1
8

```




```output2
60

```



## Note

<p>In the first sample, in order to obtain the optimal answer, you should act as follows. </p><ul> <li> On the first day collect <span class="tex-span">3</span> fruits from the <span class="tex-span">1</span>-st tree. </li><li> On the second day collect <span class="tex-span">1</span> fruit from the <span class="tex-span">2</span>-nd tree and <span class="tex-span">2</span> fruits from the <span class="tex-span">1</span>-st tree. </li><li> On the third day collect the remaining fruits from the <span class="tex-span">2</span>-nd tree. </li></ul> <p>In the second sample, you can only collect <span class="tex-span">60</span> fruits, the remaining fruit will simply wither.</p>
