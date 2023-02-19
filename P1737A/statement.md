## Description

<div><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left"><img class="tex-graphics" src="file://KejxWXvj.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-left"><span class="tex-font-style-it">Ela loves reading a lot, just like her new co-workers in DTL! On her first day after becoming an engineer in DTL, she is challenged by a co-worker to sort a heap of books into different compartments on the shelf.</span></td></tr></tbody></table><p></p><p>$n$ books must be split into $k$ compartments on the bookshelf ($n$ is divisible by $k$). Each book is represented by a lowercase Latin letter <span class="tex-font-style-bf">from <span class="tex-font-style-tt">'a'</span> to <span class="tex-font-style-tt">'y'</span></span> inclusively, which is the beginning letter in the title of the book.</p><p>Ela must stack <span class="tex-font-style-bf">exactly</span> $\frac{n}{k}$ books in each compartment. After the books are stacked, for each compartment indexed from $1$ to $k$, she takes the <span class="tex-font-style-bf">minimum excluded (MEX)</span> letter of the <span class="tex-font-style-it">multiset of letters</span> formed by letters representing all books in that compartment, then combines the resulting letters into a string. The first letter of the resulting string is the MEX letter of the multiset of letters formed by the first compartment, the second letter of the resulting string is the MEX letter of the multiset of letters formed by the second compartment, ... and so on. Please note, <span class="tex-font-style-it">under the constraint of this problem,</span> <span class="tex-font-style-bf">MEX letter can always be determined for any multiset found in this problem</span> because <span class="tex-font-style-tt">'z'</span> is not used.</p><p>What is the <span class="tex-font-style-bf">lexicographically greatest</span> resulting string possible that Ela can create?</p><p>A string $a$ is lexicographically greater than a string $b$ if and only if one of the following holds:</p><ul> <li> $b$ is a prefix of $a$, but $b \ne a$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears later in the alphabet than the corresponding letter in $b$. </li></ul><p>The <span class="tex-font-style-it">minimum excluded (MEX) letter</span> of a multiset of letters is the letter that appears earliest in the alphabet and is not contained in the multiset. For example, if a multiset of letters contains $7$ letters <span class="tex-font-style-tt">'b'</span>, <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>, <span class="tex-font-style-tt">'c'</span>, <span class="tex-font-style-tt">'e'</span>, <span class="tex-font-style-tt">'c'</span>, <span class="tex-font-style-tt">'f'</span> respectively, then the MEX letter of this compartment is <span class="tex-font-style-tt">'d'</span>, because <span class="tex-font-style-tt">'d'</span> is not included in the multiset, and all letters comes before <span class="tex-font-style-tt">'d'</span> in the alphabet, namely <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span> and <span class="tex-font-style-tt">'c'</span>, are included in the multiset.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 200$; $1 \le k \le n$). It is guaranteed that $n$ is divisible by $k$.</p><p>The second line of each test case contains a string of $n$ lowercase Latin letters from <span class="tex-font-style-tt">'a'</span> to <span class="tex-font-style-tt">'y'</span> inclusively. Each letter represents the starting letter of the title of a book in the initial heap.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output a string of $k$ letters which is the most optimal string that Ela can find.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 200$; $1 \le k \le n$). It is guaranteed that $n$ is divisible by $k$.</p><p>The second line of each test case contains a string of $n$ lowercase Latin letters from <span class="tex-font-style-tt">'a'</span> to <span class="tex-font-style-tt">'y'</span> inclusively. Each letter represents the starting letter of the title of a book in the initial heap.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, output a string of $k$ letters which is the most optimal string that Ela can find.</p>





```input1|2,3,6,7,10,11
5
12 3
cabccadabaac
12 6
cabccadabaac
12 12
cabccadabaac
25 1
abcdefghijklmnopqrstuvwxy
10 5
bcdxedbcfg
```




```output1
edb
ccbbba
bbbbbaaaaaaa
z
aaaaa
```



## Note

<p>In the first test case, the books can be divided into $3$ compartments as below:</p><ul> <li> the first compartment contains the books with indices $1, 2, 3, 7$: $multiset_1 = \{$<span class="tex-font-style-tt">'c'</span>, <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>, <span class="tex-font-style-tt">'d'</span>$\}$ $\rightarrow$ $MEX(multiset_1) =$ <span class="tex-font-style-tt">'e'</span> </li><li> the second compartment contains the books with indices $4, 5, 6, 9$ : $multiset_2 = \{$<span class="tex-font-style-tt">'c'</span>, <span class="tex-font-style-tt">'c'</span>, <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>$\}$ $\rightarrow$ $MEX(multiset_2) =$ <span class="tex-font-style-tt">'d'</span> </li><li> the third compartment contains the remaining books $8, 10, 11, 12$ : $multiset_3 = \{$ <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'c'</span>$\}$ $\rightarrow$ $MEX(multiset_3) =$ <span class="tex-font-style-tt">'b'</span> </li></ul><p>Therefore, the answer is <span class="tex-font-style-tt">'edb'</span>. It can be proven that there is no way that Ela can arrange the books so that it results in a lexicographically greater string.</p><center> <img class="tex-graphics" src="file://MTiSPeIH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
