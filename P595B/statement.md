## Description

<div><p>Pasha has recently bought a new phone <span class="tex-font-style-tt">jPager</span> and started adding his friends' phone numbers there. Each phone number consists of exactly <span class="tex-span"><i>n</i></span> digits.</p><p>Also Pasha has a number <span class="tex-span"><i>k</i></span> and two sequences of length <span class="tex-span"><i>n</i> / <i>k</i></span> (<span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>k</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> / <i>k</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> / <i>k</i></sub></span>. Let's split the phone number into blocks of length <span class="tex-span"><i>k</i></span>. The first block will be formed by digits from the phone number that are on positions <span class="tex-span">1</span>, <span class="tex-span">2</span>,..., <span class="tex-span"><i>k</i></span>, the second block will be formed by digits from the phone number that are on positions <span class="tex-span"><i>k</i> + 1</span>, <span class="tex-span"><i>k</i> + 2</span>, ..., <span class="tex-span">2·<i>k</i></span> and so on. Pasha considers a phone number <span class="tex-font-style-tt">good</span>, if the <span class="tex-span"><i>i</i></span>-th block doesn't start from the digit <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and is divisible by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> if represented as an integer. </p><p>To represent the block of length <span class="tex-span"><i>k</i></span> as an integer, let's write it out as a sequence <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>,...,<span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span>. Then the integer is calculated as the result of the expression <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>·10<sup class="upper-index"><i>k</i> - 1</sup> + <i>c</i><sub class="lower-index">2</sub>·10<sup class="upper-index"><i>k</i> - 2</sup> + ... + <i>c</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>Pasha asks you to calculate the number of <span class="tex-font-style-tt">good</span> phone numbers of length <span class="tex-span"><i>n</i></span>, for the given <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. As this number can be too big, print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 9)</span>)&nbsp;— the length of all phone numbers and the length of each block, respectively. It is guaranteed that <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>k</i></span>.</p><p>The second line of the input contains <span class="tex-span"><i>n</i> / <i>k</i></span> space-separated positive integers&nbsp;— sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> / <i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index"><i>k</i></sup></span>).</p><p>The third line of the input contains <span class="tex-span"><i>n</i> / <i>k</i></span> space-separated positive integers&nbsp;— sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> / <i>k</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>). </p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of good phone numbers of length <span class="tex-span"><i>n</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 9)</span>)&nbsp;— the length of all phone numbers and the length of each block, respectively. It is guaranteed that <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>k</i></span>.</p><p>The second line of the input contains <span class="tex-span"><i>n</i> / <i>k</i></span> space-separated positive integers&nbsp;— sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> / <i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index"><i>k</i></sup></span>).</p><p>The third line of the input contains <span class="tex-span"><i>n</i> / <i>k</i></span> space-separated positive integers&nbsp;— sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> / <i>k</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 9</span>). </p>

## Output

<p>Print a single integer&nbsp;— the number of good phone numbers of length <span class="tex-span"><i>n</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
6 2
38 56 49
7 3 4

```




```input2
8 2
1 22 3 44
5 4 3 2

```




```output1
8

```




```output2
32400

```



## Note

<p>In the first test sample <span class="tex-font-style-tt">good</span> phone numbers are: <span class="tex-font-style-tt">000000</span>, <span class="tex-font-style-tt">000098</span>, <span class="tex-font-style-tt">005600</span>, <span class="tex-font-style-tt">005698</span>, <span class="tex-font-style-tt">380000</span>, <span class="tex-font-style-tt">380098</span>, <span class="tex-font-style-tt">385600</span>, <span class="tex-font-style-tt">385698</span>.</p>
