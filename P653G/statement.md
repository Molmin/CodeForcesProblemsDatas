## Description

<div><p>Pussycat Sonya has an array consisting of <span class="tex-span"><i>n</i></span> positive integers. There are <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> possible subsequences of the array. For each subsequence she counts the minimum number of operations to make all its elements equal. Each operation must be one of two:</p><ul> <li> Choose some element of the subsequence and multiply it by some prime number. </li><li> Choose some element of the subsequence and divide it by some prime number. The chosen element must be divisible by the chosen prime number. </li></ul><p>What is the sum of minimum number of operations for all <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> possible subsequences? Find and print this sum modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 300 000</span>)&nbsp;— elements of the array.</p></div><div class="output-specification"><p>Print the sum of minimum number of operation for all possible subsequences of the given array modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 300 000</span>)&nbsp;— elements of the array.</p>

## Output

<p>Print the sum of minimum number of operation for all possible subsequences of the given array modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
60 60 40

```




```input2
4
1 2 3 4

```




```output1
6

```




```output2
24

```



## Note

<p>In the first sample, there are <span class="tex-span">8</span> possible subsequences: <span class="tex-span">(60, 60, 40)</span>, <span class="tex-span">(60, 60)</span>, <span class="tex-span">(60, 40)</span>, <span class="tex-span">(60, 40)</span>, <span class="tex-span">(60)</span>, <span class="tex-span">(60)</span>, <span class="tex-span">(40)</span> and <span class="tex-span">()</span> (empty subsequence).</p><p>For a subsequence <span class="tex-span">(60, 60, 40)</span> we can make all elements equal by two operations&nbsp;— divide <span class="tex-span">40</span> by <span class="tex-span">2</span> to get <span class="tex-span">20</span>, and then multiply <span class="tex-span">20</span> by <span class="tex-span">3</span> to get <span class="tex-span">60</span>. It's impossible to achieve the goal using less operations and thus we add <span class="tex-span">2</span> to the answer.</p><p>There are two subsequences equal to <span class="tex-span">(60, 40)</span> and for each of them the also need to make at least <span class="tex-span">2</span> operations.</p><p>In each of other subsequences all numbers are already equal, so we need <span class="tex-span">0</span> operations for each of them. The sum is equal to <span class="tex-span">2 + 2 + 2 = 6</span>.</p>
