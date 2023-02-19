## Description

<div><p>You are an experienced Codeforces user. Today you found out that during your activity on Codeforces you have made <span class="tex-span"><i>y</i></span> submissions, out of which <span class="tex-span"><i>x</i></span> have been successful. Thus, your current success rate on Codeforces is equal to <span class="tex-span"><i>x</i> / <i>y</i></span>.</p><p>Your favorite rational number in the <span class="tex-span">[0;1]</span> range is <span class="tex-span"><i>p</i> / <i>q</i></span>. Now you wonder: what is the smallest number of submissions you have to make if you want your success rate to be <span class="tex-span"><i>p</i> / <i>q</i></span>?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>)&nbsp;— the number of test cases.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains four integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">0 ≤ <i>p</i> ≤ <i>q</i> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span"><i>y</i> &gt; 0</span>; <span class="tex-span"><i>q</i> &gt; 0</span>).</p><p>It is guaranteed that <span class="tex-span"><i>p</i> / <i>q</i></span> is an irreducible fraction.</p><p><span class="tex-font-style-bf">Hacks.</span> For hacks, an additional constraint of <span class="tex-span"><i>t</i> ≤ 5</span> must be met.</p></div><div class="output-specification"><p>For each test case, output a single integer equal to the smallest number of submissions you have to make if you want your success rate to be equal to your favorite rational number, or <span class="tex-font-style-tt">-1</span> if this is impossible to achieve.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>)&nbsp;— the number of test cases.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains four integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">0 ≤ <i>p</i> ≤ <i>q</i> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span"><i>y</i> &gt; 0</span>; <span class="tex-span"><i>q</i> &gt; 0</span>).</p><p>It is guaranteed that <span class="tex-span"><i>p</i> / <i>q</i></span> is an irreducible fraction.</p><p><span class="tex-font-style-bf">Hacks.</span> For hacks, an additional constraint of <span class="tex-span"><i>t</i> ≤ 5</span> must be met.</p>

## Output

<p>For each test case, output a single integer equal to the smallest number of submissions you have to make if you want your success rate to be equal to your favorite rational number, or <span class="tex-font-style-tt">-1</span> if this is impossible to achieve.</p>





```input1
4
3 10 1 2
7 14 3 8
20 70 2 7
5 6 1 1

```




```output1
4
10
0
-1

```



## Note

<p>In the first example, you have to make 4 successful submissions. Your success rate will be equal to <span class="tex-span">7 / 14</span>, or <span class="tex-span">1 / 2</span>.</p><p>In the second example, you have to make 2 successful and 8 unsuccessful submissions. Your success rate will be equal to <span class="tex-span">9 / 24</span>, or <span class="tex-span">3 / 8</span>.</p><p>In the third example, there is no need to make any new submissions. Your success rate is already equal to <span class="tex-span">20 / 70</span>, or <span class="tex-span">2 / 7</span>.</p><p>In the fourth example, the only unsuccessful submission breaks your hopes of having the success rate equal to 1.</p>
