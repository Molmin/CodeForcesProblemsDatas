## Description

<div><p>After observing the results of Spy Syndrome, Yash realised the errors of his ways. He now believes that a super spy such as Siddhant can't use a cipher as basic and ancient as Caesar cipher. After many weeks of observation of Siddhant’s sentences, Yash determined a new cipher technique.</p><p>For a given sentence, the cipher is processed as: </p><ol> <li> Convert all letters of the sentence to lowercase. </li><li> Reverse each of the words of the sentence individually. </li><li> Remove all the spaces in the sentence. </li></ol><p>For example, when this cipher is applied to the sentence</p><p><span class="tex-font-style-tt">Kira is childish and he hates losing</span></p><p>the resulting string is</p><p><span class="tex-font-style-tt">ariksihsidlihcdnaehsetahgnisol</span></p><p>Now Yash is given some ciphered string and a list of words. Help him to find out any original sentence composed using only words from the list. Note, that any of the given words could be used in the sentence multiple times.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>)&nbsp;— the length of the ciphered text. The second line consists of <span class="tex-span"><i>n</i></span> lowercase English letters&nbsp;— the ciphered text <span class="tex-span"><i>t</i></span>.</p><p>The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of words which will be considered while deciphering the text. Each of the next <span class="tex-span"><i>m</i></span> lines contains a non-empty word <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>w</i><sub class="lower-index"><i>i</i></sub>| ≤ 1 000</span>) consisting of uppercase and lowercase English letters only. It's guaranteed that the total length of all words doesn't exceed <span class="tex-span">1 000 000</span>.</p></div><div class="output-specification"><p>Print one line — the original sentence. It is guaranteed that at least one solution exists. If there are multiple solutions, you may output any of those.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>)&nbsp;— the length of the ciphered text. The second line consists of <span class="tex-span"><i>n</i></span> lowercase English letters&nbsp;— the ciphered text <span class="tex-span"><i>t</i></span>.</p><p>The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of words which will be considered while deciphering the text. Each of the next <span class="tex-span"><i>m</i></span> lines contains a non-empty word <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>w</i><sub class="lower-index"><i>i</i></sub>| ≤ 1 000</span>) consisting of uppercase and lowercase English letters only. It's guaranteed that the total length of all words doesn't exceed <span class="tex-span">1 000 000</span>.</p>

## Output

<p>Print one line — the original sentence. It is guaranteed that at least one solution exists. If there are multiple solutions, you may output any of those.</p>





```input1
30
ariksihsidlihcdnaehsetahgnisol
10
Kira
hates
is
he
losing
death
childish
L
and
Note

```




```input2
12
iherehtolleh
5
HI
Ho
there
HeLLo
hello

```




```output1
Kira is childish and he hates losing 

```




```output2
HI there HeLLo 

```



## Note

<p>In sample case 2 there may be multiple accepted outputs, "HI there HeLLo" and "HI there hello" you may output any of them. </p>
