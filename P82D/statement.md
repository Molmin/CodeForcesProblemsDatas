## Description

<div><p>Vasya has recently developed a new algorithm to optimize the reception of customer flow and he considered the following problem.</p><p>Let the queue to the cashier contain <span class="tex-span"><i>n</i></span> people, at that each of them is characterized by a positive integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — that is the time needed to work with this customer. What is special about this very cashier is that it can serve two customers simultaneously. However, if two customers need <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> of time to be served, the time needed to work with both of them customers is equal to <span class="tex-span"><i>max</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub>)</span>. Please note that working with customers is an uninterruptable process, and therefore, if two people simultaneously come to the cashier, it means that they begin to be served simultaneously, and will both finish simultaneously (it is possible that one of them will have to wait).</p><p>Vasya used in his algorithm an ingenious heuristic — as long as the queue has more than one person waiting, then <span class="tex-font-style-it">some two people of the first three standing in front of the queue are sent simultaneously</span>. If the queue has only one customer number <span class="tex-span"><i>i</i></span>, then he goes to the cashier, and is served within <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of time. Note that the total number of phases of serving a customer will always be equal to <span class="tex-span">⌈<i>n</i> / 2⌉</span>.</p><p>Vasya thinks that this method will help to cope with the queues we all hate. That's why he asked you to work out a program that will determine the minimum time during which the whole queue will be served using this algorithm.</p></div><div class="input-specification"><p>The first line of the input file contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>), which is the number of people in the sequence. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). The people are numbered starting from the cashier to the end of the queue.</p></div><div class="output-specification"><p>Print on the first line a single number — the minimum time needed to process all <span class="tex-span"><i>n</i></span> people. Then on <span class="tex-span">⌈<i>n</i> / 2⌉</span> lines print the order in which customers will be served. Each line (probably, except for the last one) must contain two numbers separated by a space — the numbers of customers who will be served at the current stage of processing. If <span class="tex-span"><i>n</i></span> is odd, then the last line must contain a single number — the number of the last served customer in the queue. The customers are numbered starting from <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line of the input file contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>), which is the number of people in the sequence. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). The people are numbered starting from the cashier to the end of the queue.</p>

## Output

<p>Print on the first line a single number — the minimum time needed to process all <span class="tex-span"><i>n</i></span> people. Then on <span class="tex-span">⌈<i>n</i> / 2⌉</span> lines print the order in which customers will be served. Each line (probably, except for the last one) must contain two numbers separated by a space — the numbers of customers who will be served at the current stage of processing. If <span class="tex-span"><i>n</i></span> is odd, then the last line must contain a single number — the number of the last served customer in the queue. The customers are numbered starting from <span class="tex-span">1</span>.</p>





```input1
4
1 2 3 4

```




```input2
5
2 4 3 1 4

```




```output1
6
1 2
3 4

```




```output2
8
1 3
2 5
4

```


