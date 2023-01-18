## Description

<div><p>Bash likes playing with arrays. He has an array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> of <span class="tex-span"><i>n</i></span> integers. He likes to guess the greatest common divisor (gcd) of different segments of the array. Of course, sometimes the guess is not correct. However, Bash will be satisfied if his guess is <span class="tex-font-style-it">almost correct</span>.</p><p>Suppose he guesses that the gcd of the elements in the range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> of <span class="tex-span"><i>a</i></span> is <span class="tex-span"><i>x</i></span>. He considers the guess to be almost correct if he can change <span class="tex-font-style-bf">at most</span> one element in the segment such that the gcd of the segment is <span class="tex-span"><i>x</i></span> after making the change. Note that when he guesses, he doesn't actually change the array — he just wonders if the gcd of the segment can be made <span class="tex-span"><i>x</i></span>. Apart from this, he also sometimes makes changes to the array itself.</p><p>Since he can't figure it out himself, Bash wants you to tell him which of his guesses are almost correct. Formally, you have to process <span class="tex-span"><i>q</i></span> queries of one of the following forms:</p><ul> <li> <span class="tex-span">1 <i>l</i> <i>r</i> <i>x</i></span> — Bash guesses that the gcd of the range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> is <span class="tex-span"><i>x</i></span>. Report if this guess is almost correct. </li><li> <span class="tex-span">2 <i>i</i> <i>y</i></span> — Bash sets <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>y</i></span>. </li></ul><p><span class="tex-font-style-bf">Note:</span> The array is <span class="tex-span">1</span>-indexed.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) &nbsp;— the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— the elements of the array.</p><p>The third line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 4·10<sup class="upper-index">5</sup></span>) &nbsp;— the number of queries.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the queries and may have one of the following forms:</p><ul> <li> <span class="tex-span">1 <i>l</i> <i>r</i> <i>x</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>, 1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>). </li><li> <span class="tex-span">2 <i>i</i> <i>y</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup>)</span>. </li></ul><p>Guaranteed, that there is at least one query of first type.</p></div><div class="output-specification"><p>For each query of first type, output <span class="tex-font-style-tt">"YES"</span> (without quotes) if Bash's guess is almost correct and <span class="tex-font-style-tt">"NO"</span> (without quotes) otherwise.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) &nbsp;— the size of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) &nbsp;— the elements of the array.</p><p>The third line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 4·10<sup class="upper-index">5</sup></span>) &nbsp;— the number of queries.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the queries and may have one of the following forms:</p><ul> <li> <span class="tex-span">1 <i>l</i> <i>r</i> <i>x</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>, 1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>). </li><li> <span class="tex-span">2 <i>i</i> <i>y</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup>)</span>. </li></ul><p>Guaranteed, that there is at least one query of first type.</p>

## Output

<p>For each query of first type, output <span class="tex-font-style-tt">"YES"</span> (without quotes) if Bash's guess is almost correct and <span class="tex-font-style-tt">"NO"</span> (without quotes) otherwise.</p>





```input1
3
2 6 3
4
1 1 2 2
1 1 3 3
2 1 9
1 1 3 2

```




```input2
5
1 2 3 4 5
6
1 1 4 2
2 3 6
1 1 4 2
1 1 5 2
2 5 10
1 1 5 2

```




```output1
YES
YES
NO

```




```output2
NO
YES
NO
YES

```



## Note

<p>In the first sample, the array initially is <span class="tex-span">{2, 6, 3}</span>. </p><p>For query <span class="tex-span">1</span>, the first two numbers already have their gcd as <span class="tex-span">2</span>.</p><p>For query <span class="tex-span">2</span>, we can achieve a gcd of <span class="tex-span">3</span> by changing the first element of the array to <span class="tex-span">3</span>. Note that the changes made during queries of type <span class="tex-span">1</span> are temporary and do not get reflected in the array. </p><p>After query <span class="tex-span">3</span>, the array is now <span class="tex-span">{9, 6, 3}</span>.</p><p> For query <span class="tex-span">4</span>, no matter which element you change, you cannot get the gcd of the range to be <span class="tex-span">2</span>. </p>
