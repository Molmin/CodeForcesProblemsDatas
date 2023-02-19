## Description

<div><p>In all schools in Buryatia, in the $1$ class, everyone is told the theory of Fibonacci strings.</p><p>"A <span class="tex-font-style-it">block</span> is a subsegment of a string where all the letters are the same and are bounded on the left and right by the ends of the string or by letters other than the letters in the block. A string is called a <span class="tex-font-style-it">Fibonacci</span> string if, when it is divided into blocks, their lengths in the order they appear in the string form the Fibonacci sequence ($f_0 = f_1 = 1$, $f_i = f_{i-2} + f_{i-1}$), starting from the zeroth member of this sequence. A string is called <span class="tex-font-style-it">semi-Fibonacci</span> if it possible to reorder its letters to get a <span class="tex-font-style-it">Fibonacci</span> string."</p><p>Burenka decided to enter the Buryat State University, but at the entrance exam she was given a difficult task. She was given a string consisting of the letters of the Buryat alphabet (which contains exactly $k$ letters), and was asked if the given string is <span class="tex-font-style-it">semi-Fibonacci</span>. The string can be very long, so instead of the string, she was given the number of appearances of each letter ($c_i$ for the $i$-th letter) in that string. Unfortunately, Burenka no longer remembers the theory of Fibonacci strings, so without your help she will not pass the exam.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The following is a description of the input data sets.</p><p>The first line of each test case contains one integer $k$ ($1 \leq k \leq 100$) — the number of letters in the alphabet.</p><p>The second line of each test case contains $k$ integers $c_1, c_2, \ldots, c_k$ ($1 \leq c_i \leq 10^9$) — the number of occurrences of each letter in the string.</p></div><div class="output-specification"><p>For each test case print the string "<span class="tex-font-style-tt">YES</span>" if the corresponding string is semi-Fibonacci, and "<span class="tex-font-style-tt">NO</span>" if it is not.</p><p>You can print "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The following is a description of the input data sets.</p><p>The first line of each test case contains one integer $k$ ($1 \leq k \leq 100$) — the number of letters in the alphabet.</p><p>The second line of each test case contains $k$ integers $c_1, c_2, \ldots, c_k$ ($1 \leq c_i \leq 10^9$) — the number of occurrences of each letter in the string.</p>

## Output

<p>For each test case print the string "<span class="tex-font-style-tt">YES</span>" if the corresponding string is semi-Fibonacci, and "<span class="tex-font-style-tt">NO</span>" if it is not.</p><p>You can print "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive answer).</p>





```input1|2,3,6,7,10,11
6
1
1
2
1 1
2
1 2
3
3 1 3
2
7 5
6
26 8 3 4 13 34
```




```output1
YES
YES
NO
YES
NO
YES
```



## Note

<p>In the first test case, a one-character string is semi-Fibonacci, being itself a Fibonacci string.</p><p>In the second test case, a string of two different characters is Fibonacci.</p><p>In the third test case, the string "<span class="tex-font-style-tt">abb</span>" (let the first of the alphabet letter be <span class="tex-font-style-tt">a</span>, the second letter <span class="tex-font-style-tt">b</span>) is not a semi-Fibonacci string, since no permutation of its letters ("<span class="tex-font-style-tt">abb</span>", "<span class="tex-font-style-tt">bab</span>", and "<span class="tex-font-style-tt">bba</span>") is a Fibonacci string.</p><p>In the fourth test case, two permutations of the letters of the string "<span class="tex-font-style-tt">abaccac</span>" (the first letter is <span class="tex-font-style-tt">a</span>, the second letter is <span class="tex-font-style-tt">b</span>, the third letter is <span class="tex-font-style-tt">c</span>) are Fibonacci strings — "<span class="tex-font-style-tt">abaaccc</span>" and "<span class="tex-font-style-tt">cbccaaa</span>".</p>
