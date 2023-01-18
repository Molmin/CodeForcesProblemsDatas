## Description

<div><p>Long ago, when Petya was a schoolboy, he was very much interested in the Petr# language grammar. During one lesson Petya got interested in the following question: how many different continuous substrings starting with the <span class="tex-span"><i>s</i><sub class="lower-index"><i>begin</i></sub></span> and ending with the <span class="tex-span"><i>s</i><sub class="lower-index"><i>end</i></sub></span> (it is possible <span class="tex-span"><i>s</i><sub class="lower-index"><i>begin</i></sub> = <i>s</i><sub class="lower-index"><i>end</i></sub></span>), the given string <span class="tex-span"><i>t</i></span> has. Substrings are different if and only if their contents aren't equal, their positions of occurence don't matter. Petya wasn't quite good at math, that's why he couldn't count this number. Help him!</p></div><div class="input-specification"><p>The input file consists of three lines. The first line contains string <span class="tex-span"><i>t</i></span>. The second and the third lines contain the <span class="tex-span"><i>s</i><sub class="lower-index"><i>begin</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>end</i></sub></span> identificators, correspondingly. All three lines are non-empty strings consisting of lowercase Latin letters. The length of each string doesn't exceed 2000 characters.</p></div><div class="output-specification"><p>Output the only number — the amount of different substrings of <span class="tex-span"><i>t</i></span> that start with <span class="tex-span"><i>s</i><sub class="lower-index"><i>begin</i></sub></span> and end with <span class="tex-span"><i>s</i><sub class="lower-index"><i>end</i></sub></span>.</p></div>

## Input

<p>The input file consists of three lines. The first line contains string <span class="tex-span"><i>t</i></span>. The second and the third lines contain the <span class="tex-span"><i>s</i><sub class="lower-index"><i>begin</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>end</i></sub></span> identificators, correspondingly. All three lines are non-empty strings consisting of lowercase Latin letters. The length of each string doesn't exceed 2000 characters.</p>

## Output

<p>Output the only number — the amount of different substrings of <span class="tex-span"><i>t</i></span> that start with <span class="tex-span"><i>s</i><sub class="lower-index"><i>begin</i></sub></span> and end with <span class="tex-span"><i>s</i><sub class="lower-index"><i>end</i></sub></span>.</p>





```input1
round
ro
ou

```




```input2
codeforces
code
forca

```




```input3
abababab
a
b

```




```input4
aba
ab
ba

```




```output1
1

```




```output2
0

```




```output3
4

```




```output4
1

```



## Note

<p>In the third sample there are four appropriate different substrings. They are: <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">abab</span>, <span class="tex-font-style-tt">ababab</span>, <span class="tex-font-style-tt">abababab</span>.</p><p>In the fourth sample identificators intersect.</p>
