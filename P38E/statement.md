## Description

<div><p>On a number axis directed from the left rightwards, <span class="tex-span"><i>n</i></span> marbles with coordinates <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> are situated. Let's assume that the sizes of the marbles are infinitely small, that is in this task each of them is assumed to be a material point. You can stick pins in some of them and the cost of sticking in the marble number <span class="tex-span"><i>i</i></span> is equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> may be negative. After you choose and stick the pins you need, the marbles will start to roll left according to the rule: if a marble has a pin stuck in it, then the marble doesn't move, otherwise the marble rolls all the way up to the next marble which has a pin stuck in it and stops moving there. If there is no pinned marble on the left to the given unpinned one, it is concluded that the marble rolls to the left to infinity and you will pay an infinitely large fine for it. If no marble rolled infinitely to the left, then the fine will consist of two summands: </p><ul> <li> the sum of the costs of stuck pins; </li><li> the sum of the lengths of the paths of each of the marbles, that is the sum of absolute values of differences between their initial and final positions. </li></ul><p>Your task is to choose and pin some marbles in the way that will make the fine for you to pay as little as possible.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>) which is the number of marbles. The next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the marbles in pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The numbers are space-separated. Each description is given on a separate line. No two marbles have identical initial positions.</p></div><div class="output-specification"><p>Output the single number — the least fine you will have to pay.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>) which is the number of marbles. The next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the marbles in pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The numbers are space-separated. Each description is given on a separate line. No two marbles have identical initial positions.</p>

## Output

<p>Output the single number — the least fine you will have to pay.</p>





```input1
3
2 3
3 4
1 2

```




```input2
4
1 7
3 1
5 10
6 1

```




```output1
5

```




```output2
11

```


