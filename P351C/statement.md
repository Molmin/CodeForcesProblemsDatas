## Description

<div><p>Jeff loves regular bracket sequences.</p><p>Today Jeff is going to take a piece of paper and write out the regular bracket sequence, consisting of <span class="tex-span"><i>nm</i></span> brackets. Let's number all brackets of this sequence from <span class="tex-span">0</span> to <span class="tex-span"><i>nm</i></span> - <span class="tex-span">1</span> from left to right. Jeff knows that he is going to spend <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> <i>mod</i> <i>n</i></sub></span> liters of ink on the <span class="tex-span"><i>i</i></span>-th bracket of the sequence if he paints it opened and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i> <i>mod</i> <i>n</i></sub></span> liters if he paints it closed.</p><p>You've got sequences <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>. What minimum amount of ink will Jeff need to paint a regular bracket sequence of length <span class="tex-span"><i>nm</i></span>?</p><p>Operation <span class="tex-span"><i>x</i> <i>mod</i> <i>y</i></span> means taking the remainder after dividing number <span class="tex-span"><i>x</i></span> by number <span class="tex-span"><i>y</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">7</sup>;</span> <span class="tex-span"><i>m</i></span> is even). The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>b</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10)</span>. The numbers are separated by spaces.</p></div><div class="output-specification"><p>In a single line print the answer to the problem — the minimum required amount of ink in liters.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">7</sup>;</span> <span class="tex-span"><i>m</i></span> is even). The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>b</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10)</span>. The numbers are separated by spaces.</p>

## Output

<p>In a single line print the answer to the problem — the minimum required amount of ink in liters.</p>





```input1
2 6
1 2
2 1

```




```input2
1 10000000
2
3

```




```output1
12

```




```output2
25000000

```



## Note

<p>In the first test the optimal sequence is: <span class="tex-span">()()()()()()</span>, the required number of ink liters is <span class="tex-span">12</span>.</p>
