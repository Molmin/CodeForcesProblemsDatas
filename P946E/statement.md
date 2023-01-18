## Description

<div><p><span class="tex-font-style-it">Yes, that's another problem with definition of "beautiful" numbers</span>.</p><p>Let's call a positive integer <span class="tex-span"><i>x</i></span> <span class="tex-font-style-it">beautiful</span> if its decimal representation without leading zeroes contains even number of digits, and there exists a permutation of this representation which is palindromic. For example, <span class="tex-span">4242</span> is a beautiful number, since it contains <span class="tex-span">4</span> digits, and there exists a palindromic permutation <span class="tex-span">2442</span>.</p><p>Given a positive integer <span class="tex-span"><i>s</i></span>, find the largest beautiful number which is less than <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of testcases you have to solve.</p><p>Then <span class="tex-span"><i>t</i></span> lines follow, each representing one testcase and containing one string which is the decimal representation of number <span class="tex-span"><i>s</i></span>. It is guaranteed that this string has even length, contains no leading zeroes, and there exists at least one beautiful number less than <span class="tex-span"><i>s</i></span>.</p><p>The sum of lengths of <span class="tex-span"><i>s</i></span> over all testcases doesn't exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>For each testcase print one line containing the largest beautiful number which is less than <span class="tex-span"><i>s</i></span> (it is guaranteed that the answer exists).</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of testcases you have to solve.</p><p>Then <span class="tex-span"><i>t</i></span> lines follow, each representing one testcase and containing one string which is the decimal representation of number <span class="tex-span"><i>s</i></span>. It is guaranteed that this string has even length, contains no leading zeroes, and there exists at least one beautiful number less than <span class="tex-span"><i>s</i></span>.</p><p>The sum of lengths of <span class="tex-span"><i>s</i></span> over all testcases doesn't exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>For each testcase print one line containing the largest beautiful number which is less than <span class="tex-span"><i>s</i></span> (it is guaranteed that the answer exists).</p>





```input1
4
89
88
1000
28923845

```




```output1
88
77
99
28923839

```


