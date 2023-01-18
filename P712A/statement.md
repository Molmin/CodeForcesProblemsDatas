## Description

<div><p>There are <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> written in a row. For all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are defined by the crows performing the following procedure:</p><ul> <li> The crow sets <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> initially <span class="tex-span">0</span>. </li><li> The crow then adds <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, subtracts <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i> + 1</sub></span>, adds the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i> + 2</sub></span> number, and so on until the <span class="tex-span"><i>n</i></span>'th number. Thus, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub> - <i>b</i><sub class="lower-index"><i>i</i> + 1</sub> + <i>b</i><sub class="lower-index"><i>i</i> + 2</sub> - <i>b</i><sub class="lower-index"><i>i</i> + 3</sub>...</span>. </li></ul><p>Memory gives you the values <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, and he now wants you to find the initial numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> written in the row? Can you do it?</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of integers written in the row.</p><p>The next line contains <span class="tex-span"><i>n</i></span>, the <span class="tex-span"><i>i</i></span>'th of which is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the value of the <span class="tex-span"><i>i</i></span>'th number.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers corresponding to the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. It's guaranteed that the answer is unique and fits in 32-bit integer type.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of integers written in the row.</p><p>The next line contains <span class="tex-span"><i>n</i></span>, the <span class="tex-span"><i>i</i></span>'th of which is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the value of the <span class="tex-span"><i>i</i></span>'th number.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers corresponding to the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. It's guaranteed that the answer is unique and fits in 32-bit integer type.</p>





```input1
5
6 -4 8 -2 3

```




```input2
5
3 -2 -1 5 6

```




```output1
2 4 6 1 3 

```




```output2
1 -3 4 11 6 

```



## Note

<p>In the first sample test, the crows report the numbers <span class="tex-span">6</span>,<span class="tex-span"> - 4</span>, <span class="tex-span">8</span>,<span class="tex-span"> - 2</span>, and <span class="tex-span">3</span> when he starts at indices <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span> respectively. It is easy to check that the sequence <span class="tex-span">2</span> <span class="tex-span">4</span> <span class="tex-span">6</span> <span class="tex-span">1</span> <span class="tex-span">3</span> satisfies the reports. For example, <span class="tex-span">6 = 2 - 4 + 6 - 1 + 3</span>, and <span class="tex-span"> - 4 = 4 - 6 + 1 - 3</span>.</p><p>In the second sample test, the sequence <span class="tex-span">1</span>, <span class="tex-span"> - 3</span>, <span class="tex-span">4</span>, <span class="tex-span">11</span>, <span class="tex-span">6</span> satisfies the reports. For example, <span class="tex-span">5 = 11 - 6</span> and <span class="tex-span">6 = 6</span>.</p>
