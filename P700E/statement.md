## Description

<div><p>Bomboslav set up a branding agency and now helps companies to create new logos and advertising slogans. In term of this problems, <span class="tex-font-style-it">slogan</span> of the company should be a non-empty substring of its name. For example, if the company name is "<span class="tex-font-style-tt">hornsandhoofs</span>", then substrings "<span class="tex-font-style-tt">sand</span>" and "<span class="tex-font-style-tt">hor</span>" could be its slogans, while strings "<span class="tex-font-style-tt">e</span>" and "<span class="tex-font-style-tt">hornss</span>" can not.</p><p>Sometimes the company performs rebranding and changes its slogan. Slogan <span class="tex-span"><i>A</i></span> is considered to be <span class="tex-font-style-it">cooler</span> than slogan <span class="tex-span"><i>B</i></span> if <span class="tex-span"><i>B</i></span> appears in <span class="tex-span"><i>A</i></span> as a substring <span class="tex-font-style-bf">at least twice</span> (this occurrences are allowed to overlap). For example, slogan <span class="tex-span"><i>A</i> = </span> "<span class="tex-font-style-tt">abacaba</span>" is cooler than slogan <span class="tex-span"><i>B</i> = </span> "<span class="tex-font-style-tt">ba</span>", slogan <span class="tex-span"><i>A</i> = </span> "<span class="tex-font-style-tt">abcbcbe</span>" is cooler than slogan <span class="tex-span"><i>B</i> = </span> "<span class="tex-font-style-tt">bcb</span>", but slogan <span class="tex-span"><i>A</i> = </span> "<span class="tex-font-style-tt">aaaaaa</span>" is not cooler than slogan <span class="tex-span"><i>B</i> = </span> "<span class="tex-font-style-tt">aba</span>".</p><p>You are given the company name <span class="tex-span"><i>w</i></span> and your task is to help Bomboslav determine the length of the longest sequence of slogans <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>, such that any slogan in the sequence is cooler than the previous one.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the length of the company name that asks Bomboslav to help. The second line contains the string <span class="tex-span"><i>w</i></span> of length <span class="tex-span"><i>n</i></span>, that consists of lowercase English letters.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum possible length of the sequence of slogans of the company named <span class="tex-span"><i>w</i></span>, such that any slogan in the sequence (except the first one) is cooler than the previous</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the length of the company name that asks Bomboslav to help. The second line contains the string <span class="tex-span"><i>w</i></span> of length <span class="tex-span"><i>n</i></span>, that consists of lowercase English letters.</p>

## Output

<p>Print a single integer&nbsp;— the maximum possible length of the sequence of slogans of the company named <span class="tex-span"><i>w</i></span>, such that any slogan in the sequence (except the first one) is cooler than the previous</p>





```input1
3
abc

```




```input2
5
ddddd

```




```input3
11
abracadabra

```




```output1
1

```




```output2
5

```




```output3
3

```


