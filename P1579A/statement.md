## Description

<div><p>Casimir has a string $s$ which consists of capital Latin letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', and '<span class="tex-font-style-tt">C</span>' only. Each turn he can choose to do one of the two following actions:</p><ul> <li> he can either erase exactly one letter '<span class="tex-font-style-tt">A</span>' <span class="tex-font-style-bf">and</span> exactly one letter '<span class="tex-font-style-tt">B</span>' from arbitrary places of the string (these letters don't have to be adjacent); </li><li> or he can erase exactly one letter '<span class="tex-font-style-tt">B</span>' <span class="tex-font-style-bf">and</span> exactly one letter '<span class="tex-font-style-tt">C</span>' from arbitrary places in the string (these letters don't have to be adjacent). </li></ul><p>Therefore, each turn the length of the string is decreased exactly by $2$. All turns are independent so for each turn, Casimir can choose any of two possible actions.</p><p>For example, with $s$&nbsp;$=$&nbsp;"<span class="tex-font-style-tt">ABCABC</span>" he can obtain a string $s$&nbsp;$=$&nbsp;"<span class="tex-font-style-tt">ACBC</span>" in one turn (by erasing the first occurrence of '<span class="tex-font-style-tt">B</span>' and the second occurrence of '<span class="tex-font-style-tt">A</span>'). There are also many other options for a turn aside from this particular example.</p><p>For a given string $s$ determine whether there is a sequence of actions leading to an empty string. In other words, Casimir's goal is to erase all letters from the string. Is there a way to do this?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case is described by one string $s$, for which you need to determine if it can be fully erased by some sequence of turns. The string $s$ consists of capital letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">C</span>' and has a length from $1$ to $50$ letters, inclusive.</p></div><div class="output-specification"><p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should be <span class="tex-font-style-tt">YES</span> if there is a way to fully erase the corresponding string and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answers).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case is described by one string $s$, for which you need to determine if it can be fully erased by some sequence of turns. The string $s$ consists of capital letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">C</span>' and has a length from $1$ to $50$ letters, inclusive.</p>

## Output

<p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should be <span class="tex-font-style-tt">YES</span> if there is a way to fully erase the corresponding string and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answers).</p>





```input1
6
ABACAB
ABBA
AC
ABC
CABCBB
BCBCBCBCBCBCBCBC
```




```output1
NO
YES
NO
NO
YES
YES
```


