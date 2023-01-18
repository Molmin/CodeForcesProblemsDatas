## Description

<div><p>Santa Claus likes palindromes very much. There was his birthday recently. <span class="tex-span"><i>k</i></span> of his friends came to him to congratulate him, and each of them presented to him a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> having the same length <span class="tex-span"><i>n</i></span>. We denote the beauty of the <span class="tex-span"><i>i</i></span>-th string by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. It can happen that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is negative&nbsp;— that means that Santa doesn't find this string beautiful at all.</p><p>Santa Claus is crazy about palindromes. He is thinking about the following question: what is the maximum possible total beauty of a palindrome which can be obtained by concatenating some (possibly all) of the strings he has? Each present can be used at most once. Note that all strings have <span class="tex-font-style-bf">the same length</span> <span class="tex-span"><i>n</i></span>.</p><p>Recall that a palindrome is a string that doesn't change after one reverses it.</p><p>Since the empty string is a palindrome too, the answer can't be negative. Even if all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s are negative, Santa can obtain the empty string.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> divided by space and denoting the number of Santa friends and the length of every string they've presented, respectively (<span class="tex-span">1 ≤ <i>k</i>, <i>n</i> ≤ 100 000</span>; <span class="tex-span"><i>n</i>·<i>k</i>&nbsp; ≤ 100 000</span>).</p><p><span class="tex-span"><i>k</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and its beauty <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>). The string consists of <span class="tex-span"><i>n</i></span> lowercase English letters, and its beauty is integer. Some of strings may coincide. Also, equal strings can have different beauties.</p></div><div class="output-specification"><p>In the only line print the required maximum possible beauty.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> divided by space and denoting the number of Santa friends and the length of every string they've presented, respectively (<span class="tex-span">1 ≤ <i>k</i>, <i>n</i> ≤ 100 000</span>; <span class="tex-span"><i>n</i>·<i>k</i>&nbsp; ≤ 100 000</span>).</p><p><span class="tex-span"><i>k</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and its beauty <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>). The string consists of <span class="tex-span"><i>n</i></span> lowercase English letters, and its beauty is integer. Some of strings may coincide. Also, equal strings can have different beauties.</p>

## Output

<p>In the only line print the required maximum possible beauty.</p>





```input1
7 3
abb 2
aaa -3
bba -1
zyz -4
abb 5
aaa 7
xyx 4

```




```input2
3 1
a 1
a 2
a 3

```




```input3
2 5
abcde 10000
abcde 10000

```




```output1
12

```




```output2
6

```




```output3
0

```



## Note

<p>In the first example Santa can obtain <span class="tex-font-style-tt">abbaaaxyxaaabba</span> by concatenating strings <span class="tex-span">5</span>, <span class="tex-span">2</span>, <span class="tex-span">7</span>, <span class="tex-span">6</span> and <span class="tex-span">3</span> (in this order).</p>
