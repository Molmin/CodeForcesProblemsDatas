## Description

<div><p>George is a cat, so he loves playing very much.</p><p>Vitaly put <span class="tex-span"><i>n</i></span> cards in a row in front of George. Each card has one integer written on it. All cards had distinct numbers written on them. Let's number the cards from the left to the right with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Then the <span class="tex-span"><i>i</i></span>-th card from the left contains number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). </p><p>Vitaly wants the row to have exactly <span class="tex-span"><i>k</i></span> cards left. He also wants the <span class="tex-span"><i>i</i></span>-th card from left to have number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> written on it. Vitaly gave a task to George, to get the required sequence of cards using the remove operation <span class="tex-span"><i>n</i> - <i>k</i></span> times.</p><p>In one <span class="tex-font-style-it">remove operation</span> George can choose <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>w</i></span>; <span class="tex-span"><i>w</i></span> is not greater than the current number of cards in the row) contiguous cards (contiguous subsegment of cards). Let's denote the numbers written on these card as <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>w</i></sub></span> (from the left to the right). After that, George can remove the card <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, such that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i><sub class="lower-index"><i>j</i></sub></span> for each <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>j</i> ≤ <i>w</i>)</span>. After the described operation George gets <span class="tex-span"><i>w</i></span> pieces of sausage.</p><p>George wondered: what maximum number of pieces of sausage will he get in total if he reaches his goal and acts optimally well? Help George, find an answer to his question!</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the initial and the final number of cards.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the initial row of cards. </p><p>The third line contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> — the row of cards that you need to get. It is guaranteed that it's possible to obtain the given row by using the remove operation for <span class="tex-span"><i>n</i> - <i>k</i></span> times.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of pieces of sausage that George can get if he acts optimally well.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the initial and the final number of cards.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the initial row of cards. </p><p>The third line contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> — the row of cards that you need to get. It is guaranteed that it's possible to obtain the given row by using the remove operation for <span class="tex-span"><i>n</i> - <i>k</i></span> times.</p>

## Output

<p>Print a single integer — the maximum number of pieces of sausage that George can get if he acts optimally well.</p>





```input1
3 2
2 1 3
1 3

```




```input2
10 5
1 2 3 4 5 6 7 8 9 10
2 4 6 8 10

```




```output1
1

```




```output2
30

```


