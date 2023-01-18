## Description

<div><p>Boy Valera likes strings. And even more he likes them, when they are identical. That's why in his spare time Valera plays the following game. He takes any two strings, consisting of lower case Latin letters, and tries to make them identical. According to the game rules, with each move Valera can change <span class="tex-font-style-bf">one</span> arbitrary character <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> in one of the strings into arbitrary character <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>, but he has to pay for every move a particular sum of money, equal to <span class="tex-span"><i>W</i><sub class="lower-index"><i>i</i></sub></span>. He is allowed to make as many moves as he needs. Since Valera is a very economical boy and never wastes his money, he asked you, an experienced programmer, to help him answer the question: what minimum amount of money should Valera have to get identical strings. </p></div><div class="input-specification"><p>The first input line contains two initial non-empty strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, consisting of lower case Latin letters. The length of each string doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The following line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 500</span>)&nbsp;— amount of possible changings. Then follow <span class="tex-span"><i>n</i></span> lines, each containing characters <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> (lower case Latin letters) and integer <span class="tex-span"><i>W</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>W</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), saying that it's allowed to change character <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> into character <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> in any of the strings and spend sum of money <span class="tex-span"><i>W</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>If the answer exists, output the answer to the problem, and the resulting string. Otherwise output <span class="tex-font-style-tt">-1</span> in the only line. If the answer is not unique, output any.</p></div>

## Input

<p>The first input line contains two initial non-empty strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, consisting of lower case Latin letters. The length of each string doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The following line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 500</span>)&nbsp;— amount of possible changings. Then follow <span class="tex-span"><i>n</i></span> lines, each containing characters <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> (lower case Latin letters) and integer <span class="tex-span"><i>W</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>W</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), saying that it's allowed to change character <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> into character <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> in any of the strings and spend sum of money <span class="tex-span"><i>W</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>If the answer exists, output the answer to the problem, and the resulting string. Otherwise output <span class="tex-font-style-tt">-1</span> in the only line. If the answer is not unique, output any.</p>





```input1
uayd
uxxd
3
a x 8
x y 13
d c 3

```




```input2
a
b
3
a b 2
a b 3
b a 5

```




```input3
abc
ab
6
a b 4
a b 7
b a 8
c b 11
c a 3
a c 0

```




```output1
21
uxyd

```




```output2
2
b

```




```output3
-1

```


