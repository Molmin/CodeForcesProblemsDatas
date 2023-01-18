## Description

<div><p>Let's consider one interesting word game. In this game you should transform one word into another through special operations. </p><p>Let's say we have word <span class="tex-span"><i>w</i></span>, let's split this word into two non-empty parts <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> so, that <span class="tex-span"><i>w</i> = <i>xy</i></span>. A <span class="tex-font-style-it">split</span> operation is transforming word <span class="tex-span"><i>w</i> = <i>xy</i></span> into word <span class="tex-span"><i>u</i> = <i>yx</i></span>. For example, a <span class="tex-font-style-it">split</span> operation can transform word "<span class="tex-font-style-tt">wordcut</span>" into word "<span class="tex-font-style-tt">cutword</span>".</p><p>You are given two words <span class="tex-span"><i>start</i></span> and <span class="tex-span"><i>end</i></span>. Count in how many ways we can transform word <span class="tex-span"><i>start</i></span> into word <span class="tex-span"><i>end</i></span>, if we apply exactly <span class="tex-span"><i>k</i></span> <span class="tex-font-style-it">split</span> operations consecutively to word <span class="tex-span"><i>start</i></span>. </p><p>Two ways are considered different if the sequences of applied operations differ. Two operation sequences are different if exists such number <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>), that in the <span class="tex-span"><i>i</i></span>-th operation of the first sequence the word splits into parts <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, in the <span class="tex-span"><i>i</i></span>-th operation of the second sequence the word splits into parts <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, and additionally <span class="tex-span"><i>x</i> ≠ <i>a</i></span> holds.</p></div><div class="input-specification"><p>The first line contains a non-empty word <span class="tex-span"><i>start</i></span>, the second line contains a non-empty word <span class="tex-span"><i>end</i></span>. The words consist of lowercase Latin letters. The number of letters in word <span class="tex-span"><i>start</i></span> equals the number of letters in word <span class="tex-span"><i>end</i></span> and is at least <span class="tex-span">2</span> and doesn't exceed <span class="tex-span">1000</span> letters.</p><p>The third line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the required number of operations.</p></div><div class="output-specification"><p>Print a single number — the answer to the problem. As this number can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a non-empty word <span class="tex-span"><i>start</i></span>, the second line contains a non-empty word <span class="tex-span"><i>end</i></span>. The words consist of lowercase Latin letters. The number of letters in word <span class="tex-span"><i>start</i></span> equals the number of letters in word <span class="tex-span"><i>end</i></span> and is at least <span class="tex-span">2</span> and doesn't exceed <span class="tex-span">1000</span> letters.</p><p>The third line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the required number of operations.</p>

## Output

<p>Print a single number — the answer to the problem. As this number can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
ab
ab
2

```




```input2
ababab
ababab
1

```




```input3
ab
ba
2

```




```output1
1

```




```output2
2

```




```output3
0

```



## Note

<p>The sought way in the first sample is:</p><p><span class="tex-font-style-tt">ab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">a|b</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">ba</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">b|a</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">ab</span></p><p>In the second sample the two sought ways are:</p><ul><li> <span class="tex-font-style-tt">ababab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">abab|ab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">ababab</span> </li><li> <span class="tex-font-style-tt">ababab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">ab|abab</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">ababab</span></li></ul>
