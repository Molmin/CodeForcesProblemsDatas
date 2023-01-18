## Description

<div><p>Vasya has a set of <span class="tex-span">4<i>n</i></span> strings of equal length, consisting of lowercase English letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">d</span>" and "<span class="tex-font-style-tt">e</span>". Moreover, the set is split into <span class="tex-span"><i>n</i></span> groups of <span class="tex-span">4</span> equal strings each. Vasya also has one special string <span class="tex-span"><i>a</i></span> of the same length, consisting of letters "<span class="tex-font-style-tt">a</span>" only.</p><p>Vasya wants to obtain from string <span class="tex-span"><i>a</i></span> some fixed string <span class="tex-span"><i>b</i></span>, in order to do this, he can use the strings from his set in any order. When he uses some string <span class="tex-span"><i>x</i></span>, each of the letters in string <span class="tex-span"><i>a</i></span> replaces with the next letter in alphabet as many times as the alphabet position, counting from zero, of the corresponding letter in string <span class="tex-span"><i>x</i></span>. Within this process the next letter in alphabet after "<span class="tex-font-style-tt">e</span>" is "<span class="tex-font-style-tt">a</span>".</p><p>For example, if some letter in <span class="tex-span"><i>a</i></span> equals "<span class="tex-font-style-tt">b</span>", and the letter on the same position in <span class="tex-span"><i>x</i></span> equals "<span class="tex-font-style-tt">c</span>", then the letter in <span class="tex-span"><i>a</i></span> becomes equal "<span class="tex-font-style-tt">d</span>", because "<span class="tex-font-style-tt">c</span>" is the second alphabet letter, counting from zero. If some letter in <span class="tex-span"><i>a</i></span> equals "<span class="tex-font-style-tt">e</span>", and on the same position in <span class="tex-span"><i>x</i></span> is "<span class="tex-font-style-tt">d</span>", then the letter in <span class="tex-span"><i>a</i></span> becomes "<span class="tex-font-style-tt">c</span>". For example, if the string <span class="tex-span"><i>a</i></span> equals "<span class="tex-font-style-tt">abcde</span>", and string <span class="tex-span"><i>x</i></span> equals "<span class="tex-font-style-tt">baddc</span>", then <span class="tex-span"><i>a</i></span> becomes "<span class="tex-font-style-tt">bbabb</span>".</p><p>A used string disappears, but Vasya can use equal strings several times.</p><p>Vasya wants to know for <span class="tex-span"><i>q</i></span> given strings <span class="tex-span"><i>b</i></span>, how many ways there are to obtain from the string <span class="tex-span"><i>a</i></span> string <span class="tex-span"><i>b</i></span> using the given set of <span class="tex-span">4<i>n</i></span> strings? Two ways are different if the number of strings used from some group of <span class="tex-span">4</span> strings is different. Help Vasya compute the answers for these questions modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>)&nbsp;— the number of groups of four strings in the set, and the length of all strings.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>m</i></span>, consisting of lowercase English letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">d</span>" and "<span class="tex-font-style-tt">e</span>". This means that there is a group of four strings equal to <span class="tex-span"><i>s</i></span>.</p><p>The next line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 300</span>)&nbsp;— the number of strings <span class="tex-span"><i>b</i></span> Vasya is interested in.</p><p>Each of the next <span class="tex-span"><i>q</i></span> strings contains a string <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>m</i></span>, consisting of lowercase English letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">d</span>" and "<span class="tex-font-style-tt">e</span>"&nbsp;— a string Vasya is interested in.</p></div><div class="output-specification"><p>For each string Vasya is interested in print the number of ways to obtain it from string <span class="tex-span"><i>a</i></span>, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>)&nbsp;— the number of groups of four strings in the set, and the length of all strings.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>m</i></span>, consisting of lowercase English letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">d</span>" and "<span class="tex-font-style-tt">e</span>". This means that there is a group of four strings equal to <span class="tex-span"><i>s</i></span>.</p><p>The next line contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 300</span>)&nbsp;— the number of strings <span class="tex-span"><i>b</i></span> Vasya is interested in.</p><p>Each of the next <span class="tex-span"><i>q</i></span> strings contains a string <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>m</i></span>, consisting of lowercase English letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">d</span>" and "<span class="tex-font-style-tt">e</span>"&nbsp;— a string Vasya is interested in.</p>

## Output

<p>For each string Vasya is interested in print the number of ways to obtain it from string <span class="tex-span"><i>a</i></span>, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1 1
b
2
a
e

```




```input2
2 4
aaaa
bbbb
1
cccc

```




```output1
1
1

```




```output2
5

```



## Note

<p>In the first example, we have <span class="tex-span">4</span> strings "<span class="tex-font-style-tt">b</span>". Then we have the only way for each string <span class="tex-span"><i>b</i></span>: select <span class="tex-span">0</span> strings "<span class="tex-font-style-tt">b</span>" to get "<span class="tex-font-style-tt">a</span>" and select <span class="tex-span">4</span> strings "<span class="tex-font-style-tt">b</span>" to get "<span class="tex-font-style-tt">e</span>", respectively. So, we have <span class="tex-span">1</span> way for each request.</p><p>In the second example, note that the choice of the string "<span class="tex-font-style-tt">aaaa</span>" does not change anything, that is we can choose any amount of it (from <span class="tex-span">0</span> to <span class="tex-span">4</span>, it's <span class="tex-span">5</span> different ways) and we have to select the line "<span class="tex-font-style-tt">bbbb</span>" <span class="tex-span">2</span> times, since other variants do not fit. We get that we have <span class="tex-span">5</span> ways for the request.</p>
