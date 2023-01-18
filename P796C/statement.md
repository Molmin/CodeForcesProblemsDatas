## Description

<div><p>Although Inzane successfully found his beloved bone, Zane, his owner, has yet to return. To search for Zane, he would need a lot of money, of which he sadly has none. To deal with the problem, he has decided to hack the banks.</p><center> <img class="tex-graphics" src="file://xkFdHKSa.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are <span class="tex-span"><i>n</i></span> banks, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. There are also <span class="tex-span"><i>n</i> - 1</span> wires connecting the banks. All banks are initially <span class="tex-font-style-it">online</span>. Each bank also has its initial strength: bank <span class="tex-span"><i>i</i></span> has initial strength <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Let us define some keywords before we proceed. Bank <span class="tex-span"><i>i</i></span> and bank <span class="tex-span"><i>j</i></span> are <span class="tex-font-style-it">neighboring</span> if and only if there exists a wire directly connecting them. Bank <span class="tex-span"><i>i</i></span> and bank <span class="tex-span"><i>j</i></span> are <span class="tex-font-style-it">semi-neighboring</span> if and only if there exists an <span class="tex-font-style-bf"><span class="tex-font-style-it">online</span></span> bank <span class="tex-span"><i>k</i></span> such that bank <span class="tex-span"><i>i</i></span> and bank <span class="tex-span"><i>k</i></span> are <span class="tex-font-style-it">neighboring</span> and bank <span class="tex-span"><i>k</i></span> and bank <span class="tex-span"><i>j</i></span> are <span class="tex-font-style-it">neighboring</span>.</p><p>When a bank is hacked, it becomes <span class="tex-font-style-it">offline</span> (and no longer <span class="tex-font-style-it">online</span>), and other banks that are <span class="tex-font-style-it">neighboring</span> or <span class="tex-font-style-it">semi-neighboring</span> to it have their strengths increased by <span class="tex-span">1</span>.</p><p>To start his plan, Inzane will choose a bank to hack first. Indeed, the strength of such bank must not exceed the strength of his computer. After this, he will repeatedly choose some bank to hack next until all the banks are hacked, but he can continue to hack bank <span class="tex-span"><i>x</i></span> if and only if all these conditions are met:</p><ol> <li> Bank <span class="tex-span"><i>x</i></span> is <span class="tex-font-style-it">online</span>. That is, bank <span class="tex-span"><i>x</i></span> is not hacked yet. </li><li> Bank <span class="tex-span"><i>x</i></span> is <span class="tex-font-style-it">neighboring</span> to some <span class="tex-font-style-it">offline</span> bank. </li><li> The strength of bank <span class="tex-span"><i>x</i></span> is less than or equal to the strength of Inzane's computer. </li></ol><p>Determine the minimum strength of the computer Inzane needs to hack all the banks.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the total number of banks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the strengths of the banks.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— meaning that there is a wire directly connecting banks <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the wires connect the banks in such a way that Inzane can somehow hack all the banks using a computer with appropriate strength.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum strength of the computer Inzane needs to accomplish the goal.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the total number of banks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the strengths of the banks.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— meaning that there is a wire directly connecting banks <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the wires connect the banks in such a way that Inzane can somehow hack all the banks using a computer with appropriate strength.</p>

## Output

<p>Print one integer&nbsp;— the minimum strength of the computer Inzane needs to accomplish the goal.</p>





```input1
5
1 2 3 4 5
1 2
2 3
3 4
4 5

```




```input2
7
38 -29 87 93 39 28 -55
1 2
2 5
3 2
2 4
1 7
7 6

```




```input3
5
1 2 7 6 7
1 5
5 3
3 4
2 4

```




```output1
5
```




```output2
93
```




```output3
8
```



## Note

<p>In the first sample, Inzane can hack all banks using a computer with strength <span class="tex-span">5</span>. Here is how:</p><ul> <li> Initially, strengths of the banks are <span class="tex-span">[1, 2, 3, 4, 5]</span>. </li><li> He hacks bank <span class="tex-span">5</span>, then strengths of the banks become <span class="tex-span">[1, 2, 4, 5,  - ]</span>. </li><li> He hacks bank <span class="tex-span">4</span>, then strengths of the banks become <span class="tex-span">[1, 3, 5,  - ,  - ]</span>. </li><li> He hacks bank <span class="tex-span">3</span>, then strengths of the banks become <span class="tex-span">[2, 4,  - ,  - ,  - ]</span>. </li><li> He hacks bank <span class="tex-span">2</span>, then strengths of the banks become <span class="tex-span">[3,  - ,  - ,  - ,  - ]</span>. </li><li> He completes his goal by hacking bank <span class="tex-span">1</span>. </li></ul><p>In the second sample, Inzane can hack banks <span class="tex-span">4</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">1</span>, <span class="tex-span">5</span>, <span class="tex-span">7</span>, and <span class="tex-span">6</span>, in this order. This way, he can hack all banks using a computer with strength <span class="tex-span">93</span>.</p>
