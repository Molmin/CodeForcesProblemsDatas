## Description

<div><p>Paul Erdős's prediction came true. Finally an alien force landed on the Earth. In contrary to our expectation they didn't asked the humans to compute the value of a Ramsey number (maybe they had solved it themselves). They asked another question which seemed as hard as calculating Ramsey numbers. Aliens threatened that if humans don't solve this problem in less than 2 hours they will destroy the Earth. </p><p>Before telling the problem they introduced the concept of Hyper Strings. A Hyper String is made by concatenation of some base strings. Suppose you are given a list of base strings <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. Now the Hyper String made from indices list <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>m</i></sub></span> is concatenation of base strings <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub>, <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub>, ..., <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>m</i></sub></sub></span>. A Hyper String can be very large and doing operations on it is very costly for computers. </p><p>The aliens asked humans to compute the length of the longest common sub-sequence of a Hyper String <span class="tex-span"><i>t</i></span> with a string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line of input contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of base strings. </p><p>The next <span class="tex-span"><i>n</i></span> lines contains values of base strings. Each base string is made of lowercase Latin letters. A base string cannot be empty string and the sum of lengths of all <span class="tex-span"><i>n</i></span> base strings doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. </p><p>The next line contains the single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2000</span>) — the number of base strings in the given Hyper String <span class="tex-span"><i>t</i></span>. </p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated integer numbers <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the indices of base strings in the Hyper String <span class="tex-span"><i>t</i></span>.</p><p>The last line contains a non-empty string <span class="tex-span"><i>s</i></span>. String <span class="tex-span"><i>s</i></span> is made of lowercase Latin letters and its length is no more than <span class="tex-span">2000</span> characters.</p></div><div class="output-specification"><p>Print the length of longest common sub-sequence of Hyper String <span class="tex-span"><i>t</i></span> and string <span class="tex-span"><i>s</i></span>. If there is no common sub-sequence print 0.</p></div>

## Input

<p>The first line of input contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of base strings. </p><p>The next <span class="tex-span"><i>n</i></span> lines contains values of base strings. Each base string is made of lowercase Latin letters. A base string cannot be empty string and the sum of lengths of all <span class="tex-span"><i>n</i></span> base strings doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. </p><p>The next line contains the single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2000</span>) — the number of base strings in the given Hyper String <span class="tex-span"><i>t</i></span>. </p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated integer numbers <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the indices of base strings in the Hyper String <span class="tex-span"><i>t</i></span>.</p><p>The last line contains a non-empty string <span class="tex-span"><i>s</i></span>. String <span class="tex-span"><i>s</i></span> is made of lowercase Latin letters and its length is no more than <span class="tex-span">2000</span> characters.</p>

## Output

<p>Print the length of longest common sub-sequence of Hyper String <span class="tex-span"><i>t</i></span> and string <span class="tex-span"><i>s</i></span>. If there is no common sub-sequence print 0.</p>





```input1
2
cba
dgh
2
1 2
aedfhr

```




```input2
2
b
a
5
1 2 1 2 1
aaa

```




```output1
3

```




```output2
2

```



## Note

<p>The <span class="tex-font-style-it">length</span> of string <span class="tex-span"><i>s</i></span> is the number of characters in it. If the length of string <span class="tex-span"><i>s</i></span> is marked as <span class="tex-span">|<i>s</i>|</span>, then string <span class="tex-span"><i>s</i></span> can be represented as <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span>.</p><p>A non-empty string <span class="tex-span"><i>y</i> = <i>s</i>[<i>p</i><sub class="lower-index">1</sub><i>p</i><sub class="lower-index">2</sub>... <i>p</i><sub class="lower-index">|<i>y</i>|</sub>] = <i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub><i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub>... <i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">|<i>y</i>|</sub></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index">|<i>y</i>|</sub> ≤ |<i>s</i>|</span>) is a <span class="tex-font-style-it">subsequence</span> of string <span class="tex-span"><i>s</i></span>. For example, "<span class="tex-font-style-tt">coders</span>" is a subsequence of "<span class="tex-font-style-tt">codeforces</span>".</p>
