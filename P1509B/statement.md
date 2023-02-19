## Description

<div><p>The student council has a shared document file. Every day, some members of the student council write the sequence <span class="tex-font-style-tt">TMT</span> (short for Towa Maji Tenshi) in it.</p><p>However, one day, the members somehow entered the sequence into the document at the same time, creating a jumbled mess. Therefore, it is Suguru Doujima's task to figure out whether the document has malfunctioned. Specifically, he is given a string of length $n$ whose characters are all either <span class="tex-font-style-tt">T</span> or <span class="tex-font-style-tt">M</span>, and he wants to figure out if it is possible to partition it into some number of disjoint subsequences, all of which are equal to <span class="tex-font-style-tt">TMT</span>. That is, each character of the string should belong to exactly one of the subsequences.</p><p>A string $a$ is a subsequence of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero) characters.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 5000$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($3 \le n &lt; 10^5$), the number of characters in the string entered in the document. It is guaranteed that $n$ is divisible by $3$.</p><p>The second line of each test case contains a string of length $n$ consisting of only the characters <span class="tex-font-style-tt">T</span> and <span class="tex-font-style-tt">M</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line containing <span class="tex-font-style-tt">YES</span> if the described partition exists, and a single line containing <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 5000$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($3 \le n &lt; 10^5$), the number of characters in the string entered in the document. It is guaranteed that $n$ is divisible by $3$.</p><p>The second line of each test case contains a string of length $n$ consisting of only the characters <span class="tex-font-style-tt">T</span> and <span class="tex-font-style-tt">M</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a single line containing <span class="tex-font-style-tt">YES</span> if the described partition exists, and a single line containing <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
5
3
TMT
3
MTT
6
TMTMTT
6
TMTTTT
6
TTMMTT
```




```output1
YES
NO
YES
NO
YES
```



## Note

<p>In the first test case, the string itself is already a sequence equal to <span class="tex-font-style-tt">TMT</span>.</p><p>In the third test case, we may partition the string into the subsequences <span class="tex-font-style-tt"><span class="tex-font-style-bf">TM</span>TMT<span class="tex-font-style-bf">T</span></span>. Both the bolded and the non-bolded subsequences are equal to <span class="tex-font-style-tt">TMT</span>.</p>
