## Description

<div><p>Polycarpus has <span class="tex-span"><i>n</i></span> friends in Tarasov city. Polycarpus knows phone numbers of all his friends: they are strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span>. All these strings consist only of digits and have the same length. </p><p>Once Polycarpus needed to figure out Tarasov city phone code. He assumed that the phone code of the city is the longest common prefix of all phone numbers of his friends. In other words, it is the longest string <span class="tex-span"><i>c</i></span> which is a prefix (the beginning) of each <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). Help Polycarpus determine the length of the city phone code. </p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">4</sup></span>) — the number of Polycarpus's friends. The following <span class="tex-span"><i>n</i></span> lines contain strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> — the phone numbers of Polycarpus's friends. It is guaranteed that all strings consist only of digits and have the same length from <span class="tex-span">1</span> to <span class="tex-span">20</span>, inclusive. It is also guaranteed that all strings are different.</p></div><div class="output-specification"><p>Print the number of digits in the city phone code.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">4</sup></span>) — the number of Polycarpus's friends. The following <span class="tex-span"><i>n</i></span> lines contain strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> — the phone numbers of Polycarpus's friends. It is guaranteed that all strings consist only of digits and have the same length from <span class="tex-span">1</span> to <span class="tex-span">20</span>, inclusive. It is also guaranteed that all strings are different.</p>

## Output

<p>Print the number of digits in the city phone code.</p>





```input1
4
00209
00219
00999
00909

```




```input2
2
1
2

```




```input3
3
77012345678999999999
77012345678901234567
77012345678998765432

```




```output1
2

```




```output2
0

```




```output3
12

```



## Note

<p>A <span class="tex-font-style-underline">prefix</span> of string <span class="tex-span"><i>t</i></span> is a string that is obtained by deleting zero or more digits from the end of string <span class="tex-span"><i>t</i></span>. For example, string "<span class="tex-font-style-tt">00209</span>" has 6 prefixes: "" (an empty prefix), "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">00</span>", "<span class="tex-font-style-tt">002</span>", "<span class="tex-font-style-tt">0020</span>", "<span class="tex-font-style-tt">00209</span>".</p><p>In the first sample the city phone code is string "<span class="tex-font-style-tt">00</span>".</p><p>In the second sample the city phone code is an empty string.</p><p>In the third sample the city phone code is string "<span class="tex-font-style-tt">770123456789</span>".</p>
