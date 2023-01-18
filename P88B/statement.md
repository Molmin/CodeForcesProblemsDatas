## Description

<div><p>Vasya learns to type. He has an unusual keyboard at his disposal: it is rectangular and it has <span class="tex-span"><i>n</i></span> rows of keys containing <span class="tex-span"><i>m</i></span> keys in each row. Besides, the keys are of two types. Some of the keys have lowercase Latin letters on them and some of the keys work like the "Shift" key on standard keyboards, that is, they make lowercase letters uppercase.</p><p>Vasya can press one or two keys with one hand. However, he can only press two keys if the Euclidean distance between the centers of the keys does not exceed <span class="tex-span"><i>x</i></span>. The keys are considered as squares with a side equal to 1. There are no empty spaces between neighbouring keys.</p><p>Vasya is a very lazy boy, that's why he tries to type with one hand as he eats chips with his other one. However, it is possible that some symbol can't be typed with one hand only, because the distance between it and the closest "Shift" key is strictly larger than <span class="tex-span"><i>x</i></span>. In this case he will have to use his other hand. Having typed the symbol, Vasya returns other hand back to the chips.</p><p>You are given Vasya's keyboard and the text. Count the minimum number of times Vasya will have to use the other hand.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30, 1 ≤ <i>x</i> ≤ 50</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain descriptions of all the keyboard keys. Each line contains the descriptions of exactly <span class="tex-span"><i>m</i></span> keys, without spaces. The letter keys are marked with the corresponding lowercase letters. The "Shift" keys are marked with the "<span class="tex-font-style-tt">S</span>" symbol. </p><p>Then follow the length of the text <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>. The last line contains the text <span class="tex-span"><i>T</i></span>, which consists of <span class="tex-span"><i>q</i></span> symbols, which are uppercase and lowercase Latin letters.</p></div><div class="output-specification"><p>If Vasya can type the text, then print the minimum number of times he will have to use his other hand. Otherwise, print "-1" (without the quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30, 1 ≤ <i>x</i> ≤ 50</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain descriptions of all the keyboard keys. Each line contains the descriptions of exactly <span class="tex-span"><i>m</i></span> keys, without spaces. The letter keys are marked with the corresponding lowercase letters. The "Shift" keys are marked with the "<span class="tex-font-style-tt">S</span>" symbol. </p><p>Then follow the length of the text <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>. The last line contains the text <span class="tex-span"><i>T</i></span>, which consists of <span class="tex-span"><i>q</i></span> symbols, which are uppercase and lowercase Latin letters.</p>

## Output

<p>If Vasya can type the text, then print the minimum number of times he will have to use his other hand. Otherwise, print "-1" (without the quotes).</p>





```input1
2 2 1
ab
cd
1
A

```




```input2
2 2 1
ab
cd
1
e

```




```input3
2 2 1
ab
cS
5
abcBA

```




```input4
3 9 4
qwertyuio
asdfghjkl
SzxcvbnmS
35
TheQuIcKbRoWnFOXjummsovertHeLazYDOG

```




```output1
-1

```




```output2
-1

```




```output3
1

```




```output4
2

```



## Note

<p>In the first sample the symbol "<span class="tex-font-style-tt">A</span>" is impossible to print as there's no "Shift" key on the keyboard.</p><p>In the second sample the symbol "<span class="tex-font-style-tt">e</span>" is impossible to print as there's no such key on the keyboard.</p><p>In the fourth sample the symbols "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">G</span>" are impossible to print with one hand. The other letters that are on the keyboard can be printed. Those symbols come up in the text twice, thus, the answer is 2.</p>
