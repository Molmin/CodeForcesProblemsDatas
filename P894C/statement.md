## Description

<div><p>In a dream Marco met an elderly man with a pair of black glasses. The man told him the key to immortality and then disappeared with the wind of time.</p><p>When he woke up, he only remembered that the key was a sequence of positive integers of some length <span class="tex-span"><i>n</i></span>, but forgot the exact sequence. Let the elements of the sequence be <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. He remembered that he calculated <span class="tex-span"><i>gcd</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>j</i></sub>)</span> for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span> and put it into a set <span class="tex-span"><i>S</i></span>. <span class="tex-span"><i>gcd</i></span> here means the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a>.</p><p>Note that even if a number is put into the set <span class="tex-span"><i>S</i></span> twice or more, it only appears once in the set.</p><p>Now Marco gives you the set <span class="tex-span"><i>S</i></span> and asks you to help him figure out the initial sequence. If there are many solutions, print any of them. It is also possible that there are no sequences that produce the set <span class="tex-span"><i>S</i></span>, in this case print <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>)&nbsp;— the size of the set <span class="tex-span"><i>S</i></span>.</p><p>The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the elements of the set <span class="tex-span"><i>S</i></span>. It's guaranteed that the elements of the set are given in strictly increasing order, that means <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> &lt; <i>s</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>s</i><sub class="lower-index"><i>m</i></sub></span>.</p></div><div class="output-specification"><p>If there is no solution, print a single line containing <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print a single integer <span class="tex-span"><i>n</i></span> denoting the length of the sequence, <span class="tex-span"><i>n</i></span> should not exceed <span class="tex-span">4000</span>.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the sequence.</p><p>We can show that if a solution exists, then there is a solution with <span class="tex-span"><i>n</i></span> not exceeding <span class="tex-span">4000</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> not exceeding <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>)&nbsp;— the size of the set <span class="tex-span"><i>S</i></span>.</p><p>The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the elements of the set <span class="tex-span"><i>S</i></span>. It's guaranteed that the elements of the set are given in strictly increasing order, that means <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> &lt; <i>s</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>s</i><sub class="lower-index"><i>m</i></sub></span>.</p>

## Output

<p>If there is no solution, print a single line containing <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print a single integer <span class="tex-span"><i>n</i></span> denoting the length of the sequence, <span class="tex-span"><i>n</i></span> should not exceed <span class="tex-span">4000</span>.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the sequence.</p><p>We can show that if a solution exists, then there is a solution with <span class="tex-span"><i>n</i></span> not exceeding <span class="tex-span">4000</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> not exceeding <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>If there are multiple solutions, print any of them.</p>





```input1
4
2 4 6 12

```




```input2
2
2 3

```




```output1
3
4 6 12
```




```output2
-1

```



## Note

<p>In the first example <span class="tex-span">2 = <i>gcd</i>(4, 6)</span>, the other elements from the set appear in the sequence, and we can show that there are no values different from <span class="tex-span">2</span>, <span class="tex-span">4</span>, <span class="tex-span">6</span> and <span class="tex-span">12</span> among <span class="tex-span"><i>gcd</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>j</i></sub>)</span> for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>.</p>
