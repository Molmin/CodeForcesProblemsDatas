## Description

<div><p>Recently, Mishka started noticing that his keyboard malfunctions — maybe it's because he was playing rhythm games too much. Empirically, Mishka has found out that every other time he presses a key, it is registered as if the key was pressed twice. For example, if Mishka types text, the first time he presses a key, exactly one letter is printed; the second time he presses a key, two same letters are printed; the third time he presses a key, one letter is printed; the fourth time he presses a key, two same letters are printed, and so on. Note that the number of times a key was pressed is counted for the whole keyboard, not for each key separately. For example, if Mishka tries to type the word <span class="tex-font-style-tt">osu</span>, it will be printed on the screen as <span class="tex-font-style-tt">ossu</span>.</p><p>You are given a word consisting of $n$ lowercase Latin letters. You have to determine if it can be printed on Mishka's keyboard or not. You may assume that Mishka cannot delete letters from the word, and every time he presses a key, the new letter (or letters) is appended to the end of the word.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 100$) — the length of the word.</p><p>The second line of the test case contains a string $s$ consisting of $n$ lowercase Latin letters — the word that should be checked.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if the word $s$ can be printed on Mishka's keyboard, and <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 100$) — the length of the word.</p><p>The second line of the test case contains a string $s$ consisting of $n$ lowercase Latin letters — the word that should be checked.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if the word $s$ can be printed on Mishka's keyboard, and <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1|2,3,6,7
4
4
ossu
2
aa
6
addonn
3
qwe
```




```output1
YES
NO
YES
NO
```



## Note

<p>In the first test case, Mishka can type the word as follows: press <span class="tex-font-style-tt">o</span> (one letter <span class="tex-font-style-tt">o</span> appears at the end of the word), then presses <span class="tex-font-style-tt">s</span> (two letters <span class="tex-font-style-tt">s</span> appear at the end of the word), and, finally, press <span class="tex-font-style-tt">u</span> (one letter appears at the end of the word, making the resulting word <span class="tex-font-style-tt">ossu</span>).</p><p>In the second test case, Mishka can try typing the word as follows: press <span class="tex-font-style-tt">a</span> (one letter <span class="tex-font-style-tt">a</span> appears at the end of the word). But if he tries to press <span class="tex-font-style-tt">a</span> one more time, two letters <span class="tex-font-style-tt">a</span> will appear at the end of the word, so it is impossible to print the word using his keyboard.</p><p>In the fourth test case, Mishka has to start by pressing <span class="tex-font-style-tt">q</span>. Then, if he presses <span class="tex-font-style-tt">w</span>, two copies of <span class="tex-font-style-tt">w</span> will appear at the end of the word, but the third letter should be <span class="tex-font-style-tt">e</span> instead of <span class="tex-font-style-tt">w</span>, so the answer is <span class="tex-font-style-tt">NO</span>.</p>
