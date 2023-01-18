## Description

<div><p>The Smart Beaver from ABBYY invented a new message encryption method and now wants to check its performance. Checking it manually is long and tiresome, so he decided to ask the ABBYY Cup contestants for help.</p><p>A message is a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Encryption uses a key which is a sequence of <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span"><i>m</i> ≤ <i>n</i></span>). All numbers from the message and from the key belong to the interval from <span class="tex-span">0</span> to <span class="tex-span"><i>c</i> - 1</span>, inclusive, and all the calculations are performed modulo <span class="tex-span"><i>c</i></span>.</p><p>Encryption is performed in <span class="tex-span"><i>n</i> - <i>m</i> + 1</span> steps. On the first step we add to each number <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> a corresponding number <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>. On the second step we add to each number <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i> + 1</sub></span> (changed on the previous step) a corresponding number <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>. And so on: on step number <span class="tex-span"><i>i</i></span> we add to each number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>i</i> + <i>m</i> - 1</sub></span> a corresponding number <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>. The result of the encryption is the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> after <span class="tex-span"><i>n</i> - <i>m</i> + 1</span> steps.</p><p>Help the Beaver to write a program that will encrypt messages in the described manner.</p></div><div class="input-specification"><p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>c</i></span>, separated by single spaces. </p><p>The second input line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>c</i></span>), separated by single spaces — the original message. </p><p>The third input line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>c</i></span>), separated by single spaces — the encryption key.</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span> </li><li> <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">3</sup></span> </li></ul> <p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">3</sup></span> </li></ul> </div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated integers — the result of encrypting the original message.</p></div>

## Input

<p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>c</i></span>, separated by single spaces. </p><p>The second input line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>c</i></span>), separated by single spaces — the original message. </p><p>The third input line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> &lt; <i>c</i></span>), separated by single spaces — the encryption key.</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span> </li><li> <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">3</sup></span> </li></ul> <p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">3</sup></span> </li></ul>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated integers — the result of encrypting the original message.</p>





```input1
4 3 2
1 1 1 1
1 1 1

```




```input2
3 1 5
1 2 3
4

```




```output1
0 1 1 0

```




```output2
0 1 2

```



## Note

<p>In the first sample the encryption is performed in two steps: after the first step <span class="tex-span"><i>a</i> = (0, 0, 0, 1)</span> (remember that the calculations are performed modulo 2), after the second step <span class="tex-span"><i>a</i> = (0, 1, 1, 0)</span>, and that is the answer. </p>
