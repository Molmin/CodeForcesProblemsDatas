## Description

<div><p>You desperately need to build some string <span class="tex-span"><i>t</i></span>. For that you've got <span class="tex-span"><i>n</i></span> more strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span>. To build string <span class="tex-span"><i>t</i></span>, you are allowed to perform exactly <span class="tex-span">|<i>t</i>|</span> (<span class="tex-span">|<i>t</i>|</span> is the length of string <span class="tex-span"><i>t</i></span>) operations on these strings. Each operation looks like that:</p><ol> <li> choose any non-empty string from strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span>; </li><li> choose an arbitrary character from the chosen string and write it on a piece of paper; </li><li> remove the chosen character from the chosen string. </li></ol><p>Note that after you perform the described operation, the total number of characters in strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> decreases by 1. We are assumed to build string <span class="tex-span"><i>t</i></span>, if the characters, written on the piece of paper, in the order of performed operations form string <span class="tex-span"><i>t</i></span>.</p><p>There are other limitations, though. For each string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> you know number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the maximum number of characters you are allowed to delete from string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. You also know that each operation that results in deleting a character from string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, costs <span class="tex-span"><i>i</i></span> rubles. That is, an operation on string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> is the cheapest (it costs <span class="tex-span">1</span> ruble), and the operation on string <span class="tex-span"><i>s</i><sub class="lower-index"><i>n</i></sub></span> is the most expensive one (it costs <span class="tex-span"><i>n</i></span> rubles).</p><p>Your task is to count the minimum amount of money (in rubles) you will need to build string <span class="tex-span"><i>t</i></span> by the given rules. Consider the cost of building string <span class="tex-span"><i>t</i></span> to be the sum of prices of the operations you use.</p></div><div class="input-specification"><p>The first line of the input contains string <span class="tex-span"><i>t</i></span> — the string that you need to build.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of strings to which you are allowed to apply the described operation. Each of the next <span class="tex-span"><i>n</i></span> lines contains a string and an integer. The <span class="tex-span"><i>i</i></span>-th line contains space-separated string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>. Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the maximum number of characters that can be deleted from string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>All strings in the input only consist of lowercase English letters. All strings are non-empty. The lengths of all strings do not exceed <span class="tex-span">100</span> characters.</p></div><div class="output-specification"><p>Print a single number — the minimum money (in rubles) you need in order to build string <span class="tex-span"><i>t</i></span>. If there is no solution, print -1.</p></div>

## Input

<p>The first line of the input contains string <span class="tex-span"><i>t</i></span> — the string that you need to build.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of strings to which you are allowed to apply the described operation. Each of the next <span class="tex-span"><i>n</i></span> lines contains a string and an integer. The <span class="tex-span"><i>i</i></span>-th line contains space-separated string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>. Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the maximum number of characters that can be deleted from string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>All strings in the input only consist of lowercase English letters. All strings are non-empty. The lengths of all strings do not exceed <span class="tex-span">100</span> characters.</p>

## Output

<p>Print a single number — the minimum money (in rubles) you need in order to build string <span class="tex-span"><i>t</i></span>. If there is no solution, print -1.</p>





```input1
bbaze
3
bzb 2
aeb 3
ba 10

```




```input2
abacaba
4
aba 2
bcc 1
caa 2
bbb 5

```




```input3
xyz
4
axx 8
za 1
efg 4
t 1

```




```output1
8

```




```output2
18

```




```output3
-1

```



## Note

<p>Notes to the samples:</p><p>In the first sample from the first string you should take characters "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">z</span>" with price <span class="tex-span">1</span> ruble, from the second string characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">e</span>" и "<span class="tex-font-style-tt">b</span>" with price <span class="tex-span">2</span> rubles. The price of the string <span class="tex-span"><i>t</i></span> in this case is <span class="tex-span">2·1 + 3·2 = 8</span>.</p><p>In the second sample from the first string you should take two characters "<span class="tex-font-style-tt">a</span>" with price <span class="tex-span">1</span> ruble, from the second string character "<span class="tex-font-style-tt">c</span>" with price <span class="tex-span">2</span> rubles, from the third string two characters "<span class="tex-font-style-tt">a</span>" with price <span class="tex-span">3</span> rubles, from the fourth string two characters "<span class="tex-font-style-tt">b</span>" with price <span class="tex-span">4</span> rubles. The price of the string <span class="tex-span"><i>t</i></span> in this case is <span class="tex-span">2·1 + 1·2 + 2·3 + 2·4 = 18</span>.</p><p>In the third sample the solution doesn't exist because there is no character "<span class="tex-font-style-tt">y</span>" in given strings.</p>
