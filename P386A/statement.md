## Description

<div><p>In this problem we consider a special type of an auction, which is called the second-price auction. As in regular auction <span class="tex-span"><i>n</i></span> bidders place a bid which is price a bidder ready to pay. The auction is closed, that is, each bidder secretly informs the organizer of the auction price he is willing to pay. After that, the auction winner is the participant who offered the highest price. However, he pay not the price he offers, but the highest price among the offers of other participants (hence the name: the second-price auction).</p><p>Write a program that reads prices offered by bidders and finds the winner and the price he will pay. Consider that all of the offered prices are different.</p></div><div class="input-specification"><p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — number of bidders. The second line contains <span class="tex-span"><i>n</i></span> distinct integer numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ... <i>p</i><sub class="lower-index"><i>n</i></sub></span>, separated by single spaces (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> stands for the price offered by the <span class="tex-span"><i>i</i></span>-th bidder.</p></div><div class="output-specification"><p>The single output line should contain two integers: index of the winner and the price he will pay. Indices are 1-based.</p></div>

## Input

<p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — number of bidders. The second line contains <span class="tex-span"><i>n</i></span> distinct integer numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ... <i>p</i><sub class="lower-index"><i>n</i></sub></span>, separated by single spaces (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> stands for the price offered by the <span class="tex-span"><i>i</i></span>-th bidder.</p>

## Output

<p>The single output line should contain two integers: index of the winner and the price he will pay. Indices are 1-based.</p>





```input1
2
5 7

```




```input2
3
10 2 8

```




```input3
6
3 8 2 9 4 14

```




```output1
2 5

```




```output2
1 8

```




```output3
6 9

```


